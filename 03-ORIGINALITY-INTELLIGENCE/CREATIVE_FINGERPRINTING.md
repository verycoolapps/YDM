# CREATIVE FINGERPRINTING
## YOUR DEAD MEAT — Structured Asset Fingerprinting & Signature Documentation

---

**Purpose:** Creates structured fingerprints from creative assets to enable future comparison and authenticity verification.  
**Scope:** All projects with documentable creative assets.  
**Version:** 1.0.0  
**Dependencies:** `ORIGINALITY_ENGINE.md`, `HASH_VERIFICATION.md`  

---

## WHAT IS A CREATIVE FINGERPRINT?

A Creative Fingerprint is a **structured description of an asset's distinctive, identifiable characteristics**. Combined with cryptographic file hashes, it creates a two-layer identification system:

- **Layer 1 (Cryptographic):** SHA-256 hash of the file — detects exact bit-for-bit copies
- **Layer 2 (Descriptive):** Human-readable characteristic description — detects partial copies, style theft, and element-level appropriation

---

## CREATIVE FINGERPRINT RECORD

```yaml
# CREATIVE FINGERPRINT
# Asset ID: YDM-FP-[ID]

creative_fingerprint:
  asset_id: "YDM-FP-[AUTO]"
  project_id: "YDM-[ID]"
  asset_name: "[FILENAME OR DESCRIPTIVE NAME]"
  asset_type: "Image | Vector | Code | 3D Model | Audio | Video | Document | Other"
  asset_version: "[VERSION AT TIME OF FINGERPRINTING]"
  fingerprint_date: "[ISO 8601]"
  
  cryptographic_identity:
    file_hash_sha256: "[SHA-256 HASH — if available]"
    file_hash_md5: "[MD5 — SECONDARY, for reference only]"
    file_size_bytes: "[SIZE]"
    file_format: "[FORMAT/EXTENSION]"
    
  descriptive_characteristics:
    visual_elements:
      - "[SPECIFIC VISUAL CHARACTERISTIC — e.g., 'diagonal stripe pattern across upper third']"
      - "[COLOR CHARACTERISTICS — e.g., 'dominant crimson #D7193F with titanium accents']"
      - "[COMPOSITIONAL CHOICES]"
    structural_elements:
      - "[STRUCTURAL CHARACTERISTIC — e.g., 'three-column grid with asymmetric bottom element']"
    unique_identifiers:
      - "[ELEMENT THAT IS UNIQUELY IDENTIFIABLE — e.g., 'custom glyph in character M']"
      - "[DISTINCTIVE DETAIL UNLIKELY TO APPEAR BY COINCIDENCE]"
    technical_signatures:
      - "[TECHNICAL CHARACTERISTIC — e.g., 'specific brush texture at 400% zoom reveals grid pattern']"
      
  fingerprint_confidence: "High | Moderate | Low"
  fingerprint_notes: "[ANY ADDITIONAL IDENTIFICATION NOTES]"
```

---

## FINGERPRINTING BY ASSET TYPE

### Image/Illustration Fingerprint Elements
- Exact pixel dimensions
- Color profile (sRGB/Adobe RGB/CMYK)
- Dominant colors (hex values)
- Compositional structure
- Distinctive details visible only at high zoom
- Layer structure (if PSD/AI source available)
- Brush/texture signatures

### Code Fingerprint Elements  
- Repository commit hash (Git SHA)
- Unique function and variable names
- Architectural patterns
- Comments and documentation style
- Specific implementation choices

### 3D Model Fingerprint Elements
- Polygon count
- UV mapping approach
- Material/shader names
- Bone hierarchy naming (for rigged models)
- Specific topology decisions

### Audio/Music Fingerprint Elements
- Sample rate and bit depth
- Key and BPM
- Distinctive production choices
- Unique sound design elements
- Waveform visualization notes

---

## HOW TO GENERATE FILE HASHES

```bash
# macOS/Linux — SHA-256
shasum -a 256 filename.ext

# Windows (PowerShell)
Get-FileHash filename.ext -Algorithm SHA256

# Multiple files
find . -type f | xargs shasum -a 256 > checksums.txt
```

**Important:** Store hash records separately from the files themselves. If both are modified simultaneously, the hash record loses its value.

---

*→ Next: `CONCEPT_PROVENANCE.md`*  
*→ Hash verification: `../04-DIGITAL-PROVENANCE-EVIDENCE/HASH_VERIFICATION.md`*
