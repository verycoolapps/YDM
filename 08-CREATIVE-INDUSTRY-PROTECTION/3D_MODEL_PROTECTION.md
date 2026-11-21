# 3D MODEL PROTECTION
## YOUR DEAD MEAT — 3D Models & Assets Protection Workflow

---

**Purpose:** Specialized protection workflow for 3D Models & Assets projects.  
**Scope:** All 3D Models & Assets projects processed through the YDM system.  
**Version:** 1.0.0  
**Dependencies:** `PRE_CREATION_GATE.md`, `ORIGINALITY_ENGINE.md`, `PROVENANCE_ENGINE.md`  

---

## DISCIPLINE OVERVIEW

3D models are protected as sculptural or artistic works. The specific creative choices in modeling, rigging, UV mapping, and texturing constitute original expression eligible for copyright protection.

---

## SPECIALIZED PROTECTION CHECKLIST

```
3D MODEL PROTECTION CHECKLIST
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

□ Native source file preserved (.blend, .c4d, .maya, .max)
□ Source file metadata includes creator name and date
□ Render turnsheet (360° views) documented and dated
□ Topology documentation (wireframe renders) saved
□ UV map documentation saved
□ Rig structure documented (for rigged models)
□ Material/shader named with creator reference
□ SHA-256 hash of source file recorded
□ Cloud backup with verified timestamp
□ Creative fingerprint documented

□ YDM provenance record established
```

### 3D-Specific Provenance Evidence

```yaml
model_provenance:
  source_file: "[FILENAME.blend/.c4d/etc.]"
  source_file_hash: "[SHA-256]"
  polygon_count: "[COUNT]"
  creation_date: "[DATE]"
  software_version: "[TOOL v.X.X]"
  distinctive_features:
    - "[SPECIFIC MODELING DECISION]"
    - "[RIGGING APPROACH]"
    - "[UV NAMING CONVENTION]"
```

---

## PROVENANCE RECORD FORMAT

For 3D Models & Assets projects, establish provenance using:

```yaml
# 3D Models & Assets PROVENANCE RECORD
# Project ID: YDM-[ID]

discipline_provenance:
  discipline: "3D Models & Assets"
  primary_source_file: "[NATIVE FORMAT SOURCE FILE]"
  source_file_hash: "[SHA-256]"
  creation_tools: "[TOOLS AND VERSIONS USED]"
  creation_date: "[DATE — with evidence quality]"
  key_creative_decisions:
    - "[DECISION THAT IS DISTINCTIVE TO THIS WORK]"
```

---

*→ Back to entry: `../SKILL.md`*  
*→ Next industry module in sequence*
