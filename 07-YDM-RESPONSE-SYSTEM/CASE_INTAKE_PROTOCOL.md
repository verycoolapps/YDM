# CASE INTAKE PROTOCOL
## YOUR DEAD MEAT — Incident Information & Evidence Collection

---

**Purpose:** Collects and organizes incident information and initial evidence at case opening.  
**Scope:** All new incident investigations.  
**Version:** 1.0.0  
**Dependencies:** `INCIDENT_RESPONSE_ENGINE.md`, `EVIDENCE_VAULT.md`  

---

## INTAKE DIALOGUE

```
YDM CASE INTAKE
━━━━━━━━━━━━━━━

Before we begin the formal case record, I need to gather
information about the original work and the suspected incident.

ABOUT YOUR ORIGINAL WORK:
1. What is the name of your original project/work?
2. When did you create it? (approximate date is fine)
3. Do you have a YDM project ID for it, or will we create one now?
4. What is the most distinctive/original element of your work?
5. What evidence of your original creation do you have?
   (Files with dates, commits, emails, cloud storage, etc.)

ABOUT THE SUSPECTED INCIDENT:
6. What did you find, and where?
7. When did you discover it?
8. What URL or location is the suspected copy at?
9. Which specific elements appear to have been copied?
10. When was the suspected copy first published (if known)?
```

---

## INTAKE RECORD TEMPLATE

```yaml
# CASE INTAKE RECORD
# Case ID: YDM-CASE-[AUTO]
# Intake Date: [ISO 8601]

case_intake:
  
  original_work:
    name: "[WORK NAME]"
    ydm_project_id: "YDM-[ID] | [TO BE ASSIGNED]"
    creation_date_claimed: "[DATE — USER-DECLARED]"
    creation_date_evidence:
      - type: "[GIT COMMIT | FILE DATE | CLOUD UPLOAD | EMAIL | OTHER]"
        date: "[DATE FROM THIS SOURCE]"
        location: "[WHERE EVIDENCE IS]"
    distinctive_elements:
      - "[ELEMENT 1 — BE SPECIFIC]"
      - "[ELEMENT 2]"
      
  incident_details:
    discovery_date: "[DATE]"
    suspected_copy_url: "[URL]"
    platform: "[WEBSITE/APP/SERVICE]"
    suspected_creator: "[IF PUBLICLY KNOWN — only public information]"
    elements_apparently_copied:
      - "[ELEMENT THAT APPEARS IN BOTH WORKS]"
    suspected_publication_date: "[DATE — if determinable]"
    
  initial_evidence_captured:
    - "[SCREENSHOT STORED AT: LOCATION]"
    - "[HASH OF SCREENSHOT: SHA-256]"
    - "[WAYBACK ARCHIVE: URL]"
    
  preliminary_impact_assessment:
    commercial_impact: "High | Moderate | Low | Unknown"
    audience_overlap: "High | Moderate | Low | Unknown"
    urgency: "Immediate | Moderate | Low"
    
  next_step: "[WHICH DETECTION MODULE TO ACTIVATE]"
```

---

*→ Next: `EVIDENCE_COMPARISON_REPORT.md`*  
*→ Back: `INCIDENT_RESPONSE_ENGINE.md`*
