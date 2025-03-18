---
type: guide
category: development
status: final
alias: "The Surgeon's Apprentice - File Naming & Frontmatter Style Guide"
date_created: 2024-01-25
date_modified: 2024-01-25
release_date: null
in_world_date: null
week: null
related_documents: [TSA_Dev_Guide_Week1Schedule, TSA_Dev_Theme_Week1Overview]
characters: []
locations: []
tags: [style-guide, documentation, organization, naming-conventions, frontmatter]
---
# THE SURGEON'S APPRENTICE
## File Naming & Frontmatter Style Guide

### FILENAME CONVENTION

#### Basic Pattern
`TSA_[Category]_[Type]_[Descriptor]_[Date]`

#### Category Codes
- `Pre` - Prelude content
- `Main` - Main narrative
- `Dev` - Development documents
- `Char` - Character documents
- `Loc` - Location documents

#### Type Codes
For Narrative Content:
- `W[1-8]` - Week number for prelude
- `Ch[001-999]` - Chapter number for main narrative
- `Letter` - Correspondence
- `Med` - Medical documents
- `Journal` - Journal entries
- `Report` - Reports and proposals

For Development:
- `Guide` - Development guides
- `Theme` - Thematic planning
- `Voice` - Voice/style guides
- `Profile` - Character profiles
- `Map` - Location details

#### Date Format (when applicable)
- In-world dates: `YYYYMMDD`
- Modern dates: omit if not needed

#### Examples
```markdown
TSA_Pre_W1_GideonDiary_17550412
TSA_Dev_Guide_Week1Schedule
TSA_Char_Profile_GideonAldrich
TSA_Pre_W1_LetterToDuke_17550414
```

### FRONTMATTER TEMPLATE

#### Required Fields
```yaml
---
type: [document/guide/profile/map]
category: [prelude/main/development]
status: [draft/review/final]
alias: "Human-readable title"
date_created: YYYY-MM-DD
date_modified: YYYY-MM-DD
---
```

#### Optional Fields (Use When Applicable)
```yaml
---
release_date: YYYY-MM-DD
in_world_date: YYYY-MM-DD
week: [1-8]
related_documents: []
characters: []
locations: []
tags: []
---
```

### TYPE DEFINITIONS

#### Document Types
- `document` - Narrative content
- `guide` - Development guides
- `profile` - Character profiles
- `map` - Location documents

#### Categories
- `prelude` - Prelude narrative (1755-1760)
- `main` - Main narrative
- `development` - Development documents

#### Status Levels
- `draft` - Initial creation
- `review` - Ready for review
- `final` - Approved for use

### ALIAS CONVENTIONS

#### Narrative Documents
Pattern: `[Document Type] - [Date]`
Example: "Gideon's Diary Entry - April 12, 1755"

#### Letters
Pattern: `Letter [to/from] [Person] - [Date]`
Example: "Letter to Duke Malcolm - April 14, 1755"

#### Development Documents
Pattern: `[Week #] [Document Type] - [Theme]`
Example: "Week 1 Content Release Guide - Seeds of Transformation"

### TAG CONVENTIONS
- Use lowercase
- Hyphenate multi-word tags
- Be specific but concise
- Use established tag categories

### IMPLEMENTATION NOTES

#### File Organization
1. Always place files in appropriate folders:
   - /prelude
   - /main-narrative
   - /development
   - /characters
   - /locations

#### Related Documents
1. Always use full filenames in related_documents
2. Maintain bi-directional links
3. Check links when files are renamed

#### Dates
1. Modern dates: Use ISO format (YYYY-MM-DD)
2. In-world dates: Use period-appropriate format in alias
3. Use numerical format in filename (YYYYMMDD)

#### Version Control
1. Update date_modified when changes are made
2. Track status changes
3. Maintain change log if needed

### EXAMPLE SET

```yaml
---
type: document
category: prelude
status: final
alias: "Gideon's Diary Entry - April 12, 1755"
date_created: 2024-01-25
date_modified: 2024-01-25
release_date: 2024-01-19
in_world_date: 1755-04-12
week: 1
related_documents: [TSA_Pre_W1_MedicalNotes_17550412]
characters: [Gideon Aldrich, Harrison, Duke Malcolm]
locations: [Ravenwood Castle, Surgery Theater]
tags: [diary, catalyst, pain-management, transformation-theory]
---
```

### QUALITY CONTROL

#### Regular Checks
1. Filename compliance
2. Frontmatter completeness
3. Link validity
4. Tag consistency
5. Date accuracy

#### Common Issues
1. Inconsistent date formats
2. Missing required fields
3. Broken document links
4. Inconsistent tag usage
5. Incorrect categorization

#### Maintenance Tasks
1. Update modified dates
2. Check related documents
3. Verify tag usage
4. Validate links
5. Review status levels