# SOFTWARE PROJECT PROTECTION
## YOUR DEAD MEAT — Software Projects Protection Workflow

---

**Purpose:** Specialized protection workflow for Software Projects projects.  
**Scope:** All Software Projects projects processed through the YDM system.  
**Version:** 1.0.0  
**Dependencies:** `PRE_CREATION_GATE.md`, `ORIGINALITY_ENGINE.md`, `PROVENANCE_ENGINE.md`  

---

## DISCIPLINE OVERVIEW

Software is protected by copyright as a literary work. The specific code expression is protected, not the underlying idea or algorithm. Source code, compiled code, and documentation can all be separately protected.

---

## SPECIALIZED PROTECTION CHECKLIST

```
SOFTWARE PROJECT PROTECTION CHECKLIST
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

□ Repository initialized with first commit on Day 1
□ All commits have meaningful messages describing changes
□ License file (LICENSE) placed in repository root
□ Copyright notice in source file headers
□ README includes creator attribution
□ Dependencies documented with their licenses
□ No incompatible open-source licenses in dependency tree
□ Original algorithms and architectures documented
□ API design documented (if public API)
□ Release tags applied with semantic versioning
□ YDM provenance record established
```

### Software-Specific Protection Record

```yaml
software_protection:
  repository_url: "[PUBLIC URL — if applicable]"
  first_commit_hash: "[GIT SHA]"
  first_commit_date: "[DATE]"
  license_type: "[MIT | Apache | GPL | Proprietary]"
  license_file_location: "LICENSE"
  copyright_in_headers: "Yes | No"
  dependency_licenses_reviewed: "Yes | No | In Progress"
```

---

## PROVENANCE RECORD FORMAT

For Software Projects projects, establish provenance using:

```yaml
# Software Projects PROVENANCE RECORD
# Project ID: YDM-[ID]

discipline_provenance:
  discipline: "Software Projects"
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
