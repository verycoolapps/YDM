# DOCUMENT COPY DETECTION
## YOUR DEAD MEAT — DOCUMENT COPY DETECTION Module

---

**Purpose:** Detects textual and document-level similarities.  
**Scope:** Specialized detection for this asset type.  
**Version:** 1.0.0  
**Dependencies:** `PLAGIARISM_DETECTION_ENGINE.md`, `SIMILARITY_ANALYSIS.md`, `FALSE_POSITIVE_PROTECTION.md`  

---

## DOCUMENT AND TEXT SIMILARITY DETECTION

### Text Copy Indicators

| Indicator | Strength | Note |
|-----------|---------|------|
| Verbatim reproduction of unique passages | Very Strong | Strong case |
| Near-verbatim with synonyms substituted | Strong | Likely copy |
| Paraphrase preserving unique structure | Moderate | Investigate |
| Same unique factual errors | Strong | Errors don't copy themselves |
| Same invented terminology | Strong | Invented terms are distinctive |
| Same general argument structure | Weak | Could be independent |
| Same subject matter | None | Not copying |

### Text Comparison Tools

```
FREE TOOLS FOR TEXT SIMILARITY
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Copyscape: copyscape.com — web content similarity
iThenticate: used by academic publishers (subscription)
Grammarly: grammarly.com/plagiarism-checker (basic)
DupliChecker: duplichecker.com (free)
Quetext: quetext.com (free tier)

For manual comparison:
  - Paste unique phrases in quotes in Google
  - Search for invented terminology
  - Search for distinctive structural phrases
```

### Text Comparison Record

```yaml
text_comparison:
  original_distinctive_passages:
    - passage: "[UNIQUE PHRASE OR PASSAGE]"
      location: "[CHAPTER/SECTION/PAGE IN ORIGINAL]"
      uniqueness_basis: "[WHY THIS IS DISTINCTIVE]"
      
  suspected_copy_matches:
    - match_type: "Verbatim | Near-verbatim | Paraphrase"
      original_passage: "[ORIGINAL TEXT]"
      suspected_text: "[SUSPECTED COPY TEXT]"
      location_in_suspected: "[WHERE FOUND]"
```

---
