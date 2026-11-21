# ATTRIBUTION ENGINE
## YOUR DEAD MEAT — Standardized Creator Attribution Generation

---

**Purpose:** Generates standardized, context-appropriate creator attribution for all project types and output formats.  
**Scope:** All projects and deliverables requiring attribution text.  
**Version:** 1.0.0  
**Dependencies:** `CREATOR_IDENTITY_ENGINE.md`, `IDENTITY_CONSISTENCY.md`  

---

## ATTRIBUTION PRINCIPLES

1. Attribution should be **accurate** — reflecting who actually made what.
2. Attribution should be **specific** — identifying the work and creator precisely.
3. Attribution should be **consistent** — using the same format across all versions.
4. Attribution should be **prominent** — not buried where it won't be seen.
5. Attribution should be **honest** — acknowledging third-party sources and AI assistance.

---

## ATTRIBUTION FORMAT LIBRARY

### Format A — Full Legal Attribution
*Use for: formal documents, legal notices, official publications*
```
Copyright © [YEAR] [LEGAL NAME]. All rights reserved.
YDM Project: [PROJECT NAME] | ID: [YDM-XXXXXXXX]
Created: [DATE] | Version: [VERSION]
```

### Format B — Professional Attribution
*Use for: portfolio pieces, commercial releases, professional communications*
```
© [YEAR] [PROFESSIONAL NAME/STUDIO]
[PROJECT TITLE] — Original creation by [CREATOR]
YDM-[ID]
```

### Format C — Collaboration Attribution
*Use for: co-created works*
```
© [YEAR] [CREATOR A] & [CREATOR B]
Concept & Direction: [CREATOR A]
[SPECIFIC ELEMENT]: [CREATOR B]
YDM-[ID]
```

### Format D — Work-for-Hire Attribution
*Use for: commissioned or employment work*
```
© [YEAR] [ORGANIZATION NAME]
Created by [CREATOR NAME] for [ORGANIZATION]
YDM-[ID]
```

### Format E — Minimal Attribution
*Use for: space-constrained contexts (icons, small UI elements)*
```
© [YEAR] [NAME] | YDM-[ID]
```

### Format F — Open Creative Commons Attribution
*Use for: works released under Creative Commons license*
```
[WORK TITLE] © [YEAR] [NAME]
Licensed under [CC LICENSE TYPE]
YDM-[ID]
```

### Format G — AI-Assisted Attribution
*Use for: works with significant AI contribution*
```
© [YEAR] [CREATOR NAME]
Human-directed creation using AI assistance ([MODEL NAME])
Original concept, direction, and selection by [CREATOR NAME]
YDM-[ID]
```

---

## ATTRIBUTION GENERATION WORKFLOW

```
INPUT:
  - Creator name from CIR
  - Owner from Ownership Record
  - Project name from PCR
  - Year from creation timestamp
  - Project ID from registration
  - Any collaboration or AI factors
  
PROCESS:
  1. Determine context (formal/professional/minimal/collaborative/etc.)
  2. Select appropriate format
  3. Populate template with verified data
  4. Apply consistency check against existing attribution records
  5. Flag any [USER-DECLARED] fields
  
OUTPUT:
  - Attribution string in selected format
  - Attribution metadata block for embedding
  - Attribution for file properties
```

---

## ATTRIBUTION METADATA BLOCK

For embedding in file metadata (EXIF, XMP, ID3, etc.):

```
Creator:     [NAME]
Rights:      © [YEAR] [OWNER] — All Rights Reserved
Description: [PROJECT TITLE] — [BRIEF DESCRIPTION]
Identifier:  YDM-[ID]
Date:        [ISO 8601]
Software:    YOUR DEAD MEAT IP Defense System v1.0.0
```

---

*→ Next: `OWNERSHIP_DISPUTE_PROTOCOL.md`*  
*→ Back: `IDENTITY_CONSISTENCY.md`*
