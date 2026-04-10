---
id: seed
title: "Archidex"
type: seed
status: draft
createdAt: "2026-04-08"
updatedAt: "2026-04-08"
---

<flex_block type="seed-header">
{
  "name": "Archidex",
  "tagline": "The field guide to the built world",
  "description": "Point your camera at any building to instantly identify its architectural style. Collect cities, learn the language of design, and see the streets with new eyes.",
  "logo": null,
  "domain": "archidex.app",
  "inputType": "sentence"
}
</flex_block>

# Archidex

## 1. Vision

Architecture is the most public art form in the world, yet its language is locked behind academic degrees and heavy textbooks. We walk past masterpieces every day—on our way to get coffee, on our commutes, on vacations in new cities—and we feel a sense of wonder, but we lack the vocabulary to explain *why*. We know a building looks "old" or "modern" or "blocky," but we don't know the words *Beaux-Arts*, *Mid-Century Modern*, or *Brutalism*. 

Archidex changes how we look at cities. 

By turning the smartphone camera into an architectural lens, Archidex gamifies the act of looking up. It is a Pokedex for the built environment. You point your phone at a building, the AI analyzes the facade, and instantly breaks it down: "Art Deco. Notice the geometric ornamentation, the vertical emphasis, and the stylized terra cotta." It adds the building to your collection. Suddenly, you aren't just walking down a street; you are on a safari.

This product is for the urban explorer, the tourist, the design nerd, the history buff, and the person who just moved to a new city and wants to understand its bones. It is not for licensed architects to do their jobs (they already know what a Corinthian column is). It is for the rest of us, to give us the joy of recognition. 

The timing for this is perfect. Five years ago, computer vision could tell you "this is a building." Today, multimodal AI models can parse the difference between a Gothic arch and a Romanesque arch in milliseconds, even from a blurry photo taken across the street. The technology is finally ready to deliver on the magic.

But the magic isn't just the AI. The magic is the *collection*. When you capture a Victorian home in San Francisco, it goes into your Passport. You start trying to "complete" neighborhoods. You go out of your way to find a rare piece of Deconstructivism. You start noticing the corbels, the lintels, the flying buttresses. Archidex doesn't just tell you what a building is; it rewires your brain to constantly observe the details of the world around you.

If Archidex were a person at a party, they would be the fascinating local historian who knows every secret of the neighborhood. They wouldn't lecture you; they would pull you aside, point out a hidden gargoyle near the roofline that you'd never noticed, tell you a one-minute story about it, and leave you feeling like an insider.

<flex_block type="brand">
{
  "personality": ["curious", "academic but accessible", "tactile", "observant"],
  "voiceAttributes": ["speaks like a passionate tour guide", "uses precise terminology but immediately defines it", "celebrates discovery", "never pedantic"],
  "values": ["the world is a museum", "knowledge should be collected", "look up"],
  "visualMood": "A modern field guide. Blueprint blues, drafting-paper creams, concrete greys, and terracotta accents. Geometric, structured, and highly legible. It feels like a beautiful reference book crossed with a digital HUD.",
  "references": ["Pokedex interfaces (structured data, collection mechanics)", "Vintage architectural blueprints", "The layout of Monocle magazine", "Strava's sense of personal achievement"]
}
</flex_block>

---

## 2. Features

### The Lens (AI Scanner)

This is the core loop. You open the app, and the camera is live. A bespoke framing reticle—designed to look like drafting crosshairs—helps you center the building. You tap to capture. The screen dims slightly, scanning lines sweep over the image, and the AI processes the facade. Within seconds, it returns a "Capture Card" detailing the primary style, the estimated era, and confidence level. The experience is tactile, fast, and accompanied by deeply satisfying haptic feedback, making the act of "catching" a building feel physical.

### The Field Guide

An encyclopedia of architectural styles, structural elements, and historical eras. But unlike a Wikipedia page, this is structured like a collector's album. Styles you haven't found yet are rendered as beautiful, mysterious silhouettes (like undiscovered Pokemon). When you capture your first Brutalist building, the "Brutalism" page unlocks in full color, revealing the history, the defining features (raw concrete, massive forms), and your personal gallery of captures for that style.

### Annotated Breakdown

When you capture a building, the AI doesn't just give you a name. It overlays the photo with structural annotations. A line points to the roof: "Mansard Roof." A line points to the window: "Palladian Window." A box highlights the column: "Ionic Capital." This feature transforms the app from a simple labeling tool into a visual educator. You aren't just told what the style is; you are shown *why*.

