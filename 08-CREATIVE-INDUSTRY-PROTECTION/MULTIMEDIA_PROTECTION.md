# MULTIMEDIA PROTECTION
## YOUR DEAD MEAT — Audio, Video & Multimedia Protection Workflow

---

**Purpose:** Specialized protection workflow for Audio, Video & Multimedia projects.  
**Scope:** All Audio, Video & Multimedia projects processed through the YDM system.  
**Version:** 1.0.0  
**Dependencies:** `PRE_CREATION_GATE.md`, `ORIGINALITY_ENGINE.md`, `PROVENANCE_ENGINE.md`  

---

## DISCIPLINE OVERVIEW

Multimedia works combine multiple IP-protected elements: music (copyright), video (copyright), performances (may carry separate rights), and brand elements (trademark). Each element may have separate rights.

---

## SPECIALIZED PROTECTION CHECKLIST

```
MULTIMEDIA PROTECTION CHECKLIST
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

VIDEO
□ Source project files preserved (.prproj, .aep, .fcpx)
□ Rendered master file hash recorded
□ Director, producer, and creator credits documented
□ Clearances for all music and third-party elements documented

AUDIO / MUSIC
□ DAW project files preserved
□ Master audio file hash recorded
□ Songwriter, composer, and producer credits documented
□ For musicians: Sound recording vs. composition rights distinguished
□ PRO (Performing Rights Organization) registration for music
□ Copyright notice embedded in file metadata

GENERAL MULTIMEDIA
□ All contributors documented with their specific contributions
□ License status of all third-party elements verified
□ Attribution requirements for licensed elements met

□ YDM provenance record established for each media type
```

---

## PROVENANCE RECORD FORMAT

For Audio, Video & Multimedia projects, establish provenance using:

```yaml
# Audio, Video & Multimedia PROVENANCE RECORD
# Project ID: YDM-[ID]

discipline_provenance:
  discipline: "Audio, Video & Multimedia"
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
