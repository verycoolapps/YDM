# TIMESTAMPING PROTOCOL
## YOUR DEAD MEAT — Trusted Timestamping Methods & Implementation

---

**Purpose:** Documents reliable timestamping methods for establishing creation chronology.  
**Scope:** All projects requiring chronological evidence of creation.  
**Version:** 1.0.0  
**Dependencies:** `PROVENANCE_ENGINE.md`, `HASH_VERIFICATION.md`  

---

## TRUSTED TIMESTAMP SERVICES (RFC 3161)

RFC 3161 is the international standard for trusted timestamps. A TSA (Timestamp Authority) cryptographically binds a document hash to a specific point in time.

### Free/Low-Cost TSA Services
- **DigiStamp:** digistamp.com — free tier available
- **Freetsa.org:** Free RFC 3161 service
- **OpenTSA:** open-source TSA
- **SafeCreative:** creator-focused timestamping

### How to Use (OpenSSL — macOS/Linux)
```bash
# 1. Generate hash of your file
openssl dgst -sha256 -binary myfile.ext > myfile.hash

# 2. Create timestamp request
openssl ts -query -data myfile.ext -no_nonce -sha256 -out myfile.tsq

# 3. Send to TSA and get timestamp token
curl -H "Content-Type: application/timestamp-query" \
     --data-binary @myfile.tsq \
     https://freetsa.org/tsr > myfile.tsr

# 4. Verify timestamp
openssl ts -verify -in myfile.tsr -queryfile myfile.tsq -CAfile tsa_ca.crt

# Store: myfile.ext + myfile.tsr + myfile.tsq
```

---

## PLATFORM-BASED TIMESTAMPS (Practical for Most Creators)

### GitHub/GitLab
Every commit receives a server-side timestamp visible in the repository history. For non-code creators: upload any file to a private repository, commit with a message describing the work.

```bash
git init my-project
git add concept-sketch.png
git commit -m "Initial concept: [describe your work here]"
git remote add origin https://github.com/[username]/[repo].git
git push -u origin main
# GitHub's server timestamp is now your evidence
```

### Cloud Storage
Upload files to Dropbox, Google Drive, OneDrive, or iCloud. The upload timestamp is recorded by the service's servers — independent of your local machine.

**Record:** Service name, file name, upload timestamp, folder URL.

### Email Self-Send
Email yourself files with descriptive subject lines. Email headers contain server-side timestamps.

```
To: yourself@email.com
Subject: [PROJECT NAME] - [DESCRIPTION] - [DATE]
Attachment: [FILE]
```

---

## TIMESTAMP RECORD

```yaml
# TIMESTAMP RECORD
# Asset: [ASSET NAME] | Project: YDM-[ID]

timestamp_record:
  asset_name: "[FILENAME]"
  asset_hash_sha256: "[HASH AT TIME OF TIMESTAMPING]"
  
  timestamps:
    - method: "RFC 3161 TSA | GitHub | Google Drive | Email | Local | Other"
      timestamp_value: "[ISO 8601 TIMESTAMP]"
      source: "[SERVICE NAME]"
      evidence_location: "[WHERE .TSR FILE / URL IS STORED]"
      verification_possible: "Yes | No"
      strength: "Very Strong | Strong | Moderate | Weak"
      
  notes: "[ANY ADDITIONAL CONTEXT]"
```

---

## TIMESTAMP LIMITATIONS

| Limitation | Mitigation |
|-----------|----------|
| Local system clock can be manipulated | Use external/server timestamps only |
| Free TSA services may change or close | Store the .tsr file permanently; it remains verifiable |
| Platform may delete accounts | Download and preserve evidence locally |
| File modification resets local timestamp | Hash the file before and after to detect changes |

---

*→ Next: `HASH_VERIFICATION.md`*  
*→ Back: `PROVENANCE_ENGINE.md`*
