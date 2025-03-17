---
aliases:
tags:
---
**Master Lorebook Template**
```
---
aliases: Master Lorebook
tags: lorebook
created: [current date]
last_updated: [current date]
version: 001.001
---

# [YOUR WORLD] MASTER LOREBOOK

## WORLD CONFIGURATION
- **Setting:** [Where and when your world is set]
- **Current Year/Era:** [Timeline information]
- **Genre:** [Type of setting - fantasy, sci-fi, etc.]
- **Logline:** [One-line description of your world's core concept]

### Core Themes
- [Theme 1]
- [Theme 2]
- [Theme 3]

### World Concepts
- [Major Concept 1]
- [Major Concept 2]
- [Major Concept 3]

## CHARACTERS
### Main Characters
- **[Character Name]** - [Brief description]
- **[Character Name]** - [Brief description]

### Supporting Characters
- **[Character Name]** - [Brief description]
- **[Character Name]** - [Brief description]

## LOCATIONS
### [Main Region/Area]
- **[Location Name]** - [Brief description]
- **[Location Name]** - [Brief description]

### [Secondary Region/Area]
- **[Location Name]** - [Brief description]
- **[Location Name]** - [Brief description]

## ITEMS
### Key Items
- **[Item Name]** - [Brief description]
- **[Item Name]** - [Brief description]

## LORE
### Historical
- **[Historical Event/Element]** - [Brief description]
- **[Historical Event/Element]** - [Brief description]

### [Other Lore Category]
- **[Lore Element]** - [Brief description]
- **[Lore Element]** - [Brief description]
```

**RAG World Overview Template:**
```
---
id: world_overview
type: setting
name: [World Name] Overview
category: world_configuration
tags: [setting, overview, time_period, location, genre]
related_concepts: [concept1, concept2, concept3]
related_themes: [theme1, theme2, theme3]
version: 001.001
---

# [Setting Name] Overview

**Setting:** [Geographic location and specific environment]  
**Current Year/Era:** [Time period]  
**Genre:** [Primary and secondary genres]

## Core Narrative
[One to two sentences that capture the central conflict, premise, or narrative hook of the setting]

## Core Themes
- **[Theme 1]**: [Brief explanation]
- **[Theme 2]**: [Brief explanation]
- **[Theme 3]**: [Brief explanation]

## World Concepts
### [Major Concept 1]
[Paragraph explaining this foundational concept]

### [Major Concept 2]
[Paragraph explaining this foundational concept]

## Physical Structure
[Setting Name] is divided into [number] main areas:
1. **[Area 1]** - [Brief description]
2. **[Area 2]** - [Brief description]
```

**RAG Character Template:**
```
---
id: char_[unique_id]
type: character
name: [Character Name]
category: [main_character/supporting_character]
tags: [tag1, tag2, tag3]
locations: [Primary Location, Secondary Location]
key_items: [Associated Item 1, Associated Item 2]
related_characters: [Related Character 1, Related Character 2]
version: 001.001
---

# [Character Name]

Brief one-sentence description that captures the character's essential nature and role.

## Appearance & Role
Two to three sentences describing physical appearance, role in the world, and any immediately notable traits.

## Location & Activities
Where the character is typically found and what activities they regularly engage in.

## Key Relationships
- **[Related Character 1]**: Brief description of relationship
- **[Related Character 2]**: Brief description of relationship

## Character Traits
Description of personality, motivations, and notable behavioral patterns.

## Background/History
Brief relevant history or background information.

## Narrative Significance
Character's role in the broader narrative.
```

**RAG Location Template:**
```
---
id: loc_[unique_id]
type: location
name: [Location Name]
category: [category]
tags: [tag1, tag2, tag3]
connected_locations: [Connected Location 1, Connected Location 2]
key_characters: [Character 1, Character 2]
key_items: [Item 1, Item 2]
version: 001.001
---

# [Location Name]

Brief one or two sentence description establishing what this location is and its primary function.

## Physical Description
Detailed description of the location's appearance, atmosphere, and sensory details.

## Notable Sub-locations
### [Sub-location 1]
Brief description of this specific area.

### [Sub-location 2]
Brief description of this specific area.

## Regular Occupants
- **[Character 1]**: Brief note about their connection to this location
- **[Character 2]**: Brief note about their connection to this location

## Activities & Functions
Description of what typically happens in this location.

## Historical/Supernatural Significance
Any historical background or special elements connected to this location.
```

**RAG Item Template:**
```
---
id: item_[unique_id]
type: item
name: [Item Name]
category: [category]
tags: [tag1, tag2, tag3]
locations: [Location 1, Location 2]
related_characters: [Character 1, Character 2]
version: 001.001
---

# [Item Name]

Brief one or two sentence description establishing what this item is and its significance.

## Physical Description
Detailed description of the item's appearance and distinctive features.

## Properties & Functions
Description of what the item does and how it works.

## Historical Significance
Background information on when and how the item was created or discovered.

## Current Status & Location
Where the item is currently kept and its condition.

## Associated Characters
- **[Character 1]**: Their specific connection to the item
- **[Character 2]**: Their specific connection to the item
```

**RAG Lore Template:**
```
---
id: lore_[unique_id]
type: lore
name: [Lore Element Name]
category: [category]
tags: [tag1, tag2, tag3]
related_characters: [Character 1, Character 2]
related_locations: [Location 1, Location 2]
version: 001.001
---

# [Lore Element Name]

Introduction paragraph establishing what this lore element encompasses and its significance.

## [Subsection 1]
Detailed information about this aspect of the lore element.

## [Subsection 2]
Additional area of knowledge related to the main lore element.

## Practical Implications
How this lore element affects daily life or activities in your world.

## Connections to Other Knowledge
How this lore element connects to other areas of knowledge.
```
