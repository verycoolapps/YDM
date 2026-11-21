# HASH VERIFICATION
## YOUR DEAD MEAT — Cryptographic File Hashing & Integrity Verification

---

**Purpose:** Uses cryptographic hashes to detect file changes and verify creation integrity.  
**Scope:** All projects with documentable digital files.  
**Version:** 1.0.0  
**Dependencies:** `PROVENANCE_ENGINE.md`, `TIMESTAMPING_PROTOCOL.md`, `CREATIVE_FINGERPRINTING.md`  

---

## CRYPTOGRAPHIC HASH BASICS

A cryptographic hash (SHA-256) produces a fixed-length "fingerprint" of any file. Any change to the file — even one character — produces a completely different hash. This makes hashes ideal for:
- Proving a file has not been modified since a specific time
- Verifying that submitted evidence matches original files
- Detecting tampering in an evidence chain

**Important:** A hash alone does not prove when a file was created. It must be combined with a timestamp to establish chronology.

---

## HASH GENERATION COMMANDS

```bash
# macOS (built-in)
shasum -a 256 filename.ext
# Output: [64-char hex] filename.ext

# macOS alternative
openssl dgst -sha256 filename.ext

# Linux
sha256sum filename.ext

# Windows (PowerShell)
Get-FileHash filename.ext -Algorithm SHA256

# Multiple files in directory
find . -type f -exec shasum -a 256 {} \; > CHECKSUMS-$(date +%Y%m%d).txt

# Git hash (for code files)
git hash-object filename.ext
```

---

## HASH RECORD FORMAT

```yaml
# HASH VERIFICATION RECORD
# Project ID: YDM-[ID]
# Generated: [DATE]

hash_verification_record:
  project_id: "YDM-[ID]"
  generated_date: "[ISO 8601]"
  algorithm: "SHA-256"
  
  files:
    - filename: "[FILE NAME AND PATH]"
      sha256: "[64-CHARACTER HEX HASH]"
      file_size_bytes: "[SIZE]"
      format: "[FILE EXTENSION/TYPE]"
      description: "[WHAT THIS FILE IS]"
      hash_date: "[WHEN HASH WAS GENERATED]"
      timestamp_paired: "Yes — YDM-TS-[ID] | No"
      
  checksum_file: "checksums.txt stored at: [LOCATION]"
  checksum_file_hash: "[SHA-256 OF THE CHECKSUMS FILE ITSELF]"
  
  verification_instructions: >
    To verify: run 'shasum -a 256 [filename]' and compare
    to the hash value above. If values match, file is unchanged.
    If values differ, the file has been modified.
```

---

## HASH-BASED CHAIN OF CUSTODY

For evidence submitted in formal proceedings:

```
HASH CHAIN OF CUSTODY
━━━━━━━━━━━━━━━━━━━━━

ORIGINAL FILE:    [NAME]
HASH AT ORIGIN:   [SHA-256] — Recorded [DATE]
HASH AFTER:       [SHA-256] — Verified [DATE] ← Match confirms no tampering
STORED AT:        [LOCATION]
HANDLED BY:       [NAME]
```

---

*→ Next: `VERSION_HISTORY_ENGINE.md`*  
*→ Timestamps: `TIMESTAMPING_PROTOCOL.md`*
