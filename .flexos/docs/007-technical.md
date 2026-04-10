---
id: doc-technical
title: "Technical Specification"
type: doc
status: active
createdAt: "2026-04-10"
relatesTo: ["docs/002-features.md", "docs/004-database.md", "docs/006-design.md"]
---

# 7. Technical Specification

The technology stack for Archidex is chosen to deliver a high-performance, native-feeling mobile experience with a heavy reliance on real-time data synchronization, offline capabilities, and cutting-edge AI.

## The Stack

<flex_block type="stack">
{
  "framework": { 
    "name": "React Native / Expo", 
    "why": "The 'Lens' feature requires high-performance, native camera APIs for a fluid, responsive feel. Expo provides a robust development environment and simplifies the build process for both iOS and Android. A PWA fallback using Expo for Web can serve as a frictionless entry point for users who don't want to download an app." 
  },
  "database": { 
    "name": "Convex", 
    "why": "The gamified, collection-based nature of the Passport and Field Guide requires real-time data sync. Convex's architecture is ideal for this. Its seamless offline caching and synchronization are critical for users who are exploring areas with poor cell service, ensuring captures are never lost." 
  },
  "auth": { 
    "name": "Clerk", 
    "why": "Authentication needs to be as frictionless as possible. Users will be on a sidewalk, often with one hand. Clerk's pre-built components for social logins (Google, Apple) are perfect for this, removing the need to manage passwords."
  },
  "ai_vision": { 
    "name": "GPT-4o / Claude 3.5 Sonnet", 
    "why": "The core feature—identifying architectural styles and elements from a photo—requires state-of-the-art multimodal vision capabilities. These models can accurately classify styles from imperfect images and provide the structured JSON output (including bounding box coordinates) needed for the Annotated Breakdown feature."
  },
  "maps": { 
    "name": "Mapbox", 
    "why": "The 'Architecture Radar' is a key discovery feature that must align with the app's unique 'blueprint' aesthetic. Mapbox's extensive customization capabilities are essential for this, allowing us to create a map that feels like part of the Archidex world, not a generic Google Maps embed."
  },
  "hosting": { 
    "name": "Vercel", 
    "why": "For the marketing website and API endpoints that serve the app. Vercel provides a simple, powerful platform for hosting the Next.js-based landing page and serverless functions that will route image data to the AI vision models for analysis."
  }
}
</flex_block>

## Key Technical Challenges

### AI Prompt Engineering & Latency
The most complex technical component is the interaction with the vision model.
1.  **Prompting for Structured Data:** The prompt sent to the AI must be carefully engineered to request a specific JSON schema in return: `{ "style": "Art Deco", "confidence": 0.92, "elements": [ { "name": "Geometric Ornamentation", "box": [0.1, 0.2, 0.3, 0.4] } ] }`. This ensures the response can be reliably parsed.
2.  **Coordinate Mapping:** The bounding box coordinates (`box`) returned by the AI must be mapped from the compressed image dimensions sent for analysis back to the original device screen dimensions to render the overlays accurately.
3.  **Latency Masking:** An AI round-trip can take 2-4 seconds. As noted in the Design spec, the UI must feature an engaging "scanning" animation. This is not just cosmetic; it's a crucial UX element to make the wait feel like the app is "thinking" rather than "loading."

### Offline-First Data Sync
Users will frequently be in areas with spotty connectivity. The application logic must be robust enough to handle this:
- **Local-First Captures:** When a user taps 'Capture', the photo, GPS data, and timestamp must be saved immediately to local device storage.
- **Queueing System:** The analysis request should be added to a queue.
- **Background Sync:** When connectivity is restored, the queue is processed in the background. The AI analysis is performed, and the user's data (`Captures`, `Milestones`) is synced with the server.
- **Delayed Notifications:** "Style Unlocked" and "Milestone Achieved" notifications should only be triggered after a successful background sync, ensuring the user sees them when they next open the app with a connection.