### The Passport (Your Collection)

Your personal profile and gamified collection hub. It tracks the cities you've scanned, the unique styles you've discovered, and your rarest finds. It features a literal "Passport" view full of digital stamps from different architectural eras and regions. "You've captured 14 of the 20 distinct styles found in Chicago." This drives retention. It turns a casual walk into a scavenger hunt.

### Architecture Radar (Map)

A map view of your city, but filtered through the lens of design. It shows pins for your previous captures, but more importantly, it shows "Uncollected Landmarks"—notable buildings nearby that represent styles you are missing. "There is a prime example of Neo-Classical architecture 0.4 miles away." It acts as a walking-tour generator, guiding users to explore new streets.

### The Glossary

A searchable, visual dictionary of architectural terms. When reading a building description, terms like *clerestory*, *pediment*, or *rustication* are underlined. Tapping them brings up a bottom-sheet glossary card with a clean, vector illustration of the element. It removes the friction of learning the vocabulary.

### Capture Cards (Social Sharing)

Every capture generates a beautiful, shareable "Trading Card." It features your photo perfectly cropped, the architectural style in bold typography, the location, and the date. It looks like a premium museum placard. Users can export these directly to Instagram Stories or share them with friends, serving as a high-quality organic growth engine for the app.

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

---

## 3. Pages

The Archidex experience is mobile-first and deeply spatial. The app opens immediately to The Lens—the camera is the home screen, just like Snapchat or Pokemon Go. The interface here is minimal: drafting-style crosshairs, a large capture button, and a bottom navigation bar. 

When you capture a building, a full-screen Modal slides up over the camera. This is the **Capture Result** page. It begins with an analyzing animation (blueprint lines scanning over your photo), then snaps to the result. Your photo is at the top, annotated. Below is the style name in massive typography, a confidence score, and a breakdown of why the AI made this choice. From here, you can tap "Add to Passport."

Swiping left from the camera takes you to **The Field Guide**. This page is a grid of beautiful cards. Discovered styles show your best capture photo. Undiscovered styles show a blueprint-blue silhouette with a question mark. Tapping a discovered style opens the **Style Detail** page: a rich, editorial layout explaining the history of Art Deco or Gothic Revival, complete with a timeline and a gallery of all your captures of that style.

Swiping right from the camera takes you to the **Architecture Radar** map. It's a dark-mode styled map (even in light mode, to make pins pop). Gold pins are your captures. Blue rings are nearby uncollected landmarks. Tapping a pin brings up a quick-look card of the building.

The **Passport** is accessible from the bottom nav. It acts as your user profile. It shows a summary dashboard: "14 Styles Found | 3 Cities Explored | 42 Total Captures." Below are beautifully designed digital stamps representing achievements (e.g., "The Concrete Jungle" for finding 5 Brutalist buildings). 

The **Glossary** lives as a searchable database accessible via a top-right icon in the Field Guide, or invoked via bottom-sheets whenever a technical term is tapped anywhere in the app.

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

---

## 4. Data

At the heart of Archidex is the **Capture**. A Capture represents a specific moment when a user documented a building. It contains the raw photo, the AI's structural annotations (coordinates on the image), the GPS location, and the identified Style.

Captures link to **Styles**. Styles are the canonical database of architectural history—Brutalist, Romanesque, Mid-Century Modern, Queen Anne. A Style is not user-generated; it is the master record that contains the historical description, the era, and the defining elements. 

Styles are made up of **Elements**. Elements are the specific vocabulary words of architecture: *Corbel*, *Dormer Window*, *Flying Buttress*. Elements populate the Glossary and are the exact things the AI is drawing bounding boxes around in the Annotated Breakdown.

The gamification layer is driven by **Milestones**. A Milestone is logic evaluating a user's Captures. If a user has 5 Captures linked to the "Brutalist" Style, they unlock the "Concrete Jungle" Milestone, which awards a digital Stamp to their Passport. 

