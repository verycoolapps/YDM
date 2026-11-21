# IDENTITY CONSISTENCY
## YOUR DEAD MEAT — Attribution Consistency Detection & Management

---

**Purpose:** Detects and resolves inconsistencies in creator attribution across a project's documentation.  
**Scope:** All projects. Runs as a validation layer after creator records are established.  
**Version:** 1.0.0  
**Dependencies:** `CREATOR_IDENTITY_ENGINE.md`, `CONTRIBUTOR_REGISTRY.md`  

---

## CONSISTENCY CHECKS

### Check 1 — Name Consistency
Creator name must be consistent across all records. Flag if different spellings, formats, or names appear.

**Common causes:**
- Legal name vs. professional name confusion
- Name change during project lifecycle
- Transcription errors

**Resolution:** Establish one canonical name per record; note variations explicitly.

### Check 2 — Attribution vs. Ownership Consistency
The name in the attribution credit must align with the declared owner, or the discrepancy must be documented.

**Common causes:**
- Studio name in attribution but personal name in ownership records
- Pseudonym in public attribution, legal name in legal records

**Resolution:** Document both forms with explicit relationship noted.

### Check 3 — Version-to-Attribution Consistency
Attribution embedded in older versions must align with current records.

### Check 4 — Contributor Acknowledgment Consistency
If a contributor is mentioned in a project, their record must exist in the Contributor Registry.

### Check 5 — Cross-Document Consistency
All documents referencing this project must use the same Project ID and creator name.

---

## CONSISTENCY AUDIT TEMPLATE

```yaml
# IDENTITY CONSISTENCY AUDIT
# Project ID: YDM-[ID]
# Audit Date: [DATE]

consistency_audit:
  
  name_consistency:
    creator_name_in_cir: "[NAME]"
    creator_name_in_declaration: "[NAME]"
    creator_name_in_certificates: "[NAME]"
    creator_name_in_embedded_metadata: "[NAME]"
    consistent: "Yes | No — [DISCREPANCY DESCRIPTION]"
    
  attribution_ownership_alignment:
    attribution_credit: "[NAME USED FOR CREDIT]"
    declared_owner: "[NAME OF RIGHTS HOLDER]"
    relationship_documented: "Yes | No"
    consistent: "Yes | No — [NOTE]"
    
  contributor_records_complete:
    contributors_named_in_project: "[LIST]"
    contributors_in_registry: "[LIST]"
    unregistered_contributors: "[LIST — if any]"
    
  project_id_consistency:
    id_in_cir: "YDM-[ID]"
    id_in_declaration: "YDM-[ID]"
    id_in_certificates: "YDM-[ID]"
    consistent: "Yes | No"
    
  audit_result: "PASS | FAIL — [ISSUES TO RESOLVE]"
  resolution_required: "Yes | No"
```

---

## INCONSISTENCY RESOLUTION PROTOCOL

When an inconsistency is found:

```
INCONSISTENCY DETECTED
━━━━━━━━━━━━━━━━━━━━━

Type: [NAME MISMATCH | ATTRIBUTION-OWNERSHIP GAP | MISSING CONTRIBUTOR RECORD | OTHER]
Location: [WHERE THE INCONSISTENCY WAS FOUND]
Details: [SPECIFIC DISCREPANCY]

Options:
  1. Correct the record (specify which is authoritative)
  2. Document both versions with explanation
  3. Flag as "Under Review" until resolved

Recommended: Resolve before any formal notice is issued.
An inconsistent attribution record weakens a legal position.
```

---

*→ Next: `ATTRIBUTION_ENGINE.md`*  
*→ Back: `ORGANIZATION_OWNERSHIP.md`*
