# SOURCE FILE ARCHIVE
## YOUR DEAD MEAT — SOURCE FILE ARCHIVE Module

---

**Purpose:** Preserves original source files and materials.  
**Scope:** All projects requiring digital provenance documentation.  
**Version:** 1.0.0  
**Dependencies:** `PROVENANCE_ENGINE.md`, `HASH_VERIFICATION.md`  

---

## SOURCE FILE PRESERVATION

Source files — the original native-format files in the tool that created them — are among the most powerful provenance evidence:

1. Source files contain embedded creation metadata
2. They show the creative process (layers, history, structure)
3. They are extremely difficult to fake convincingly
4. They prove the creator had access to the full original, not just a copy

### Source vs. Export

| File Type | Category | Evidentiary Value |
|-----------|---------|-----------------|
| .psd, .ai, .xd (layered source) | Source | Very High |
| .blend, .c4d, .maya (3D source) | Source | Very High |
| .git repository with history | Source | Very High |
| .fla, .aep (animation source) | Source | Very High |
| Exported .jpg, .png, .mp4 | Export | Moderate |
| Exported .pdf | Export | Moderate |

### Archive Record

```yaml
# SOURCE FILE ARCHIVE RECORD
# Project ID: YDM-[ID]

source_archive:
  project_id: "YDM-[ID]"
  
  source_files:
    - filename: "[SOURCE FILE NAME]"
      format: "[FORMAT — .psd | .blend | .git | etc.]"
      tool_version: "[TOOL AND VERSION USED TO CREATE IT]"
      sha256: "[HASH]"
      last_modified: "[DATE — from file metadata]"
      archived_date: "[DATE OF ARCHIVE]"
      archive_location: "[WHERE IT IS STORED — LOCAL | CLOUD | BOTH]"
      
  archive_policy:
    retention_period: "Indefinite | [X years]"
    backup_locations: "[LIST OF BACKUP LOCATIONS]"
    access_restricted: "Yes | No"
```

### Archive Creation Commands

```bash
# Create dated archive with hash verification
DATE=$(date +%Y%m%d)
zip -r "${PROJECT_NAME}-source-${DATE}.zip" ./source-files/
shasum -a 256 "${PROJECT_NAME}-source-${DATE}.zip" > "${PROJECT_NAME}-source-${DATE}.sha256"
```

---

*→ Next: \`CHAIN_OF_CUSTODY.md\`*

---