<flex_block type="data-model">
{
  "collections": [
    {
      "name": "Users",
      "icon": "lucide:user",
      "description": "The explorers. Tracks their overall progress, home city, and settings.",
      "keyFields": ["username", "avatar", "homeCity", "totalCaptures", "joinedAt"],
      "relationships": ["captures → Captures", "unlockedMilestones → Milestones"]
    },
    {
      "name": "Captures",
      "icon": "lucide:camera",
      "description": "An instance of a user scanning a building. The core user-generated entity.",
      "keyFields": ["photoUrl", "location (lat/lng)", "confidenceScore", "annotations (JSON)", "capturedAt"],
      "relationships": ["user → Users", "style → Styles"]
    },
    {
      "name": "Styles",
      "icon": "lucide:landmark",
      "description": "The canonical database of architectural movements (e.g., Art Deco, Gothic).",
      "keyFields": ["name", "eraStart", "eraEnd", "description", "silhouetteImage", "keyFeatures"],
      "relationships": ["elements → Elements", "captures → Captures"]
    },
    {
      "name": "Elements",
      "icon": "lucide:puzzle",
      "description": "The structural building blocks and vocabulary (e.g., Gargoyle, Pilaster).",
      "keyFields": ["name", "definition", "vectorIllustrationUrl", "category"],
      "relationships": ["styles → Styles"]
    },
    {
      "name": "Milestones",
      "icon": "lucide:award",
      "description": "Achievements users can unlock based on their collection patterns.",
      "keyFields": ["title", "description", "stampImageUrl", "requirementLogic", "rarity"],
      "relationships": ["users → Users"]
    }
  ]
}
</flex_block>

---

## 5. Flows

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

## 6. Design

Archidex is a digital field guide. The design language must bridge two worlds: the historic, physical reality of architecture, and the precise, gamified nature of a collection app. 

The visual identity is rooted in the aesthetics of architectural drafting and blueprints. The interface feels highly structured, governed by clear grids, visible hairlines, and precise spacing. It avoids the soft, bubbly, heavily shadowed look of typical consumer apps. Instead, corners have tighter radii (`--radius-sm` or `--radius-md`), mimicking the sharp intersections of buildings.

In Dark Mode (the default "Blueprint" theme), backgrounds are a deep, inky navy blue, not standard black. Accents are electric cyan and drafting-pencil yellow, making annotations and UI elements pop like chalk on a blueprint. In Light Mode (the "Drafting Paper" theme), the background is a warm, textured cream, with deep charcoal text and terracotta accents, evoking classic reference books and masonry.

Typography is critical. The display font is a structured, geometric sans-serif (Space Grotesk or Archivo) that looks like it could be on an engineering diagram. The body font is highly legible (Inter), while data points (GPS coordinates, eras, confidence scores) use a monospace font to emphasize precision.

Photography is treated as the hero. UI elements overlaying photos (like the scanner reticle or annotations) are crisp, thin, and utilitarian. The app should feel like a piece of high-end specialized equipment—a tricorder for design nerds.

<flex_block type="tokens">
{
  "category": "colors",
  "mode": "dark",
  "tokens": {
    "--color-primary": "oklch(75% 0.15 230)",
    "--color-primary-hover": "oklch(80% 0.15 230)",
    "--color-primary-active": "oklch(70% 0.15 230)",
    "--color-primary-muted": "oklch(75% 0.15 230 / 0.15)",
    "--color-accent": "oklch(85% 0.18 90)",
    "--color-bg": "oklch(18% 0.04 250)",
    "--color-surface": "oklch(23% 0.04 250)",
    "--color-surface-raised": "oklch(28% 0.03 250)",
    "--color-surface-overlay": "oklch(15% 0.04 250 / 0.8)",
    "--color-border": "oklch(35% 0.03 250)",
    "--color-border-subtle": "oklch(28% 0.03 250)",
    "--color-text": "oklch(95% 0.01 250)",
    "--color-text-secondary": "oklch(75% 0.02 250)",
    "--color-text-muted": "oklch(60% 0.02 250)",
    "--color-text-on-primary": "oklch(15% 0.04 250)",
    "--color-success": "oklch(75% 0.12 160)",
    "--color-warning": "oklch(85% 0.18 90)",
    "--color-error": "oklch(65% 0.15 25)"
  }
}
</flex_block>

<flex_block type="tokens">
{
  "category": "colors",
  "mode": "light",
  "tokens": {
    "--color-primary": "oklch(45% 0.12 250)",
    "--color-primary-hover": "oklch(40% 0.12 250)",
    "--color-primary-active": "oklch(35% 0.12 250)",
    "--color-primary-muted": "oklch(45% 0.12 250 / 0.12)",
    "--color-accent": "oklch(55% 0.15 45)",
    "--color-bg": "oklch(97% 0.01 85)",
    "--color-surface": "oklch(99% 0.005 85)",
    "--color-surface-raised": "oklch(100% 0 0)",
    "--color-surface-overlay": "oklch(95% 0.01 85 / 0.8)",
    "--color-border": "oklch(85% 0.01 85)",
    "--color-border-subtle": "oklch(90% 0.01 85)",
    "--color-text": "oklch(25% 0.02 250)",
    "--color-text-secondary": "oklch(45% 0.02 250)",
    "--color-text-muted": "oklch(60% 0.02 250)",
    "--color-text-on-primary": "oklch(98% 0 0)",
    "--color-success": "oklch(50% 0.12 160)",
    "--color-warning": "oklch(60% 0.15 45)",
    "--color-error": "oklch(55% 0.15 25)"
  }
}
</flex_block>

