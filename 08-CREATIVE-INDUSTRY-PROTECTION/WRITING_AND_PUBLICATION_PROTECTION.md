# WRITING AND PUBLICATION PROTECTION
## YOUR DEAD MEAT — Writing & Publications Protection Workflow

---

**Purpose:** Specialized protection workflow for Writing & Publications projects.  
**Scope:** All Writing & Publications projects processed through the YDM system.  
**Version:** 1.0.0  
**Dependencies:** `PRE_CREATION_GATE.md`, `ORIGINALITY_ENGINE.md`, `PROVENANCE_ENGINE.md`  

---

## DISCIPLINE OVERVIEW

Written works receive strong copyright protection from the moment of creation. This includes fiction, non-fiction, journalism, scripts, poetry, song lyrics, and other textual works.

---

## SPECIALIZED PROTECTION CHECKLIST

```
WRITING & PUBLICATION PROTECTION CHECKLIST
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

□ Manuscript versions preserved with dates
□ Drafts saved with timestamps (version numbering recommended)
□ Research notes and outlines preserved
□ For published work: Publication record (ISBN, DOI, URL) documented
□ Self-send via email: Draft emailed to self with meaningful subject
□ Cloud backup of all versions
□ For books: Copyright notice on copyright page
□ For online: Copyright notice visible on page
□ For important works: Register with copyright authority

□ YDM provenance record established
```

### Writing-Specific Evidence

```yaml
writing_evidence:
  manuscript_versions:
    - version: "v[N]"
      date: "[DATE]"
      word_count: "[COUNT]"
      hash: "[SHA-256]"
      
  publication_record:
    platform: "[WHERE PUBLISHED]"
    date: "[DATE]"
    url: "[URL]"
    archived: "[WAYBACK URL]"
    isbn_doi: "[IF APPLICABLE]"
```

---

## PROVENANCE RECORD FORMAT

For Writing & Publications projects, establish provenance using:

```yaml
# Writing & Publications PROVENANCE RECORD
# Project ID: YDM-[ID]

discipline_provenance:
  discipline: "Writing & Publications"
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
