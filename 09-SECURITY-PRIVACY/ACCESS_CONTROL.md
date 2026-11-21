# ACCESS CONTROL
## YOUR DEAD MEAT — Security & Privacy Module

---

**Purpose:** Defines authorization and evidence access management.
**Scope:** All system operations and evidence handling.  
**Version:** 1.0.0  
**Dependencies:** `GLOBAL_RULES.md`, `EVIDENCE_VAULT.md`  

---

## ACCESS MANAGEMENT

### Evidence Access Principles

1. **Need to know:** Evidence is accessible only to those with a legitimate need
2. **Minimum privilege:** Grant the minimum access level required
3. **Explicit authorization:** Access must be explicitly authorized, not assumed
4. **Audit:** Access events should be recorded where possible

### Access Levels

| Level | Who | Access |
|-------|-----|--------|
| Creator | Project owner | Full access to all project evidence |
| Co-creator | Documented contributor | Access to their own contribution records |
| Legal counsel | Explicitly authorized | Access to relevant case evidence only |
| Third party | None by default | No access without creator authorization |

### Evidence Sharing Protocol

```
BEFORE SHARING EVIDENCE WITH ANY THIRD PARTY:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

□ Confirm the third party's identity and role
□ Confirm legitimate purpose for access
□ Determine which specific evidence they need
□ Share only what is necessary
□ Record the sharing event in Chain of Custody
□ For legal proceedings: use secure transfer methods
□ Consider whether attorney-client privilege applies
```

---
