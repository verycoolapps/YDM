# PRESENTATION AND DOCUMENT PROTECTION
## YOUR DEAD MEAT — Presentations & Professional Documents Protection Workflow

---

**Purpose:** Specialized protection workflow for Presentations & Professional Documents projects.  
**Scope:** All Presentations & Professional Documents projects processed through the YDM system.  
**Version:** 1.0.0  
**Dependencies:** `PRE_CREATION_GATE.md`, `ORIGINALITY_ENGINE.md`, `PROVENANCE_ENGINE.md`  

---

## DISCIPLINE OVERVIEW

Professional documents and presentations are protected as literary and artistic works. Original layouts, structured content, and visual design elements all receive copyright protection.

---

## SPECIALIZED PROTECTION CHECKLIST

```
PRESENTATION & DOCUMENT PROTECTION CHECKLIST
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

□ Source presentation file preserved (.pptx, .key, .pages)
□ Date and author in document properties
□ SHA-256 hash of final version recorded
□ Copyright notice in footer or on title slide
□ Cloud backup with verified timestamp
□ For client submissions: Dated delivery record (email)
□ Watermark on sensitive presentations shared for review

□ YDM provenance record established
```

### Document Metadata Template

```
Document Title:  [TITLE]
Author:         [CREATOR NAME]
Created:        [DATE]
YDM ID:         YDM-[ID]
Copyright:      © [YEAR] [NAME] — All Rights Reserved
```

---

## PROVENANCE RECORD FORMAT

For Presentations & Professional Documents projects, establish provenance using:

```yaml
# Presentations & Professional Documents PROVENANCE RECORD
# Project ID: YDM-[ID]

discipline_provenance:
  discipline: "Presentations & Professional Documents"
  primary_source_file: "[NATIVE FORMAT SOURCE FILE]"
  source_file_hash: "[SHA-256]"
  creation_tools: "[TOOLS AND VERSIONS USED]"
  creation_date: "[DATE — with evidence quality]"
  key_creative_decisions:
    - "[DECISION THAT IS DISTINCTIVE TO THIS WORK]"
```

---

*→ Back to entry: `../SKILL.md`*  
*→ Next industry module in sequence*