<flex_block type="tokens">
{
  "category": "typography",
  "tokens": {
    "--font-display": "'Space Grotesk', system-ui, sans-serif",
    "--font-body": "'Inter', system-ui, sans-serif",
    "--font-mono": "'JetBrains Mono', monospace",
    "--font-size-xs": "0.75rem",
    "--font-size-sm": "0.875rem",
    "--font-size-base": "1rem",
    "--font-size-lg": "1.125rem",
    "--font-size-xl": "1.25rem",
    "--font-size-2xl": "1.5rem",
    "--font-size-3xl": "2rem",
    "--font-size-4xl": "2.5rem",
    "--font-size-5xl": "3.5rem",
    "--font-weight-normal": "400",
    "--font-weight-medium": "500",
    "--font-weight-bold": "700",
    "--line-height-tight": "1.1",
    "--line-height-normal": "1.5",
    "--line-height-relaxed": "1.7"
  }
}
</flex_block>

<flex_block type="tokens">
{
  "category": "spacing",
  "tokens": {
    "--space-1": "0.25rem",
    "--space-2": "0.5rem",
    "--space-3": "0.75rem",
    "--space-4": "1rem",
    "--space-6": "1.5rem",
    "--space-8": "2rem",
    "--space-12": "3rem",
    "--space-16": "4rem",
    "--space-24": "6rem"
  }
}
</flex_block>

<flex_block type="tokens">
{
  "category": "radii",
  "tokens": {
    "--radius-sm": "0.25rem",
    "--radius-md": "0.5rem",
    "--radius-lg": "0.75rem",
    "--radius-xl": "1rem",
    "--radius-full": "9999px"
  }
}
</flex_block>

<flex_block type="tokens">
{
  "category": "shadows",
  "tokens": {
    "--shadow-sm": "0 2px 4px oklch(0% 0 0 / 0.1)",
    "--shadow-md": "0 4px 12px oklch(0% 0 0 / 0.15), 0 1px 3px oklch(0% 0 0 / 0.08)",
    "--shadow-lg": "0 12px 32px oklch(0% 0 0 / 0.2), 0 4px 8px oklch(0% 0 0 / 0.1)"
  }
}
</flex_block>

<flex_block type="tokens">
{
  "category": "transitions",
  "tokens": {
    "--transition-fast": "150ms ease-out",
    "--transition-base": "250ms ease-out",
    "--transition-slow": "400ms cubic-bezier(0.2, 0.8, 0.2, 1)",
    "--ease-spring": "cubic-bezier(0.34, 1.56, 0.64, 1)"
  }
}
</flex_block>

