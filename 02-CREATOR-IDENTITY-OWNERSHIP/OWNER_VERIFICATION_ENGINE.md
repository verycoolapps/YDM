# OWNER VERIFICATION ENGINE
## YOUR DEAD MEAT — Ownership Claim Documentation & Verification

---

**Purpose:** Documents ownership claims and provides verification workflows for establishing rights holder identity.  
**Scope:** All projects where ownership needs to be established or verified.  
**Version:** 1.0.0  
**Dependencies:** `CREATOR_IDENTITY_ENGINE.md`, `RIGHTS_HOLDER_MANAGEMENT.md`  

---

## OWNERSHIP TYPES

### Type 1 — Original Creator Ownership
Creator and owner are the same person. Created independently, no employment or contract affects ownership.

**Documentation:** Creator Identity Record is sufficient. Mark owner as "Same as creator."

### Type 2 — Organizational / Employer Ownership
Work created within employment. Employer may own rights under work-made-for-hire doctrine.

**Documentation:** Requires employment context, job scope documentation, and jurisdiction-specific analysis.

### Type 3 — Client Ownership
Work commissioned by a client. Ownership depends heavily on jurisdiction and written agreement.

**Documentation:** Requires contract review. Without written assignment, copyright may remain with creator in many jurisdictions.

### Type 4 — Collaborative / Joint Ownership
Multiple creators. Ownership is shared by default in most jurisdictions absent agreement.

**Documentation:** Requires documented contribution records and any existing collaboration agreements.

### Type 5 — Assigned Ownership
Creator has formally transferred rights to another party via written agreement.

**Documentation:** Requires assignment agreement reference. YDM cannot verify assignment without document.

### Type 6 — Licensed (Not Owned)
User has permission to use something but does not own it.

**Documentation:** Record license terms. Clearly distinguish "licensed to use" from "owns."

---

## OWNERSHIP VERIFICATION MATRIX

| Claim Type | Evidence Required | Verification Level |
|-----------|-----------------|------------------|
| Personal creation | Creator record + timestamps | Unverified (declaration only) |
| Employment creation | Contract + job description | Partially verified |
| Client work | Contract with assignment clause | Partially verified |
| Collaborative | Collaboration agreement | Partially verified |
| Formally registered | Government registration certificate | Verified |
| Court-determined | Court order | Verified |

---

## OWNER RECORD TEMPLATE

```yaml
# OWNERSHIP RECORD
# YOUR DEAD MEAT — Owner Verification Engine

ownership_record:
  project_id: "YDM-[ID]"
  
  rights_holder:
    name: "[DECLARED NAME]"
    type: "Individual | Company | Partnership | Institution | Government"
    registration_number: "[IF FORMALLY REGISTERED — Optional]"
    
  ownership_basis:
    basis_type: >
      Original Creation | Work-for-Hire | Assignment |
      Joint Creation | License | Inheritance | Purchase
    documentation_reference: "[CONTRACT/AGREEMENT NAME IF ANY]"
    documentation_status: "None | Referenced | Reviewed | Verified"
    
  rights_scope:
    reproduction_right: "Owner | Licensed | Restricted | Unknown"
    distribution_right: "Owner | Licensed | Restricted | Unknown"
    display_right: "Owner | Licensed | Restricted | Unknown"
    derivative_works_right: "Owner | Licensed | Restricted | Unknown"
    
  jurisdiction: "[PRIMARY JURISDICTION FOR RIGHTS]"
  
  verification_status: "Unverified | Partially Verified | Verified"
  verification_notes: "[ANY SUPPORTING INFORMATION]"
  
  important_disclaimer: >
    This ownership record is based on user-provided declarations.
    YDM cannot independently verify ownership claims. For formal
    legal ownership establishment, consult a qualified IP attorney
    and consider formal registration with relevant authorities.
```

---

## OWNERSHIP VERIFICATION QUESTIONS

When establishing ownership, ask:

```
OWNERSHIP VERIFICATION DIALOGUE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Q1: "Who owns the rights to this project — you personally, 
     a company, or is it shared?"

Q2: "If you created this for an employer or client:
     Is there a written contract that addresses who owns the work?"

Q3: "Have you ever transferred, assigned, or sold rights to 
     any part of this project to anyone else?"

Q4: "Have you formally registered this work with any 
     copyright office or IP authority?"

Q5: "Are there any active disputes about who owns this work?"
```

---

*→ Next: `CONTRIBUTOR_REGISTRY.md`*  
*→ Disputed ownership: `OWNERSHIP_DISPUTE_PROTOCOL.md`*
