# DIGITAL ART PROTECTION
## YOUR DEAD MEAT — Digital Art & Illustration Protection Workflow

---

**Purpose:** Specialized protection workflow for Digital Art & Illustration projects.  
**Scope:** All Digital Art & Illustration projects processed through the YDM system.  
**Version:** 1.0.0  
**Dependencies:** `PRE_CREATION_GATE.md`, `ORIGINALITY_ENGINE.md`, `PROVENANCE_ENGINE.md`  

---

## DISCIPLINE OVERVIEW

Digital art and illustration are protected by copyright as artistic works from the moment of creation. The original creative expression is what's protected, not the subject matter or medium.

---

## SPECIALIZED PROTECTION CHECKLIST

```
DIGITAL ART PROTECTION CHECKLIST
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

□ Source files (.psd, .ai, .krita, etc.) preserved and dated
□ Layer structure preserved (reveals creative process)
□ SHA-256 hash of source file recorded
□ Attribution embedded in file metadata (EXIF/IPTC/XMP)
□ Work-in-progress screenshots saved with timestamps
□ Style reference sheet (moodboard) preserved separately
□ Uploaded to cloud storage with verified timestamp
□ For commercial work: Register with copyright authority
□ Watermark strategy for public sharing
□ Portfolio post with date stamps the work publicly

□ Creative fingerprint documented (see CREATIVE_FINGERPRINTING.md)
```

### Watermarking Recommendations

| Situation | Watermark Approach |
|-----------|-------------------|
| Portfolio display | Visible transparent overlay with name and YDM ID |
| Client preview | "PREVIEW — [NAME] — YDM-[ID]" prominent watermark |
| Released work | Embedded attribution in metadata |
| High-value pieces | Steganographic watermark (invisible but detectable) |

---

## PROVENANCE RECORD FORMAT

For Digital Art & Illustration projects, establish provenance using:

```yaml
# Digital Art & Illustration PROVENANCE RECORD
# Project ID: YDM-[ID]

discipline_provenance:
  discipline: "Digital Art & Illustration"
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
