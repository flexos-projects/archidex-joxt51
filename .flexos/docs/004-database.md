---
id: doc-database
title: "Database & Data Model"
type: doc
status: active
createdAt: "2026-04-10"
relatesTo: ["docs/003-pages.md"]
---

# 4. Database & Data Model

The data architecture for Archidex is designed to support a rich, content-heavy application with a significant gamification layer. The model separates user-generated content (Captures) from the canonical, encyclopedic content (Styles, Elements).

## Core Collections

### Users
Represents the individual explorers. This collection stores their profile information and tracks high-level progress to populate the Passport page.
- **Key Fields:** `username`, `avatar`, `homeCity`, `totalCaptures`, `joinedAt`
- **Relationships:** A User has many Captures and many unlocked Milestones.

### Captures
This is the central, user-generated entity. Every time a user scans a building, a Capture record is created. It's the "instance" of a discovery.
- **Key Fields:** `photoUrl`, `location (lat/lng)`, `confidenceScore`, `annotations (JSON)`, `capturedAt`
- **Relationships:** A Capture belongs to one User and is classified as one Style.
- **Notes:** The `annotations` field stores the bounding box data from the AI, allowing the Annotated Breakdown to be rendered on the `/capture/:id` page without re-running the analysis.

### Styles
The canonical, admin-managed database of architectural movements. This collection populates the Field Guide. It is read-only for users.
- **Key Fields:** `name`, `eraStart`, `eraEnd`, `description`, `silhouetteImage`, `keyFeatures`
- **Relationships:** A Style can be linked to many Captures from many different users. It is composed of many Elements.
- **Notes:** This data is foundational and must be well-researched and populated at launch.

### Elements
The vocabulary of architecture. These are the specific, identifiable features that make up a Style (e.g., "Gargoyle," "Pilaster"). This collection powers the Glossary.
- **Key Fields:** `name`, `definition`, `vectorIllustrationUrl`, `category`
- **Relationships:** An Element can be a defining feature of many Styles.

### Milestones
The gamification engine. These are the achievements that users can unlock by performing specific collection actions. Unlocking a Milestone grants a digital Stamp to the user's Passport.
- **Key Fields:** `title`, `description`, `stampImageUrl`, `requirementLogic`, `rarity`
- **Relationships:** A Milestone can be unlocked by many Users.
- **Notes:** The `requirementLogic` will be a server-side function that evaluates a user's collection against criteria (e.g., `user.captures.where(style.name == 'Brutalist').count >= 5`).

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
