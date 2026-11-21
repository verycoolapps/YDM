# DIGITAL SIGNATURES
## YOUR DEAD MEAT — DIGITAL SIGNATURES Module

---

**Purpose:** Defines digital signing workflows and verification.  
**Scope:** All projects requiring digital provenance documentation.  
**Version:** 1.0.0  
**Dependencies:** `PROVENANCE_ENGINE.md`, `HASH_VERIFICATION.md`  

---

## DIGITAL SIGNATURES FOR CREATORS

A digital signature cryptographically links a document to the signer's identity. It proves the document came from a specific key holder and has not been modified since signing.

### GPG Signature (Free, Open Standard)

```bash
# Generate a GPG key (do this once)
gpg --full-generate-key
# Choose: RSA and RSA, 4096 bits, never expires (or set expiry)
# Enter your name and email

# Sign a file
gpg --armor --detach-sign filename.ext
# Creates: filename.ext.asc (the signature file)

# Verify a signature
gpg --verify filename.ext.asc filename.ext
# "Good signature" = file is unmodified and from expected key

# Export your public key (share this for verification)
gpg --armor --export your@email.com > public-key.asc
```

### Git Commit Signing

```bash
# Configure git to sign all commits
git config --global user.signingkey [YOUR GPG KEY ID]
git config --global commit.gpgsign true
git config --global tag.gpgsign true

# Verify signed commits
git log --show-signature
```

### Signature Record Template

```yaml
# DIGITAL SIGNATURE RECORD
# Asset: [FILENAME] | Project: YDM-[ID]

signature_record:
  asset_hash_sha256: "[SHA-256]"
  signature_file: "[FILENAME].asc"
  signing_key_id: "[GPG KEY ID — last 8 chars]"
  signing_key_fingerprint: "[FULL FINGERPRINT]"
  signature_date: "[ISO 8601]"
  verification_command: "gpg --verify [FILENAME].asc [FILENAME]"
  public_key_location: "[WHERE YOUR PUBLIC KEY IS PUBLISHED]"
```

---

*→ Next: \`SOURCE_FILE_ARCHIVE.md\`*

---
