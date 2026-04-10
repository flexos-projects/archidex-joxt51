---
id: doc-pages
title: "Pages & Screens"
type: doc
status: active
createdAt: "2026-04-10"
relatesTo: ["docs/002-features.md"]
---

# 3. Pages & Screens

The user interface of Archidex is designed to be spatial and intuitive, prioritizing the camera as the home screen. The structure is mobile-first and built around the core features of scanning, collecting, and exploring.

## App Screens

### /lens (The Lens - Camera)
The default, "home" screen of the application. This is not a menu, but an active tool.
- **Purpose:** To enable the core action of capturing a building with zero friction.
- **Key Components:** Live camera feed, drafting-style crosshairs, a large capture button, and a minimal bottom navigation bar.
- **Features Hosted:** `f-001: The Lens`

### /capture/:id (Capture Result)
A full-screen modal that appears immediately after a building is scanned. It's the "reveal" moment.
- **Purpose:** To present the AI's findings in a clear, exciting, and educational way.
- **Key Components:** The user's photo with annotations overlaid, the identified style in large typography, a confidence score, and a brief description. A primary CTA "Add to Passport" saves the capture.
- **Features Hosted:** `f-003: Annotated Breakdown`, `f-007: Capture Cards` (sharing is initiated from here).

### /guide (Field Guide)
The main collection view, accessible via the bottom nav or by swiping.
- **Purpose:** To allow users to browse their collection, see what they're missing, and learn more about architectural styles.
- **Key Components:** A grid of cards for all styles. Discovered styles show a photo; undiscovered styles show a mysterious silhouette.
- **Features Hosted:** `f-002: The Field Guide`

### /guide/style/:id (Style Detail)
A deep-dive page for a specific architectural style, accessed by tapping a card in the Field Guide.
- **Purpose:** To provide rich, encyclopedic content about a style the user has discovered.
- **Key Components:** A hero image, historical description, list of defining features (with glossary links), and a gallery of all the user's personal captures of that style.
- **Features Hosted:** `f-002: The Field Guide`, `f-006: Visual Glossary`

### /map (Architecture Radar)
The map view, accessible via the bottom nav or by swiping.
- **Purpose:** To encourage active exploration by showing users what's nearby.
- **Key Components:** A custom-styled map. Gold pins represent the user's previous captures. Glowing blue rings represent "Uncollected Landmarks" nearby.
- **Features Hosted:** `f-005: Architecture Radar`

### /passport (Passport - Profile)
The user's profile and gamification hub, accessible from the bottom nav.
- **Purpose:** To track progress, celebrate achievements, and drive long-term engagement.
- **Key Components:** A summary dashboard of stats (styles found, cities explored), a collection of beautifully designed digital "stamps" for unlocked milestones.
- **Features Hosted:** `f-004: The Passport`

### /glossary (Glossary)
A searchable list of all architectural terms.
- **Purpose:** To provide a central, searchable dictionary of architectural vocabulary.
- **Key Components:** A simple A-Z searchable list. Each entry opens a bottom-sheet with a vector illustration and definition. This screen is a secondary access point; most users will interact with the glossary via contextual pop-ups.
- **Features Hosted:** `f-006: Visual Glossary`

## Utility & Web Pages

### /login (Authentication)
A simple, modal-based screen for account management.
- **Purpose:** To allow users to sign up or log in to sync their collection across devices. The focus is on social logins to minimize friction.

### / (Marketing Landing Page)
A web-only page to drive app downloads.
- **Purpose:** To explain the app's value proposition, showcase its design, and serve as the primary destination for marketing campaigns.
- **Key Components:** Hero section with tagline, interactive scanner demo, feature breakdown, and prominent App Store / Google Play download buttons.

<flex_block type="page-inventory">
{
  "pages": [
    { "route": "/", "name": "Landing Page", "type": "marketing", "description": "Web-only. App showcase, interactive scanner demo, download CTAs." },
    { "route": "/lens", "name": "The Lens (Camera)", "type": "app", "description": "The default view. Live camera feed, drafting crosshairs, capture button." },
    { "route": "/capture/:id", "name": "Capture Result", "type": "app", "description": "Post-scan analysis. Annotated photo, style classification, add-to-collection CTA." },
    { "route": "/guide", "name": "Field Guide", "type": "app", "description": "Grid of all architectural styles. Discovered vs. undiscovered silhouettes." },
    { "route": "/guide/style/:id", "name": "Style Detail", "type": "app", "description": "History, defining features, and your personal gallery for a specific style." },
    { "route": "/map", "name": "Architecture Radar", "type": "app", "description": "Map view of your captures and nearby uncollected landmarks." },
    { "route": "/passport", "name": "Passport (Profile)", "type": "app", "description": "Your stats, digital stamps, and journey across cities." },
    { "route": "/glossary", "name": "Glossary", "type": "app", "description": "Searchable visual dictionary of architectural terms and elements." },
    { "route": "/login", "name": "Auth", "type": "auth", "description": "Simple social login to save your collection across devices." }
  ]
}
</flex_block>
