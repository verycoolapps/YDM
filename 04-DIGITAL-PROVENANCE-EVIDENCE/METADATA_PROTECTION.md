# METADATA PROTECTION
## YOUR DEAD MEAT — METADATA PROTECTION Module

---

**Purpose:** Manages file metadata and attribution embedding.  
**Scope:** All projects requiring digital provenance documentation.  
**Version:** 1.0.0  
**Dependencies:** `PROVENANCE_ENGINE.md`, `HASH_VERIFICATION.md`  

---

## METADATA AS EVIDENCE

File metadata can carry attribution information that persists with the file through copying and sharing. Properly maintained metadata strengthens provenance claims.

### Metadata Types by Format

| Format | Metadata Standard | Key Fields |
|--------|-----------------|-----------|
| JPEG/PNG | EXIF / IPTC / XMP | Creator, Copyright, Description, DateTimeOriginal |
| PDF | XMP / Document Info | Author, Creator, CreationDate, Subject |
| MP3/Audio | ID3 | Artist, Copyright, Comment, Year |
| SVG/HTML | HTML meta tags | Author, Description, Copyright |
| PSD/AI | XMP | Creator, Rights, Description |

### Recommended Metadata Fields

```
Creator:        [YOUR NAME]
Copyright:      © [YEAR] [NAME] — All Rights Reserved
Rights:         All rights reserved. Contact: [REFERENCE]
Description:    [BRIEF DESCRIPTION OF THE WORK]
Subject:        [KEYWORDS DESCRIBING THE WORK]
Identifier:     YDM-[PROJECT ID]
Date Created:   [ISO 8601]
Software:       [TOOL USED TO CREATE IT]
```

### Tools for Embedding Metadata

```bash
# ExifTool (cross-platform, free)
exiftool -Creator="Your Name"          -Copyright="© 2024 Your Name"          -Description="[Description]"          -XMP:Identifier="YDM-XXXXXXXX"          filename.jpg

# Batch process all files in directory
exiftool -Creator="Your Name" -Copyright="© 2024 Your Name" *.jpg
```

### Metadata Preservation Warning

Metadata can be stripped by:
- Social media platform uploads (most strip EXIF)
- Online compression tools
- Some conversion workflows
- Deliberate stripping by infringers

**Best practice:** Always preserve the original file with intact metadata. The stripped version on a platform is not your master copy.

---

*→ Next: \`DIGITAL_SIGNATURES.md\`*

---
