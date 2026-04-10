---
id: doc-technical
title: Archidex — Technical
type: doc
subtype: technical
status: published
sequence: 7
createdAt: "2026-04-10T21:02:21.436Z"
updatedAt: "2026-04-10T21:02:21.436Z"
---

# Technical

Archidex processes complex visual data in real-time while rendering a fast, fluid, gamified interface. It uses a modern stack designed for offline-capable collection tracking and high-performance camera integration.

<flex_block type="stack">
{
  "framework": { "name": "React Native / Expo (PWA fallback)", "why": "Native camera APIs are essential for the 'Lens' feel, but a PWA serves as a frictionless web entry point." },
  "database": { "name": "Convex", "why": "Real-time sync for the Passport and seamless offline-caching for when users are exploring areas with bad cell service." },
  "auth": { "name": "Clerk", "why": "Social login that just works. Users don't want to manage passwords while standing on a sidewalk." },
  "ai_vision": { "name": "GPT-4o / Claude 3.5 Sonnet", "why": "State-of-the-art multimodal vision capability to accurately classify obscure architectural styles and provide bounding box coordinates." },
  "maps": { "name": "Mapbox", "why": "Custom map styling allows the 'Architecture Radar' to match the app's blueprint aesthetic instead of looking like generic Google Maps." },
  "hosting": { "name": "Vercel", "why": "Edge-rendered landing pages and fast API routes for routing images to the AI models." }
}
</flex_block>

The most technically complex part is the prompt engineering and coordinate mapping for the annotated breakdown. The app takes the photo, compresses it, and sends it to the vision model with a strict JSON schema prompt: "Identify the style. List 2-3 key features visible in the image, and provide bounding box coordinates [x, y, w, h] relative to the image dimensions for each feature." The frontend then renders CSS overlays based on those coordinates.

---

<flex_block type="stack" id="blk-001" name="Tech Stack">
{
  "framework": {
    "name": "React Native / Expo (PWA fallback)",
    "why": "Native camera APIs are essential for the 'Lens' feel, but a PWA serves as a frictionless web entry point."
  },
  "database": {
    "name": "Convex",
    "why": "Real-time sync for the Passport and seamless offline-caching for when users are exploring areas with bad cell service."
  },
  "auth": {
    "name": "Clerk",
    "why": "Social login that just works. Users don't want to manage passwords while standing on a sidewalk."
  },
  "ai_vision": {
    "name": "GPT-4o / Claude 3.5 Sonnet",
    "why": "State-of-the-art multimodal vision capability to accurately classify obscure architectural styles and provide bounding box coordinates."
  },
  "maps": {
    "name": "Mapbox",
    "why": "Custom map styling allows the 'Architecture Radar' to match the app's blueprint aesthetic instead of looking like generic Google Maps."
  },
  "hosting": {
    "name": "Vercel",
    "why": "Edge-rendered landing pages and fast API routes for routing images to the AI models."
  }
}
</flex_block>
