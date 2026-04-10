---
id: doc-features
title: "Features"
type: doc
status: active
createdAt: "2026-04-10"
relatesTo: ["docs/001-vision.md"]
---

# 2. Features

Based on the vision of making architectural discovery a gamified, accessible experience, the features of Archidex are designed to create a tight loop of scanning, learning, and collecting.

## Core Features

These features represent the primary user journey and the core "Pokedex for buildings" loop.

### f-001: The Lens (AI Scanner)
This is the heart of the app. It's the action of "catching" a building. The experience must be fast, tactile, and magical.
- **Live Camera View:** Opens directly to the camera.
- **Drafting Reticle:** On-screen crosshairs to help users frame their subject.
- **One-Tap Capture:** A single, satisfying tap to initiate the scan.
- **AI Analysis:** The image is sent to a multimodal AI to identify the architectural style, era, and key elements.
- **Haptic Feedback:** Deeply satisfying physical feedback to make the capture feel tangible.

### f-002: The Field Guide
The collection album. This feature provides the motivation to keep exploring, turning the world into a museum where the user is the curator.
- **Style Encyclopedia:** A canonical, non-user-editable database of architectural styles.
- **Discovered vs. Undiscovered States:** Styles the user has found are shown in full color with their best photo. Undiscovered styles are represented by mysterious silhouettes, driving curiosity.
- **Rich Style Pages:** Each unlocked style has a dedicated page with its history, defining features, and a gallery of the user's captures of that style.

### f-003: Annotated Breakdown
This transforms the app from a labeling tool into a visual educator, directly answering the "why" for the user.
- **AI-Powered Annotations:** The vision model identifies specific architectural elements in the user's photo.
- **Visual Overlays:** Bounding boxes and labels are drawn directly on the captured image, pointing out things like "Mansard Roof," "Palladian Window," or "Ionic Capital."
- **Glossary Integration:** Tapping on a labeled element links directly to its definition in the Visual Glossary.

### f-004: The Passport
The gamified profile hub that tracks progress and rewards discovery. This is the primary long-term retention driver.
- **Personal Stats:** Tracks key metrics like unique styles found, cities explored, and total captures.
- **Digital Stamps & Milestones:** Achievements are awarded for collection patterns (e.g., "Capture 5 Brutalist buildings," "Scan your first building from the 18th century").
- **Collection Visualization:** Shows the user's journey and rarest finds in a visually compelling way.

## Supporting Features

These features enrich the core loop, adding utility, discovery vectors, and social sharing capabilities.

### f-005: Architecture Radar (Map)
Turns passive discovery into active hunting, generating walking tours on the fly.
- **Map View:** Displays the user's past captures as pins.
- **Uncollected Landmarks:** Highlights nearby, notable buildings of styles the user is missing, encouraging exploration.

### f-006: Visual Glossary
Removes the friction from learning the academic vocabulary of architecture.
- **Searchable Dictionary:** A simple, A-Z list of architectural terms.
- **Illustrated Definitions:** Each term has a clean vector illustration and a concise, easy-to-understand definition.
- **Contextual Access:** Can be accessed from anywhere in the app by tapping an underlined term.

### f-007: Capture Cards (Social Sharing)
Provides a high-quality, organic growth channel by letting users share their discoveries.
- **Sharable Asset:** Every capture generates a beautiful "trading card" with the user's photo, the identified style, location, and date.
- **Premium Design:** The card is designed to look like a premium museum placard, making it highly shareable on platforms like Instagram Stories.

<flex_block type="feature-list">
{
  "core": [
    {
      "id": "f-001",
      "icon": "lucide:scan-line",
      "title": "The Lens",
      "summary": "Point, snap, and identify. Real-time AI analysis of building facades and structural styles."
    },
    {
      "id": "f-002",
      "icon": "lucide:book-open",
      "title": "The Field Guide",
      "summary": "Your collector's album of architectural styles. Locked silhouettes until you find them in the wild."
    },
    {
      "id": "f-003",
      "icon": "lucide:microscope",
      "title": "Annotated Breakdown",
      "summary": "Visual callouts on your photo pointing out exact elements like pediments, arches, and cornices."
    },
    {
      "id": "f-004",
      "icon": "lucide:stamp",
      "title": "The Passport",
      "summary": "Track your journey. Digital stamps for cities visited, styles captured, and rare milestones."
    }
  ],
  "supporting": [
    {
      "id": "f-005",
      "icon": "lucide:map",
      "title": "Architecture Radar",
      "summary": "A map showing your captures and nearby uncollected architectural landmarks."
    },
    {
      "id": "f-006",
      "icon": "lucide:library",
      "title": "Visual Glossary",
      "summary": "An illustrated dictionary of terms. Never wonder what a 'flying buttress' is again."
    },
    {
      "id": "f-007",
      "icon": "lucide:share-2",
      "title": "Capture Cards",
      "summary": "Export your finds as beautiful, museum-placard style trading cards for social media."
    }
  ]
}
</flex_block>
