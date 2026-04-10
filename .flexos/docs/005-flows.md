---
id: doc-flows
title: "User Flows"
type: doc
status: active
createdAt: "2026-04-10"
relatesTo: ["docs/003-pages.md", "docs/004-database.md"]
---

# 5. User Flows

User flows describe the primary paths users take through the Archidex app to accomplish their goals. These narrative journeys connect the app's pages, features, and data into a cohesive experience.

## Core Flow: "The Catch" (Scan & Identify)

This is the central loop of the app. It's the moment of discovery and collection.

- **Actor:** An Urban Explorer walking through a city.
- **Trigger:** They see a fascinating building and want to know its story.
- **Flow:**
    1. **Open App:** The user opens Archidex, which defaults immediately to `/lens`.
    2. **Frame & Capture:** They align the building in the drafting crosshairs and tap the capture button.
    3. **Analysis:** The app displays a brief, engaging scanning animation while the AI processes the image. A new `Capture` record is being created in the background.
    4. **View Result:** The `/capture/:id` modal slides up, displaying the identified `Style` (e.g., "Neo-Gothic"), confidence score, and the annotated photo showing key `Elements`.
    5. **Save to Collection:** The user taps "Add to Passport." The `Capture` record is now permanently associated with their `User` profile.
    6. **Celebration:** If this is the first time they've found this `Style`, a "New Style Unlocked!" celebration is shown. If the capture triggers a `Milestone`, a "New Stamp Awarded!" notification appears.
- **Outcome:** The user has identified a building, learned about its style, and added it to their personal collection, deepening their connection to their surroundings.

<flex_block type="flow">
{
  "id": "flow-scan-identify",
  "title": "The Catch",
  "actor": "Urban Explorer",
  "trigger": "Sees a fascinating building and wants to know what it is",
  "steps": [
    "Open app → /lens",
    "Frame building in drafting crosshairs → Tap capture",
    "Watch 2-second scanning animation with haptic feedback",
    "View Result Card (/capture/:id): Style name, era, and annotated photo",
    "Tap 'Add to Passport'",
    "See 'Style Unlocked' celebration screen"
  ],
  "outcome": "Identified a building, learned its style, and added it to the personal collection."
}
</flex_block>


## Discovery Flow: "The Explorer" (Map & Discover)

This flow is for when a user wants to be actively guided to new architectural finds.

- **Actor:** A Weekend Wanderer with an hour to kill in a new neighborhood.
- **Trigger:** Looking for a reason to walk around and explore.
- **Flow:**
    1. **Open Map:** The user navigates to the `/map` screen.
    2. **Find Landmark:** They see their previously collected `Captures` (gold pins) and spot a glowing blue ring nearby—an "Uncollected Landmark."
    3. **Navigate:** They tap the ring, see a hint ("A prime example of *Streamline Moderne*"), and walk towards the location.
    4. **Identify & Capture:** Upon arrival, they recognize the building. They switch to `/lens` and perform "The Catch" flow.
    5. **Update Map:** After adding the building to their passport, they can return to the `/map` to see the blue ring has been replaced by a new gold pin.
- **Outcome:** The user turned a casual walk into a successful scavenger hunt, discovering a new part of their city and a new `Style` for their collection.

<flex_block type="flow">
{
  "id": "flow-radar-discover",
  "title": "The Explorer",
  "actor": "Weekend Wanderer",
  "trigger": "Looking for a reason to walk around a neighborhood",
  "steps": [
    "Navigate to Architecture Radar (/map)",
    "Spot a blue 'Uncollected Landmark' ring nearby",
    "Follow map to the physical location",
    "Recognize the building from the app's hint",
    "Use The Lens to scan and capture the building",
    "Map updates: Blue ring becomes a Gold Pin"
  ],
  "outcome": "Turned a casual walk into a successful scavenger hunt, completing a new style."
}
</flex_block>

## Learning Flow: "The Scholar" (Browse & Learn)

This flow describes how users engage with the educational content of the app when not actively scanning.

- **Actor:** A Curious User on their commute.
- **Trigger:** Wants to review their collection and learn more about what they've found.
- **Flow:**
    1. **Browse Guide:** The user opens the `/guide` and scrolls through their collected `Styles`.
    2. **Select Style:** They tap on a `Style` they want to know more about, navigating to `/guide/style/:id`.
    3. **Read Description:** They read the history of the style. They see an underlined architectural term (an `Element`), like "Ogee Arch."
    4. **Open Glossary:** They tap the term. A bottom-sheet modal appears with a vector illustration and a simple definition of the `Element`.
    5. **Dismiss & Continue:** They swipe the sheet away and continue reading with a deeper understanding.
- **Outcome:** The user learned architectural vocabulary instantly and frictionlessly, deepening their knowledge without leaving the context of what they were reading.

<flex_block type="flow">
{
  "id": "flow-glossary-learn",
  "title": "The Scholar",
  "actor": "Curious User",
  "trigger": "Reading a style description and encountering an unknown term",
  "steps": [
    "Navigate to Field Guide (/guide)",
    "Select a discovered style → /guide/style/:id",
    "See an underlined term like 'Ogee Arch' in the description",
    "Tap the term",
    "Bottom sheet slides up with an illustration and definition from the Glossary",
    "Swipe sheet down to dismiss and continue reading"
  ],
  "outcome": "Learned architectural vocabulary instantly without leaving the context of the reading."
}
</flex_block>
