# CONTENT ORIGINALITY
## YOUR DEAD MEAT — Written & Multimedia Content Originality Analysis

---

**Purpose:** Analyzes written and multimedia content originality; documents distinctive creative elements in text-based works.  
**Scope:** Books, articles, scripts, research papers, blog posts, documentation, educational content, presentations.  
**Version:** 1.0.0  
**Dependencies:** `ORIGINALITY_ENGINE.md`, `CONCEPT_PROVENANCE.md`  

---

## WRITTEN CONTENT ORIGINALITY

### Strongly Protected Elements
- Original narrative structure and story architecture
- Invented fictional worlds, characters, and terminology
- Unique voice, tone, and authorial style
- Original analytical frameworks and argument structures
- Invented characters' dialogue and internal monologue
- Creative non-fiction that expresses facts in a distinctive way

### Not Directly Protected (But Important Context)
- Historical facts, scientific data, news events
- Common phrases and expressions
- Standard structural forms (the "hero's journey" structure itself)
- Generic descriptions of common things

---

## CONTENT ORIGINALITY RECORD

```yaml
# CONTENT ORIGINALITY RECORD
# Project ID: YDM-[ID]

content_originality:
  
  content_type: "Fiction | Non-fiction | Journalism | Research | Educational | Technical | Mixed"
  primary_format: "Book | Article | Script | Report | Blog | Documentation | Other"
  word_count_approximate: "[NUMBER]"
  language: "[LANGUAGE(S)]"
  
  distinctive_elements:
    voice_and_style:
      description: "[HOW THE AUTHOR'S VOICE IS DISTINCTIVE]"
      examples: "[SAMPLE PHRASES OR PASSAGES SHOWING STYLE]"
      
    structural_originality:
      narrative_structure: "[HOW THE WORK IS STRUCTURED — if original]"
      original_to_this_work: "Yes | No | Adapted from [SOURCE]"
      
    invented_elements:
      - type: "Character | World | Terminology | Concept | Framework | System"
        name: "[INVENTED NAME]"
        description: "[WHAT WAS INVENTED]"
        
    research_and_synthesis:
      original_research: "Yes — describe | No"
      original_synthesis: "[HOW INFORMATION IS UNIQUELY COMBINED]"
      
  source_acknowledgment:
    sources_cited: "Yes | No | In Progress"
    citation_style: "[APA | MLA | Chicago | Custom]"
    source_material_clearly_distinguished: "Yes | No"
    
  publication_history:
    previously_published: "Yes — where and when | No"
    publication_rights_granted: "[TO WHOM — publisher, journal, etc.]"
    rights_retained: "[WHAT RIGHTS CREATOR KEPT]"
    
  content_hash:
    final_draft_sha256: "[HASH OF FINAL FILE — if available]"
    draft_dates:
      - version: "[DRAFT NUMBER]"
        date: "[DATE]"
        significant_changes: "[WHAT CHANGED]"
```

---

## DISTINGUISHING FACTS FROM EXPRESSION

For non-fiction and research content:

| Element | Protection Status | YDM Approach |
|---------|-----------------|-------------|
| Raw facts and data | Not protected | Document as source, not as original creation |
| Compilation and selection of facts | May be protected (if original selection) | Document the specific curatorial choices |
| Analysis and interpretation | Protected (the specific expression) | Document the original analytical approach |
| Quotations from others | Protected by original author | Document source and license/fair use basis |

---

*→ Next: `AI_GENERATION_DISCLOSURE.md`*  
*→ Document copy detection: `../05-ANTI-PLAGIARISM-DEFENSE/DOCUMENT_COPY_DETECTION.md`*
