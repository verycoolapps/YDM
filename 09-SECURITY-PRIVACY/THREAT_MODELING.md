# THREAT MODELING
## YOUR DEAD MEAT — Security & Privacy Module

---

**Purpose:** Identifies realistic threats and appropriate mitigations.
**Scope:** All system operations and evidence handling.  
**Version:** 1.0.0  
**Dependencies:** `GLOBAL_RULES.md`, `EVIDENCE_VAULT.md`  

---

## THREAT MODEL

### Realistic Threats for Creators

| Threat | Likelihood | Impact | Mitigation |
|--------|-----------|--------|-----------|
| Evidence file corruption | Medium | High | Regular backups, hash verification |
| Account compromise | Medium | High | Strong passwords, 2FA on all services |
| Accidental deletion | High | High | Multiple backups, never delete originals |
| Cloud service closure | Low | Medium | Multiple cloud services, local backup |
| Evidence tampering | Low | Very High | Hash verification, trusted timestamps |
| False accusation against user | Low | High | Maintain accurate evidence; don't overstate claims |
| Alleged infringer claims user plagiarized them | Low | High | Thorough provenance documentation is the best defense |
| Legal action against user for C&D abuse | Low | High | Only send evidence-based, legally reviewed notices |

### Threat Mitigations

#### For Evidence Integrity
- Use cryptographic hashes to verify files haven't changed
- Use trusted timestamps to establish when files existed
- Use multiple storage locations to prevent single point of failure

#### For Account Security
- Strong, unique passwords for all accounts holding evidence
- Two-factor authentication (2FA) on GitHub, cloud storage, email
- Do not share credentials

#### For Legal Threats
- Never send formal notices without adequate evidence
- Always have notices reviewed by qualified legal counsel
- Document everything in case the situation escalates

---