<flex_block type="mockup-html" id="landing-preview">
<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Archidex | The Field Guide to the Built World</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&family=JetBrains+Mono:wght@400;700&family=Space+Grotesk:wght@500;700&display=swap" rel="stylesheet">
<script src="https://unpkg.com/lucide@latest"></script>
<style>
  :root[data-theme="dark"] {
    --color-primary: oklch(75% 0.15 230);
    --color-primary-hover: oklch(80% 0.15 230);
    --color-primary-muted: oklch(75% 0.15 230 / 0.15);
    --color-accent: oklch(85% 0.18 90);
    --color-bg: oklch(18% 0.04 250);
    --color-surface: oklch(23% 0.04 250);
    --color-surface-raised: oklch(28% 0.03 250);
    --color-border: oklch(35% 0.03 250);
    --color-text: oklch(95% 0.01 250);
    --color-text-secondary: oklch(75% 0.02 250);
    --color-text-muted: oklch(60% 0.02 250);
    --color-text-on-primary: oklch(15% 0.04 250);
  }
  
  :root[data-theme="light"] {
    --color-primary: oklch(45% 0.12 250);
    --color-primary-hover: oklch(40% 0.12 250);
    --color-primary-muted: oklch(45% 0.12 250 / 0.12);
    --color-accent: oklch(55% 0.15 45);
    --color-bg: oklch(97% 0.01 85);
    --color-surface: oklch(99% 0.005 85);
    --color-surface-raised: oklch(100% 0 0);
    --color-border: oklch(85% 0.01 85);
    --color-text: oklch(25% 0.02 250);
    --color-text-secondary: oklch(45% 0.02 250);
    --color-text-muted: oklch(60% 0.02 250);
    --color-text-on-primary: oklch(98% 0 0);
  }

  :root {
    --font-display: 'Space Grotesk', system-ui, sans-serif;
    --font-body: 'Inter', system-ui, sans-serif;
    --font-mono: 'JetBrains Mono', monospace;
    --radius-sm: 0.25rem;
    --radius-md: 0.5rem;
    --radius-lg: 0.75rem;
    --radius-xl: 1rem;
    --transition-fast: 150ms ease-out;
    --transition-base: 250ms ease-out;
    --transition-slow: 400ms cubic-bezier(0.2, 0.8, 0.2, 1);
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }
  
  body {
    font-family: var(--font-body);
    background-color: var(--color-bg);
    color: var(--color-text);
    line-height: 1.5;
    transition: background-color var(--transition-base), color var(--transition-base);
    overflow-x: hidden;
    background-image: 
      linear-gradient(var(--color-border) 1px, transparent 1px),
      linear-gradient(90deg, var(--color-border) 1px, transparent 1px);
    background-size: 40px 40px;
    background-position: center top;
  }

  /* Typography */
  h1, h2, h3, .font-display { font-family: var(--font-display); font-weight: 700; line-height: 1.1; }
  .font-mono { font-family: var(--font-mono); }
  
  /* Layout */
  .container { max-width: 1200px; margin: 0 auto; padding: 0 2rem; }
  
  /* Navbar */
  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1.5rem 0;
    border-bottom: 1px solid var(--color-border);
    backdrop-filter: blur(10px);
    position: sticky;
    top: 0;
    z-index: 100;
  }
  .logo { font-family: var(--font-display); font-size: 1.5rem; font-weight: 700; display: flex; align-items: center; gap: 0.5rem; }
  .logo i { color: var(--color-primary); }
  
  .nav-actions { display: flex; gap: 1rem; align-items: center; }
  button {
    background: none; border: none; cursor: pointer;
    font-family: var(--font-body); font-weight: 500; font-size: 0.875rem;
    transition: all var(--transition-fast);
  }
  .btn-primary {
    background-color: var(--color-primary);
    color: var(--color-text-on-primary);
    padding: 0.75rem 1.5rem;
    border-radius: var(--radius-md);
  }
  .btn-primary:hover { background-color: var(--color-primary-hover); transform: translateY(-1px); }
  .btn-icon {
    width: 40px; height: 40px;
    border-radius: var(--radius-md);
    background-color: var(--color-surface);
    color: var(--color-text);
    display: flex; align-items: center; justify-content: center;
    border: 1px solid var(--color-border);
  }
  .btn-icon:hover { background-color: var(--color-surface-raised); }

  /* Hero Section */
  .hero {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 4rem;
    padding: 6rem 0;
    align-items: center;
    min-height: calc(100vh - 80px);
  }
  
  .hero-content h1 {
    font-size: clamp(3rem, 5vw, 4.5rem);
    margin-bottom: 1.5rem;
    letter-spacing: -0.02em;
  }
  .hero-content p {
    font-size: 1.25rem;
    color: var(--color-text-secondary);
    margin-bottom: 2.5rem;
    max-width: 480px;
  }
  
  .hero-badges {
    display: flex; gap: 1rem; margin-top: 3rem;
  }
  .badge {
    display: flex; align-items: center; gap: 0.5rem;
    padding: 0.5rem 1rem;
    background-color: var(--color-surface);
    border: 1px solid var(--color-border);
    border-radius: var(--radius-full);
    font-family: var(--font-mono); font-size: 0.75rem;
    color: var(--color-text-secondary);
  }

  /* Phone Mockup & Scanner Interactive */
  .phone-mockup {
    position: relative;
    width: 320px;
    height: 650px;
    background-color: #000;
    border-radius: 40px;
    border: 12px solid var(--color-surface-raised);
    box-shadow: 0 24px 48px rgba(0,0,0,0.4);
    margin: 0 auto;
    overflow: hidden;
    display: flex;
    flex-direction: column;
  }
  
  .phone-screen {
    position: relative;
    flex: 1;
    background-image: url('https://images.unsplash.com/photo-1552596954-c9233f2afbe8?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80');
    background-size: cover;
    background-position: center;
  }
  
  .camera-ui {
    position: absolute;
    inset: 0;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 2rem 1.5rem;
    z-index: 10;
  }
  
  .crosshairs {
    position: absolute;
    top: 50%; left: 50%;
    transform: translate(-50%, -50%);
    width: 200px; height: 200px;
    border: 1px solid rgba(255,255,255,0.3);
  }
  .crosshairs::before, .crosshairs::after {
    content: ''; position: absolute; background: white;
  }
  .crosshairs::before { top: 50%; left: -10px; right: -10px; height: 1px; }
  .crosshairs::after { left: 50%; top: -10px; bottom: -10px; width: 1px; }
  
  .scan-line {
    position: absolute;
    top: 0; left: 0; right: 0; height: 2px;
    background-color: var(--color-primary);
    box-shadow: 0 0 12px var(--color-primary);
    opacity: 0;
    transform: translateY(0);
  }
  
  .capture-btn-wrapper {
    display: flex; justify-content: center; margin-top: auto;
  }
  .capture-btn {
    width: 64px; height: 64px;
    border-radius: 50%;
    background-color: transparent;
    border: 4px solid white;
    position: relative;
  }
  .capture-btn::after {
    content: ''; position: absolute; inset: 4px;
    background-color: white; border-radius: 50%;
    transition: transform var(--transition-fast);
  }
  .capture-btn:hover::after { transform: scale(0.9); }
  .capture-btn:active::after { transform: scale(0.8); }

  /* Analysis Result Card */
  .result-card {
    position: absolute;
    bottom: 0; left: 0; right: 0;
    background-color: var(--color-surface);
    padding: 1.5rem;
    border-top-left-radius: var(--radius-xl);
    border-top-right-radius: var(--radius-xl);
    transform: translateY(100%);
    transition: transform var(--transition-slow);
    z-index: 20;
    border-top: 1px solid var(--color-border);
  }
  .result-card.active { transform: translateY(0); }
  
  .result-header { display: flex; justify-content: space-between; align-items: flex-start; margin-bottom: 1rem; }
  .result-style { font-family: var(--font-display); font-size: 1.5rem; font-weight: 700; color: var(--color-text); }
  .result-confidence { font-family: var(--font-mono); font-size: 0.75rem; color: var(--color-primary); background: var(--color-primary-muted); padding: 0.25rem 0.5rem; border-radius: var(--radius-sm); }
  .result-desc { font-size: 0.875rem; color: var(--color-text-secondary); margin-bottom: 1.5rem; }
  .result-cta { width: 100%; background: var(--color-text); color: var(--color-bg); padding: 0.75rem; border-radius: var(--radius-md); font-weight: 700; }

  /* Bounding Boxes */
  .bounding-box {
    position: absolute;
    border: 2px solid var(--color-primary);
    background: var(--color-primary-muted);
    opacity: 0;
    transition: opacity var(--transition-base);
    z-index: 15;
  }
  .box-1 { top: 20%; left: 30%; width: 40%; height: 25%; }
  .box-2 { top: 55%; left: 40%; width: 20%; height: 30%; }
  .bounding-box.active { opacity: 1; }
  .bounding-label {
    position: absolute; bottom: 100%; left: 0;
    background: var(--color-primary); color: var(--color-text-on-primary);
    font-family: var(--font-mono); font-size: 0.6rem;
    padding: 2px 6px; white-space: nowrap;
  }

  /* Animations */
  @keyframes scan {
    0% { transform: translateY(0); opacity: 1; }
    50% { transform: translateY(500px); opacity: 1; }
    100% { transform: translateY(0); opacity: 1; }
  }

  /* Field Guide Section */
  .field-guide { padding: 6rem 0; border-top: 1px solid var(--color-border); background: var(--color-surface); }
  .section-header { text-align: center; margin-bottom: 4rem; }
  .section-header h2 { font-size: 2.5rem; margin-bottom: 1rem; }
  .section-header p { color: var(--color-text-secondary); max-width: 600px; margin: 0 auto; }
  
  .grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
  }
  
  .style-card {
    background: var(--color-bg);
    border: 1px solid var(--color-border);
    border-radius: var(--radius-lg);
    overflow: hidden;
    transition: transform var(--transition-fast), border-color var(--transition-fast);
  }
  .style-card:hover { transform: translateY(-4px); border-color: var(--color-primary); }
  
  .style-img { height: 200px; background: var(--color-surface-raised); position: relative; }
  .style-img img { width: 100%; height: 100%; object-fit: cover; opacity: 0.8; mix-blend-mode: luminosity; }
  .style-card.locked .style-img img { opacity: 0.1; filter: blur(4px); }
  .style-card.locked .style-img::after {
    content: '?'; position: absolute; inset: 0; display: flex; align-items: center; justify-content: center;
    font-family: var(--font-display); font-size: 3rem; color: var(--color-text-muted);
  }
  
  .style-content { padding: 1.5rem; }
  .style-content h3 { font-size: 1.25rem; margin-bottom: 0.5rem; }
  .style-meta { display: flex; justify-content: space-between; font-family: var(--font-mono); font-size: 0.75rem; color: var(--color-text-muted); }

  @media (max-width: 768px) {
    .hero { grid-template-columns: 1fr; text-align: center; gap: 3rem; padding: 3rem 0; }
    .hero-content p { margin: 0 auto 2rem; }
    .hero-badges { justify-content: center; }
  }
