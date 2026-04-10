---
id: doc-database
title: Archidex — Database
type: doc
subtype: database
status: published
sequence: 4
createdAt: "2026-04-10T21:02:21.436Z"
updatedAt: "2026-04-10T21:02:21.436Z"
---

# Database

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

<flex_block type="data-model" id="blk-001" name="Data Model">
{
  "collections": [
    {
      "name": "Users",
      "icon": "lucide:user",
      "description": "The explorers. Tracks their overall progress, home city, and settings.",
      "keyFields": [
        "username",
        "avatar",
        "homeCity",
        "totalCaptures",
        "joinedAt"
      ],
      "relationships": [
        "captures → Captures",
        "unlockedMilestones → Milestones"
      ]
    },
    {
      "name": "Captures",
      "icon": "lucide:camera",
      "description": "An instance of a user scanning a building. The core user-generated entity.",
      "keyFields": [
        "photoUrl",
        "location (lat/lng)",
        "confidenceScore",
        "annotations (JSON)",
        "capturedAt"
      ],
      "relationships": [
        "user → Users",
        "style → Styles"
      ]
    },
    {
      "name": "Styles",
      "icon": "lucide:landmark",
      "description": "The canonical database of architectural movements (e.g., Art Deco, Gothic).",
      "keyFields": [
        "name",
        "eraStart",
        "eraEnd",
        "description",
        "silhouetteImage",
        "keyFeatures"
      ],
      "relationships": [
        "elements → Elements",
        "captures → Captures"
      ]
    },
    {
      "name": "Elements",
      "icon": "lucide:puzzle",
      "description": "The structural building blocks and vocabulary (e.g., Gargoyle, Pilaster).",
      "keyFields": [
        "name",
        "definition",
        "vectorIllustrationUrl",
        "category"
      ],
      "relationships": [
        "styles → Styles"
      ]
    },
    {
      "name": "Milestones",
      "icon": "lucide:award",
      "description": "Achievements users can unlock based on their collection patterns.",
      "keyFields": [
        "title",
        "description",
        "stampImageUrl",
        "requirementLogic",
        "rarity"
      ],
      "relationships": [
        "users → Users"
      ]
    }
  ]
}
</flex_block>
