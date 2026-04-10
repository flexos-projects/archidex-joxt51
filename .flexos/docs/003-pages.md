---
id: doc-pages
title: Archidex — Pages
type: doc
subtype: pages
status: published
sequence: 3
createdAt: "2026-04-10T21:02:21.436Z"
updatedAt: "2026-04-10T21:02:21.436Z"
---

# Pages

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

<flex_block type="page-inventory" id="blk-001" name="Page Inventory">
{
  "pages": [
    {
      "route": "/",
      "name": "Landing Page",
      "type": "marketing",
      "description": "Web-only. App showcase, interactive scanner demo, download CTAs."
    },
    {
      "route": "/lens",
      "name": "The Lens (Camera)",
      "type": "app",
      "description": "The default view. Live camera feed, drafting crosshairs, capture button."
    },
    {
      "route": "/capture/:id",
      "name": "Capture Result",
      "type": "app",
      "description": "Post-scan analysis. Annotated photo, style classification, add-to-collection CTA."
    },
    {
      "route": "/guide",
      "name": "Field Guide",
      "type": "app",
      "description": "Grid of all architectural styles. Discovered vs. undiscovered silhouettes."
    },
    {
      "route": "/guide/style/:id",
      "name": "Style Detail",
      "type": "app",
      "description": "History, defining features, and your personal gallery for a specific style."
    },
    {
      "route": "/map",
      "name": "Architecture Radar",
      "type": "app",
      "description": "Map view of your captures and nearby uncollected landmarks."
    },
    {
      "route": "/passport",
      "name": "Passport (Profile)",
      "type": "app",
      "description": "Your stats, digital stamps, and journey across cities."
    },
    {
      "route": "/glossary",
      "name": "Glossary",
      "type": "app",
      "description": "Searchable visual dictionary of architectural terms and elements."
    },
    {
      "route": "/login",
      "name": "Auth",
      "type": "auth",
      "description": "Simple social login to save your collection across devices."
    }
  ]
}
</flex_block>