</style>
</head>
<body>

  <div class="container">
    <nav>
      <div class="logo"><i data-lucide="scan-line"></i> Archidex</div>
      <div class="nav-actions">
        <button id="theme-toggle" class="btn-icon" aria-label="Toggle theme">
          <i data-lucide="sun"></i>
        </button>
        <button class="btn-primary">Get the App</button>
      </div>
    </nav>
  </div>

  <section class="hero container">
    <div class="hero-content">
      <h1>Read the streets.</h1>
      <p>Point your camera at any building to instantly identify its architectural style. Collect cities, learn the language of design, and see the world with new eyes.</p>
      
      <button class="btn-primary" style="font-size: 1.125rem; padding: 1rem 2rem;">Start Exploring</button>
      
      <div class="hero-badges">
        <div class="badge"><i data-lucide="camera" style="width:14px;height:14px;"></i> AI Scanner</div>
        <div class="badge"><i data-lucide="book" style="width:14px;height:14px;"></i> 80+ Styles</div>
        <div class="badge"><i data-lucide="map-pin" style="width:14px;height:14px;"></i> Global Map</div>
      </div>
    </div>
    
    <div class="phone-mockup">
      <div class="phone-screen">
        <div class="scan-line" id="scanLine"></div>
        
        <div class="bounding-box box-1" id="box1">
          <div class="bounding-label">Cresting</div>
        </div>
        <div class="bounding-box box-2" id="box2">
          <div class="bounding-label">Oriel Window</div>
        </div>

        <div class="camera-ui">
          <div style="display:flex; justify-content:space-between; color:white;">
            <i data-lucide="x"></i>
            <i data-lucide="zap"></i>
          </div>
          
          <div class="crosshairs" id="crosshairs"></div>
          
          <div class="capture-btn-wrapper">
            <button class="capture-btn" id="captureBtn" aria-label="Scan Building"></button>
          </div>
        </div>
        
        <div class="result-card" id="resultCard">
          <div class="result-header">
            <div class="result-style">Châteauesque</div>
            <div class="result-confidence">98% Match</div>
          </div>
          <p class="result-desc">Characterized by massive masonry, steep roofs with cresting, and elaborate dormers. Popularized in the late 19th century by Richard Morris Hunt.</p>
          <button class="result-cta" id="resetBtn">Add to Passport</button>
        </div>
      </div>
    </div>
  </section>

  <section class="field-guide">
    <div class="container">
      <div class="section-header">
        <h2>The Field Guide</h2>
        <p>Your personal collector's album. Discover the stories behind the facades and complete your architectural catalog.</p>
      </div>
      
      <div class="grid">
        <div class="style-card">
          <div class="style-img">
            <img src="https://images.unsplash.com/photo-1513694203232-719a280e022f?w=600&q=80" alt="Brutalist">
          </div>
          <div class="style-content">
            <h3>Brutalism</h3>
            <div class="style-meta"><span>1950s - 1970s</span><span>Collected</span></div>
          </div>
        </div>
        
        <div class="style-card">
          <div class="style-img">
            <img src="https://images.unsplash.com/photo-1541857754-557a24ed9217?w=600&q=80" alt="Art Deco">
          </div>
          <div class="style-content">
            <h3>Art Deco</h3>
            <div class="style-meta"><span>1920s - 1930s</span><span>Collected</span></div>
          </div>
        </div>
        
        <div class="style-card locked">
          <div class="style-img">
            <img src="https://images.unsplash.com/photo-1582582494705-f8ce0b0c24f0?w=600&q=80" alt="Gothic Revival">
          </div>
          <div class="style-content">
            <h3 style="color:var(--color-text-muted);">Gothic Revival</h3>
            <div class="style-meta"><span>1740s - 1800s</span><span>Undiscovered</span></div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <script>
    // Initialize Lucide icons
    lucide.createIcons();

    // Theme Toggle
    const themeToggle = document.getElementById('theme-toggle');
    const html = document.documentElement;
    
    themeToggle.addEventListener('click', () => {
      const currentTheme = html.getAttribute('data-theme');
      const newTheme = currentTheme === 'dark' ? 'light' : 'dark';
      html.setAttribute('data-theme', newTheme);
      
      // Update icon
      themeToggle.innerHTML = newTheme === 'dark' 
        ? '<i data-lucide="sun"></i>' 
        : '<i data-lucide="moon"></i>';
      lucide.createIcons();
    });

    // Scanner Interaction
    const captureBtn = document.getElementById('captureBtn');
    const scanLine = document.getElementById('scanLine');
    const crosshairs = document.getElementById('crosshairs');
    const resultCard = document.getElementById('resultCard');
    const resetBtn = document.getElementById('resetBtn');
    const boxes = document.querySelectorAll('.bounding-box');

    captureBtn.addEventListener('click', () => {
      // Hide crosshairs and button
      crosshairs.style.opacity = '0';
      captureBtn.style.opacity = '0';
      
      // Start scan
      scanLine.style.animation = 'scan 1.5s ease-in-out';
      
      // Show boxes during scan
      setTimeout(() => {
        boxes.forEach(box => box.classList.add('active'));
      }, 500);

      // Show result
      setTimeout(() => {
        scanLine.style.animation = 'none';
        scanLine.style.opacity = '0';
        resultCard.classList.add('active');
      }, 1500);
    });

    resetBtn.addEventListener('click', () => {
      resultCard.classList.remove('active');
      boxes.forEach(box => box.classList.remove('active'));
      setTimeout(() => {
        crosshairs.style.opacity = '1';
        captureBtn.style.opacity = '1';
      }, 300);
    });
  </script>
