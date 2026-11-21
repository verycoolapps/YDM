# CONTRACTUAL RIGHTS
## YOUR DEAD MEAT — Legal & Rights Intelligence Module

---

**Purpose:** Reviews relevant contractual ownership provisions.
**Scope:** All projects with legal rights considerations.  
**Version:** 1.0.0  
**Dependencies:** `GLOBAL_RULES.md`, `LEGAL_LIMITATIONS.md`  

---

## CONTRACTUAL RIGHTS REVIEW

Contracts can transfer, limit, or expand IP rights beyond the defaults established by copyright law.

### Key Contract Types Affecting IP

| Contract Type | IP Implication |
|--------------|---------------|
| Employment Agreement | May assign all work-product to employer |
| Freelance/Service Agreement | Defines ownership of deliverables |
| IP Assignment Agreement | Transfers copyright to another party |
| Non-Disclosure Agreement | Protects confidential information |
| Collaboration Agreement | Establishes joint ownership terms |
| License Agreement | Grants usage rights without ownership transfer |
| Work-Made-For-Hire Agreement | Establishes employer/commissioner as author |

### Contract Review Checklist

```
IP CONTRACT REVIEW CHECKLIST
━━━━━━━━━━━━━━━━━━━━━━━━━━━━

□ Is there a written agreement for this project?
□ Does it address who owns the work product?
□ Does it contain an IP assignment clause?
  (transfers copyright from creator to commissioner)
□ Does it contain a work-made-for-hire clause?
□ Does it address rights in pre-existing work?
  (things you bring to the project that you owned before)
□ Does it address rights in tools and methods?
□ Does it contain a confidentiality provision?
□ Does it address derivative works?
□ What jurisdiction/governing law applies?
□ Are there any license-back provisions?
  (you assign rights but get a license to use your own work)
```

### Contract Record

```yaml
contract_record:
  contract_type: "[TYPE]"
  parties: "[PARTY A] and [PARTY B]"
  effective_date: "[DATE]"
  ip_assignment_clause: "Yes — describes: [WHAT] | No | Unclear"
  work_for_hire_clause: "Yes | No"
  pre_existing_ip_addressed: "Yes | No | Not applicable"
  governing_law: "[JURISDICTION]"
  document_reference: "[WHERE CONTRACT IS STORED]"
  reviewed_by_lawyer: "Yes | No"
```

---
