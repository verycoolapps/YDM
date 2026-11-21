# ARCHITECTURAL WORK PROTECTION
## YOUR DEAD MEAT — Architectural Designs Protection Workflow

---

**Purpose:** Specialized protection workflow for Architectural Designs projects.  
**Scope:** All Architectural Designs projects processed through the YDM system.  
**Version:** 1.0.0  
**Dependencies:** `PRE_CREATION_GATE.md`, `ORIGINALITY_ENGINE.md`, `PROVENANCE_ENGINE.md`  

---

## DISCIPLINE OVERVIEW

Architectural works receive copyright protection for original design elements. Both plans/drawings and completed buildings can be protected. Functional elements may not be protected, but creative expression in design is.

---

## SPECIALIZED PROTECTION CHECKLIST

```
ARCHITECTURAL WORK PROTECTION CHECKLIST
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

□ Original design files preserved (CAD, BIM, Sketch)
□ Design concepts documented in writing before detailed drawings
□ Date-stamped design presentation to client preserved
□ Schematic and design development drawings preserved
□ Written design intent document created
□ Attribution in all drawings and renderings
□ Client contract reviewed for IP ownership provisions
□ Photography of completed building documenting original elements

□ YDM provenance record established
```

### Architectural IP Notes

- **Plans and drawings:** Protected as artistic/literary works
- **Completed buildings:** Protected as architectural works in many jurisdictions
- **Standard structural solutions:** May not be protectable (functional necessity)
- **Client contracts:** Often transfer IP to client — review carefully

> **Indonesia:** Hak cipta atas karya arsitektur dilindungi berdasarkan UU No. 28 Tahun 2014.

---

## PROVENANCE RECORD FORMAT

For Architectural Designs projects, establish provenance using:

```yaml
# Architectural Designs PROVENANCE RECORD
# Project ID: YDM-[ID]

discipline_provenance:
  discipline: "Architectural Designs"
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
