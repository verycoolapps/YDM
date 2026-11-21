# OUTPUT FORMAT STANDARDS
## YOUR DEAD MEAT — Execution & Documentation Module

---

**Purpose:** Defines professional output formatting standards for all YDM documents.
**Version:** 1.0.0  
**Dependencies:** All modules.  

---

## OUTPUT FORMAT STANDARDS

### Document Header Standard
```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
[DOCUMENT TYPE] — YOUR DEAD MEAT
Reference: YDM-[TYPE]-[ID]
Date: [ISO 8601]
Creator: [NAME]
Project: [PROJECT NAME] | YDM-[ID]
Status: [DRAFT | FINAL | FOR LEGAL REVIEW]
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Status Indicators
```
🟢 Protected / Complete / Verified
🟡 Partial / In Progress / Needs Action
🔴 Critical / Missing / Immediate Action Required
⚪ Informational / Pending / Reference
```

### Evidence Citation Format
```
[EVIDENCE TYPE], [DATE], [SOURCE/LOCATION]:
"[SPECIFIC EVIDENCE DESCRIPTION]"
Strength: [Strong | Moderate | Weak]
Hash: [SHA-256 — first 16 chars...] (if file evidence)
```

### YAML Record Standards
- All dates: ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
- All hashes: SHA-256, 64-character hex string
- All IDs: YDM-[8-char uppercase hex]
- Status labels: Consistent with established vocabulary
- Declarations: Always labeled [USER-DECLARED] or [VERIFIED: source]

### Markdown Document Standards
- Section dividers: `━━━` (80 chars) for major sections
- Subsection dividers: `---` for minor breaks
- Tables: Aligned pipe format
- Code blocks: Triple backtick with language hint
- Status emoji: Only in designated status fields

---
