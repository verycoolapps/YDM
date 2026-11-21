# DATA RETENTION POLICY
## YOUR DEAD MEAT — Security & Privacy Module

---

**Purpose:** Defines evidence retention periods and deletion practices.
**Scope:** All system operations and evidence handling.  
**Version:** 1.0.0  
**Dependencies:** `GLOBAL_RULES.md`, `EVIDENCE_VAULT.md`  

---

## DATA RETENTION POLICY

### Retention Periods

| Data Type | Minimum Retention | Recommended |
|----------|-----------------|-------------|
| Creation source files | Lifetime of project + 5 years | Permanent |
| Hash records | Lifetime of project + 5 years | Permanent |
| Timestamp tokens | Lifetime of project + 5 years | Permanent |
| Creator records | Lifetime of project + 5 years | Permanent |
| Case investigation records | Until fully resolved + 3 years | Until fully resolved + 7 years |
| Formal notices sent | Until fully resolved + 7 years | Permanent |
| Correspondence with infringers | Until fully resolved + 7 years | Permanent |
| Background research | 1 year after case closure | Per above |

### Retention Rationale

Copyright protection lasts for the life of the creator plus 50-70 years in most jurisdictions. Evidence should ideally be retained as long as the work is commercially valuable and rights are actively enforced.

Statute of limitations for IP claims varies by jurisdiction (typically 3-7 years from discovery). Retain enforcement evidence at least through the applicable limitation period plus a margin.

### Deletion Procedure

When evidence is no longer needed:
1. Confirm case is fully closed and all limitation periods have passed
2. Record the deletion in the audit log
3. Securely delete the files (overwrite or encrypted container deletion)
4. Retain the index/record that evidence once existed (but not the evidence itself)

### No Deletion Rule

**Never delete:** Creator records, provenance records, or formal notices sent. These are part of the permanent project history.

---
