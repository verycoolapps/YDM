# 3D ASSET SIMILARITY
## YOUR DEAD MEAT — 3D ASSET SIMILARITY Module

---

**Purpose:** Analyzes 3D models and digital asset similarities.  
**Scope:** Specialized detection for this asset type.  
**Version:** 1.0.0  
**Dependencies:** `PLAGIARISM_DETECTION_ENGINE.md`, `SIMILARITY_ANALYSIS.md`, `FALSE_POSITIVE_PROTECTION.md`  

---

## 3D ASSET SIMILARITY DETECTION

### 3D-Specific Similarity Indicators

| Indicator | Strength | Notes |
|-----------|---------|-------|
| Identical topology / polygon flow | Very Strong | Mesh structure is creator choice |
| Identical UV layout | Strong | Specific to creator's workflow |
| Same bone/armature naming | Strong | Naming is arbitrary and distinctive |
| Same mesh errors/artifacts | Strong | Specific artifacts don't recur by chance |
| Same unusual detail decisions | Moderate | Small choices reveal copying |
| Same basic silhouette | Weak | May be coincidental |
| Same genre conventions | None | Expected in the field |

### 3D Asset Fingerprint Elements

```yaml
3d_asset_fingerprint:
  asset_name: "[ASSET NAME]"
  asset_type: "Character | Vehicle | Environment | Prop | Other"
  
  mesh_characteristics:
    polygon_count: "[COUNT]"
    topology_description: "[KEY MESH FLOW DECISIONS]"
    distinctive_mesh_choices:
      - "[SPECIFIC TOPOLOGY DECISION]"
      
  rig_characteristics:
    bone_count: "[COUNT]"
    bone_naming_convention: "[PATTERN]"
    distinctive_rig_elements:
      - "[SPECIFIC RIG CHOICE]"
      
  material_characteristics:
    shader_names: "[LIST]"
    texture_naming_convention: "[PATTERN]"
    
  metadata_embedded:
    creator_in_file: "[NAME IN FILE METADATA]"
    creation_software_version: "[TOOL AND VERSION]"
```

---