</body>
</html>
</flex_block>

---

## 7. Technical

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

## 8. Content

Archidex requires a robust, accurate canonical database at launch. The "Field Guide" needs to feel complete even before the user starts collecting.

<flex_block type="content-inventory">
{
  "have": [
    { "type": "concept", "source": "founder", "notes": "The Pokedex metaphor perfectly defines the collection mechanics and UI flow." }
  ],
  "need": [
    { "type": "data", "description": "A canonical list of 50-80 architectural styles with eras, descriptions, and defining features." },
    { "type": "data", "description": "A glossary of 150+ architectural terms (corbel, pediment, entablature, etc.)." },
    { "type": "assets", "description": "Vector illustrations for the glossary terms (blueprint/line-art style)." },
    { "type": "assets", "description": "Silhouette SVGs for the undiscovered styles in the Field Guide." },
    { "type": "copy", "description": "Marketing landing page copy focusing on discovery, learning, and collection." },
    { "type": "copy", "description": "Milestone logic and copy (e.g., 'Modernist Master', 'Gothic Ghost')." },
    { "type": "assets", "description": "Digital 'Stamps' (graphics) awarded for completing milestones." }
  ]
}
</flex_block>

The voice of the content is crucial. Architectural history can easily become dry and pedantic. Archidex content must be snappy, story-driven, and focused on visual identification. "Look for the massive, raw concrete and the sense of heavy, unapologetic weight" rather than "Brutalism emerged in the mid-20th century as a response to...".

---

## 9. Downstream Alerts

- **ALERT: AI Latency & UX** → The time between capturing a photo and receiving the AI response could be 2-4 seconds. The UI needs an engaging "scanning" animation to mask this latency so it feels like the app is "working hard" rather than "loading slowly."
- **ALERT: False Positives** → Buildings are often a mix of styles (e.g., a Victorian house renovated with modern windows). The AI prompt needs to handle ambiguity gracefully, perhaps returning a "Primary Style" and "Secondary Influences."
- **ALERT: Offline Capability** → Users will use this while traveling, often with poor data roaming. Captures should save locally with GPS data, and sync/analyze when back on WiFi, queuing up the "Style Unlocked" notifications for later.
- **ALERT: Content Accuracy** → We are relying on an LLM for factual architectural history. A human-in-the-loop validation process or a pre-vetted database of style descriptions should be used rather than generating the historical text dynamically on every scan. Only the *image analysis* should be dynamic.