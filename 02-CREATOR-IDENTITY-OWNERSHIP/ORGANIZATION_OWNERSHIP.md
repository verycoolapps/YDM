# ORGANIZATION OWNERSHIP
## YOUR DEAD MEAT — Company & Institutional Ownership Declarations

---

**Purpose:** Handles company and institutional ownership declarations, work-for-hire scenarios, and corporate IP management.  
**Scope:** All projects created within or for an organizational context.  
**Version:** 1.0.0  
**Dependencies:** `OWNER_VERIFICATION_ENGINE.md`, `CONTRACTUAL_RIGHTS.md`  

---

## ORGANIZATIONAL OWNERSHIP TYPES

### Work Made for Hire (Most Common)
Work created by an employee within the scope of employment. In many jurisdictions, the employer is considered the legal author and owner.

**Triggers:**
- Creator is an employee (not independent contractor)
- Work is created within the scope of employment duties
- Work is on company time, with company resources

**YDM Response:** Document as organizational ownership. Note that individual creator may retain moral rights in some jurisdictions.

### Contractor/Freelance Work
In many jurisdictions, independent contractors retain copyright unless there's a written assignment agreement.

**YDM Response:** Flag as requiring written contract review. Without explicit assignment, rights may remain with the contractor.

### Commissioned Work
Work specially commissioned for a specific purpose. Rules vary significantly by jurisdiction.

**YDM Response:** Require documentation of commission agreement and any IP assignment clause.

---

## ORGANIZATION RECORD TEMPLATE

```yaml
# ORGANIZATION OWNERSHIP RECORD
# Project ID: YDM-[ID]

organization_ownership:
  organization_name: "[COMPANY/INSTITUTION NAME — USER-DECLARED]"
  organization_type: "Corporation | LLC | Partnership | Non-profit | Government | Educational | Other"
  registration_country: "[COUNTRY]"
  
  ownership_basis:
    basis: "Work-for-Hire | Assignment | Commission | License-In | Other"
    documentation: "Written Contract | Employment Agreement | IP Policy | Verbal | None"
    documentation_reference: "[DOCUMENT NAME/DATE IF EXISTS]"
    
  authorized_representative:
    name: "[PERSON MANAGING THIS PROJECT]"
    title: "[THEIR ROLE]"
    authority_level: "Full IP Authority | Delegated | Unknown"
    
  individual_creator_acknowledgment:
    creator_names: "[LIST OF INDIVIDUAL CREATORS]"
    creator_acknowledged_in_records: "Yes | No"
    creator_moral_rights_status: "Retained | Waived | Unknown | N/A"
    
  registration_status:
    formally_registered: "Yes | No | In Progress"
    registration_type: "[Copyright | Trademark | Patent | None]"
    registration_number: "[IF REGISTERED]"
    registration_jurisdiction: "[WHERE REGISTERED]"
    
  ip_policy_reference:
    has_ip_policy: "Yes | No | Unknown"
    policy_reference: "[POLICY NAME/DATE IF EXISTS]"
    policy_covers_this_work: "Yes | No | Unclear"
```

---

## CORPORATE ATTRIBUTION STANDARD

When an organization owns a work:

```
© [YEAR] [ORGANIZATION NAME] — All Rights Reserved
YDM Project ID: [YDM-XXXXXXXX]
Created by: [INDIVIDUAL CREATOR NAME(S)] for [ORGANIZATION]
```

Minimal corporate attribution:
```
© [YEAR] [ORG NAME] | YDM-[ID]
```

---

## FLAG: ORGANIZATIONAL OWNERSHIP UNCERTAINTY

When organizational ownership is unclear:

```
⚠️  OWNERSHIP UNCERTAINTY DETECTED

The employment/contractor relationship for this project
has not been fully documented.

Questions to resolve:
  1. Is [CREATOR NAME] an employee or independent contractor?
  2. Does an employment/service agreement address IP ownership?
  3. Was this work created within the scope of paid duties?

Until resolved, this record notes ownership as: "DISPUTED — PENDING DOCUMENTATION"
Recommended action: Review applicable employment agreement
                    or consult a qualified IP attorney.
```

---

*→ Next: `IDENTITY_CONSISTENCY.md`*  
*→ Contract details: `../06-LEGAL-RIGHTS-INTELLIGENCE/CONTRACTUAL_RIGHTS.md`*
