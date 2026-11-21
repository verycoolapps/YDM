# CODE ORIGINALITY
## YOUR DEAD MEAT — Software Code Provenance & Originality Analysis

---

**Purpose:** Analyzes code provenance, originality indicators, and similarity detection methodology for software projects.  
**Scope:** All software, scripts, libraries, applications, and code-containing projects.  
**Version:** 1.0.0  
**Dependencies:** `ORIGINALITY_ENGINE.md`, `VERSION_HISTORY_ENGINE.md`  

---

## CODE ORIGINALITY FRAMEWORK

### What Makes Code Original
Copyright in software protects specific creative expression in code — not the underlying idea or algorithm. Original elements include:
- Specific implementation choices among many possible approaches
- Creative naming conventions and organizational structure
- Original comments, documentation, and variable naming
- Unique combination of techniques and patterns

### What Code Copyright Does NOT Protect
- Algorithms and mathematical methods (may be patentable instead)
- Standard industry patterns and "scenes à faire" (inevitable code for a given problem)
- APIs and interfaces (jurisdiction-dependent and evolving)
- Functional requirements and specifications

---

## CODE PROVENANCE RECORD

```yaml
# CODE PROVENANCE RECORD
# Project ID: YDM-[ID]

code_provenance:
  
  repository_information:
    version_control: "Git | SVN | Mercurial | None"
    repository_initialized: "[DATE]"
    first_commit_hash: "[GIT SHA — most reliable provenance anchor]"
    first_commit_date: "[DATE FROM GIT LOG]"
    remote_repository: "[PUBLIC URL — if exists and user consents to record]"
    
  language_and_stack:
    primary_language: "[LANGUAGE]"
    frameworks: "[FRAMEWORKS/LIBRARIES]"
    dependencies: "[MAJOR DEPENDENCIES]"
    
  original_code_elements:
    distinctive_implementations:
      - "[SPECIFIC APPROACH THAT IS DISTINCTIVELY THIS CREATOR'S]"
    naming_conventions:
      - "[UNIQUE NAMING PATTERNS USED]"
    architectural_decisions:
      - "[SPECIFIC STRUCTURAL CHOICES]"
      
  third_party_code:
    - package: "[PACKAGE NAME]"
      version: "[VERSION]"
      license: "[LICENSE TYPE]"
      usage: "[HOW IT'S USED]"
      
  license_applied_to_this_code:
    license_type: "[MIT | Apache 2.0 | GPL | Proprietary | Other]"
    license_declared_in: "LICENSE file | Header comments | README | None"
    
  code_hash_anchors:
    - file: "[FILENAME]"
      sha256: "[HASH]"
      date_captured: "[DATE]"
```

---

## GIT AS PROVENANCE TOOL

Git commit history is one of the strongest provenance tools available for software:

```bash
# Show full commit history with timestamps
git log --pretty=format:"%H %ai %s" --all

# Hash of the entire repository at a point in time
git rev-parse HEAD

# Archive with provenance metadata
git archive --format=tar.gz --prefix=project-v1.0/ HEAD > project-v1.0.tar.gz
```

**Best practices for provenance:**
1. Commit frequently with meaningful messages
2. Use signed commits (`git commit -S`) for stronger attribution
3. Push to a dated remote host — GitHub/GitLab timestamps serve as independent evidence
4. Tag releases with semantic versions

---

## CODE SIMILARITY DETECTION APPROACH

For detecting potential code copying (see `CODE_COPY_DETECTION.md` for full methodology):

| Similarity Type | Potential Significance |
|----------------|----------------------|
| Identical code blocks | High — investigate |
| Same logic with renamed variables | High — investigate |
| Same architecture with different implementation | Moderate — could be independent |
| Same algorithm (standard algorithm) | Low — not copying unless expression is identical |
| Same language and framework patterns | Low — common in the field |

---

*→ Next: `CONTENT_ORIGINALITY.md`*  
*→ Code copy detection: `../05-ANTI-PLAGIARISM-DEFENSE/CODE_COPY_DETECTION.md`*
