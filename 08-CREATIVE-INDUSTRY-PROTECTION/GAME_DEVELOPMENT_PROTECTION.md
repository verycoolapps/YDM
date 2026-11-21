# GAME DEVELOPMENT PROTECTION
## YOUR DEAD MEAT — Game Development Protection Workflow

---

**Purpose:** Specialized protection workflow for Game Development projects.  
**Scope:** All Game Development projects processed through the YDM system.  
**Version:** 1.0.0  
**Dependencies:** `PRE_CREATION_GATE.md`, `ORIGINALITY_ENGINE.md`, `PROVENANCE_ENGINE.md`  

---

## DISCIPLINE OVERVIEW

Game projects involve multiple overlapping IP types: code (copyright), art assets (copyright), music (copyright), brand elements (trademark), and potentially novel mechanics (patent, in some jurisdictions).

---

## SPECIALIZED PROTECTION CHECKLIST

```
GAME DEVELOPMENT PROTECTION CHECKLIST
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

CODE
□ Repository with full commit history
□ License in repository root

ART ASSETS
□ All original assets dated and hashed
□ Style guide documented showing unique visual language
□ Source files preserved (PSD, AI, etc.)
□ Third-party asset licenses verified

AUDIO
□ Original music/sound effects documented
□ Licensed audio clearly identified
□ Composer credits documented

NARRATIVE
□ Original script/story documented
□ Character concepts documented (written + visual)
□ World-building documents dated

BRAND
□ Game title trademark search recommended
□ Logo protection via copyright (auto) + trademark (register)

□ YDM provenance record established for each major asset category
```

---

## PROVENANCE RECORD FORMAT

For Game Development projects, establish provenance using:

```yaml
# Game Development PROVENANCE RECORD
# Project ID: YDM-[ID]

discipline_provenance:
  discipline: "Game Development"
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
