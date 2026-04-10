---
id: doc-flows
title: Archidex — Flows
type: doc
subtype: flows
status: published
sequence: 5
createdAt: "2026-04-10T21:02:21.436Z"
updatedAt: "2026-04-10T21:02:21.436Z"
---

# Flows

### The Catch (Scan & Identify)

You are walking in downtown Chicago and see a soaring, ornate skyscraper. You pull out Archidex. The camera opens instantly. You align the building within the on-screen drafting crosshairs and tap the large capture button. 

The app freezes the frame. A satisfying haptic *thump* occurs. A blue "scanning line" sweeps down the photo, leaving geometric bounding boxes in its wake. The screen dims, and a card slides up from the bottom: **"Neo-Gothic."** 

The card displays a 96% confidence score. It highlights the bounding boxes on your photo: "Notice the pointed arches, the intricate tracery, and the vertical emphasis." You tap the "Add to Passport" button. A flurry of haptic ticks confirms the addition, and a notification appears: *New Style Unlocked! You've discovered your first Neo-Gothic building.* You put your phone away, feeling like you just learned a secret about the city.

### The Explorer (Map & Discover)

It's a Saturday afternoon, and you have an hour to kill in a new neighborhood. You open Archidex and swipe to the Architecture Radar. Your map is dark, but you see three gold pins nearby—buildings you captured last month. 

More importantly, you see a glowing blue ring three blocks away. It's an "Uncollected Landmark." You tap it. The preview says: "A prime example of *Streamline Moderne*, a style you haven't collected yet." You follow the map. When you arrive, you see a sleek, curved diner with glass blocks and chrome accents. You open the Lens, scan it, and claim the style for your Field Guide. The map updates, turning the blue ring into a gold pin. You've claimed the territory.

### The Scholar (Browse Field Guide)

You're on the train commuting home. You open the Field Guide to look at your collection. You scroll past the vibrant, full-color cards of styles you've captured: Brutalist, International, Art Deco. You stop at a grayed-out silhouette labeled "Beaux-Arts." 

You tap the silhouette. Because you haven't captured it yet, the gallery is empty, but you can read the history. You read about the grand, theatrical style taught at the École des Beaux-Arts in Paris. You look at the vector illustrations of rusticated ground floors and flat roofs. You close the card, making a mental note. Tomorrow, when you walk past the city library, you're going to look a little closer to see if it matches.

<flex_block type="flow">
{
  "id": "flow-scan-identify",
  "title": "The Catch",
  "actor": "Urban Explorer",
  "trigger": "Sees a fascinating building and wants to know what it is",
  "steps": [
    "Open app → Camera opens instantly",
    "Frame building in drafting crosshairs → Tap capture",
    "Watch 2-second scanning animation with haptic feedback",
    "View Result Card: Style name, era, and annotated photo",
    "Tap 'Add to Passport'",
    "See 'Style Unlocked' celebration screen"
  ],
  "outcome": "Identified a building, learned its style, and added it to the personal collection."
}
</flex_block>

<flex_block type="flow">
{
  "id": "flow-radar-discover",
  "title": "The Explorer",
  "actor": "Weekend Wanderer",
  "trigger": "Looking for a reason to walk around a neighborhood",
  "steps": [
    "Swipe to Architecture Radar map",
    "Spot a blue 'Uncollected Landmark' ring nearby",
    "Follow map to the physical location",
    "Recognize the building from the app's hint",
    "Use The Lens to scan and capture the building",
    "Map updates: Blue ring becomes a Gold Pin"
  ],
  "outcome": "Turned a casual walk into a successful scavenger hunt, completing a new style."
}
</flex_block>

<flex_block type="flow">
{
  "id": "flow-glossary-learn",
  "title": "The Scholar",
  "actor": "Curious User",
  "trigger": "Reading a style description and encountering an unknown term",
  "steps": [
    "Read description of Gothic Revival on a captured building",
    "See the word 'Ogee Arch' underlined",
    "Tap 'Ogee Arch'",
    "Bottom sheet slides up with an elegant vector illustration and simple definition",
    "Swipe sheet down to dismiss",
    "Continue reading with newfound understanding"
  ],
  "outcome": "Learned architectural vocabulary instantly without leaving the context of the reading."
}
</flex_block>

---

<flex_block type="flow" id="blk-001" name="Flow 1">
{
  "id": "flow-scan-identify",
  "title": "The Catch",
  "actor": "Urban Explorer",
  "trigger": "Sees a fascinating building and wants to know what it is",
  "steps": [
    "Open app → Camera opens instantly",
    "Frame building in drafting crosshairs → Tap capture",
    "Watch 2-second scanning animation with haptic feedback",
    "View Result Card: Style name, era, and annotated photo",
    "Tap 'Add to Passport'",
    "See 'Style Unlocked' celebration screen"
  ],
  "outcome": "Identified a building, learned its style, and added it to the personal collection."
}
</flex_block>

<flex_block type="flow" id="blk-002" name="Flow 2">
{
  "id": "flow-radar-discover",
  "title": "The Explorer",
  "actor": "Weekend Wanderer",
  "trigger": "Looking for a reason to walk around a neighborhood",
  "steps": [
    "Swipe to Architecture Radar map",
    "Spot a blue 'Uncollected Landmark' ring nearby",
    "Follow map to the physical location",
    "Recognize the building from the app's hint",
    "Use The Lens to scan and capture the building",
    "Map updates: Blue ring becomes a Gold Pin"
  ],
  "outcome": "Turned a casual walk into a successful scavenger hunt, completing a new style."
}
</flex_block>

<flex_block type="flow" id="blk-003" name="Flow 3">
{
  "id": "flow-glossary-learn",
  "title": "The Scholar",
  "actor": "Curious User",
  "trigger": "Reading a style description and encountering an unknown term",
  "steps": [
    "Read description of Gothic Revival on a captured building",
    "See the word 'Ogee Arch' underlined",
    "Tap 'Ogee Arch'",
    "Bottom sheet slides up with an elegant vector illustration and simple definition",
    "Swipe sheet down to dismiss",
    "Continue reading with newfound understanding"
  ],
  "outcome": "Learned architectural vocabulary instantly without leaving the context of the reading."
}
</flex_block>
