# ENCRYPTION GUIDELINES
## YOUR DEAD MEAT — Security & Privacy Module

---

**Purpose:** Defines appropriate encryption recommendations.
**Scope:** All system operations and evidence handling.  
**Version:** 1.0.0  
**Dependencies:** `GLOBAL_RULES.md`, `EVIDENCE_VAULT.md`  

---

## ENCRYPTION RECOMMENDATIONS

### File Encryption for Evidence Storage

**For macOS:**
```bash
# Encrypt a folder of evidence (using built-in tools)
# Option 1: Create encrypted disk image
hdiutil create -encryption AES-256   -stdinpass   -type UDIF   -size 1g   /path/to/evidence-vault.dmg

# Option 2: Use Finder > right-click > Compress (not encrypted)
# Then encrypt with GPG
gpg --symmetric --cipher-algo AES256 evidence.zip
```

**For cross-platform (VeraCrypt — free, open source):**
- Download from veracrypt.fr
- Create encrypted container for evidence vault
- Strong passphrase (minimum 20 characters, random)

### Encryption Strength Requirements

| Use Case | Minimum Standard |
|---------|----------------|
| Evidence vault | AES-256 |
| File transfer to counsel | TLS 1.3 or GPG |
| Backup encryption | AES-256 |
| Password protection only | NOT sufficient for sensitive evidence |

### Password/Passphrase Requirements

```
SECURE PASSPHRASE GUIDELINES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Length: Minimum 20 characters
Type: Random words or character combination
Storage: Password manager (Bitwarden, 1Password, KeePassXC)
Never: Written on paper or stored in plain text
```

---
