# SECURE STORAGE
## YOUR DEAD MEAT — Security & Privacy Module

---

**Purpose:** Defines secure evidence storage requirements.
**Scope:** All system operations and evidence handling.  
**Version:** 1.0.0  
**Dependencies:** `GLOBAL_RULES.md`, `EVIDENCE_VAULT.md`  

---

## SECURE EVIDENCE STORAGE

### Storage Requirements by Evidence Type

| Evidence Type | Storage Requirement |
|--------------|-------------------|
| Creation source files | Encrypted backup + cloud backup |
| Hash records | Plain text OK (not sensitive); backup essential |
| Timestamp tokens (.tsr files) | Long-term preservation critical |
| Screenshots | Dated folder structure; backup |
| Correspondence | Encrypted if sensitive |
| Legal documents | Encrypted; attorney holds copies |

### Storage Architecture

```
RECOMMENDED STORAGE ARCHITECTURE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

PRIMARY: Local encrypted storage
  → Fast access
  → Full evidence vault
  → Source files

BACKUP 1: Cloud storage (Dropbox/Drive/iCloud)
  → Automatic sync
  → Server-side timestamps
  → Version history

BACKUP 2: External drive (offline)
  → Encrypted
  → Stored separately from primary
  → Updated monthly or at major milestones

BACKUP 3: Remote (optional, for critical IP)
  → Second cloud provider
  → Geographic separation from Backup 1
```

### Evidence Vault Location

Default location: Dedicated encrypted folder separate from working files  
Naming convention: `[PROJECT-NAME]-EVIDENCE-YDM-[ID]/`  
Never store in: Downloads folder, Desktop, Shared drives accessible to others

---
