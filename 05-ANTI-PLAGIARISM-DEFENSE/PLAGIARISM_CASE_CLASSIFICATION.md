# PLAGIARISM CASE CLASSIFICATION
## YOUR DEAD MEAT — PLAGIARISM CASE CLASSIFICATION Module

---

**Purpose:** Classifies suspected incidents by evidence quality and severity.  
**Scope:** Specialized detection for this asset type.  
**Version:** 1.0.0  
**Dependencies:** `PLAGIARISM_DETECTION_ENGINE.md`, `SIMILARITY_ANALYSIS.md`, `FALSE_POSITIVE_PROTECTION.md`  

---

## CASE CLASSIFICATION SYSTEM

Every suspected plagiarism case is classified by evidence quality and severity to guide appropriate response.

### Classification Matrix

```
SEVERITY × EVIDENCE QUALITY = CLASSIFICATION

                │ Strong Evidence │ Moderate Evidence │ Weak Evidence
────────────────┼─────────────────┼───────────────────┼──────────────
High Impact     │  CRITICAL       │  ELEVATED         │  WATCHLIST
(Commercial     │  Immediate      │  Formal inquiry   │  Document
 harm, wide     │  legal action   │  recommended      │  for now
 distribution)  │  recommended    │                   │
────────────────┼─────────────────┼───────────────────┼──────────────
Moderate Impact │  ACTIVE         │  STANDARD         │  MONITOR
(Ongoing use,   │  Formal notice  │  Initial notice   │  Gather more
 some harm)     │  appropriate    │  appropriate      │  evidence
────────────────┼─────────────────┼───────────────────┼──────────────
Low Impact      │  DOCUMENTED     │  NOTED            │  ARCHIVE
(Minor use,     │  Document &     │  Note & monitor   │  File; no
 limited harm)  │  monitor        │                   │  action now
```

### Case Record

```yaml
# PLAGIARISM CASE RECORD
# Case ID: YDM-CASE-[AUTO: YYYY-XXXX]

case_record:
  case_id: "YDM-CASE-[ID]"
  opened_date: "[ISO 8601]"
  
  original_work:
    project_id: "YDM-[ID]"
    work_description: "[BRIEF DESCRIPTION]"
    
  suspected_incident:
    description: "[WHAT WAS FOUND]"
    location: "[PUBLIC URL OR LOCATION]"
    discovery_date: "[DATE]"
    
  classification:
    severity: "Critical | Elevated | Active | Standard | Documented | Watchlist | Monitor | Noted | Archive"
    evidence_quality: "Strong | Moderate | Weak | Insufficient"
    
  recommended_next_action: "[SPECIFIC NEXT STEP]"
  case_status: "Open | Under Investigation | Response Sent | Resolved | Archived"
```

---
