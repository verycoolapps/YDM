# SIMILARITY ANALYSIS
## YOUR DEAD MEAT — Similarity Detection & Comparison Methodology

---

**Purpose:** Defines structured similarity detection and comparison methodology for originality investigations.  
**Scope:** All investigation scenarios involving potential copying or unauthorized similarity.  
**Version:** 1.0.0  
**Dependencies:** `ORIGINALITY_ENGINE.md`, `PLAGIARISM_DETECTION_ENGINE.md`, `FALSE_POSITIVE_PROTECTION.md`  

---

## SIMILARITY ANALYSIS PRINCIPLES

**Critical distinction:** Similarity is not proof of copying.

Identical or near-identical works can result from:
1. Direct copying (what we investigate)
2. Independent creation (both creators had the same idea)
3. Common source (both borrowed from the same third-party work)
4. Generic conventions (the similarity is industry-standard)
5. Merger doctrine (the idea can only be expressed one way)

YDM analysis must clearly address which of these is most plausible.

---

## SIMILARITY ANALYSIS FRAMEWORK

### Level 1 — Surface Similarity
Casual visual/functional resemblance. Common in creative fields.
**Action:** Note; not sufficient alone for any formal action.

### Level 2 — Structural Similarity
Similar composition, structure, or architecture beyond surface appearance.
**Action:** Investigate whether common conventions explain this.

### Level 3 — Element-Level Similarity
Specific distinctive elements appear in both works in the same relationship.
**Action:** Document precisely which elements match; assess likelihood of independent creation.

### Level 4 — Expression-Level Similarity
The specific creative expression (not just idea) is reproduced.
**Action:** Document exact matching passages/elements; assess copying probability.

### Level 5 — Near-Identical Reproduction
Works are virtually identical in original creative expression.
**Action:** Strongest indicator of copying; document thoroughly; consider formal response.

---

## SIMILARITY ANALYSIS RECORD

```yaml
# SIMILARITY ANALYSIS RECORD
# Case ID: YDM-CASE-[ID]

similarity_analysis:
  
  original_work:
    project_id: "YDM-[ID]"
    creation_date: "[DATE]"
    distinctive_elements: "[FROM ORIGINALITY RECORD]"
    
  compared_work:
    description: "[WHAT WAS FOUND]"
    location: "[URL OR LOCATION — publicly available]"
    discovery_date: "[WHEN FOUND]"
    
  element_comparison:
    - element: "[SPECIFIC ELEMENT BEING COMPARED]"
      in_original: "[HOW IT APPEARS IN ORIGINAL WORK]"
      in_compared: "[HOW IT APPEARS IN COMPARED WORK]"
      match_level: "Identical | Near-identical | Similar | Superficially similar | Different"
      distinctiveness: "High | Moderate | Low"
      alternative_explanation: "[COULD THERE BE AN INNOCENT EXPLANATION?]"
      
  overall_similarity_level: "Level 1 | Level 2 | Level 3 | Level 4 | Level 5"
  total_distinctive_elements_matching: "[NUMBER OUT OF TOTAL DISTINCTIVE ELEMENTS]"
  
  alternative_explanations:
    independent_creation_possible: "Likely | Possible | Unlikely"
    common_convention_explains: "Yes | Partial | No"
    common_source_possible: "Yes | Possible | No"
    
  chronology:
    original_creation_date: "[DATE — with evidence quality note]"
    compared_work_first_seen: "[DATE]"
    chronology_supports_copying: "Yes | Unclear | No"
    
  analysis_confidence: "High | Moderate | Low | Insufficient evidence"
  recommended_action: "[WHAT TO DO BASED ON THIS ANALYSIS]"
```

---

*→ Next: `ORIGINALITY_CONFIDENCE_ENGINE.md`*  
*→ Full investigation: `../07-YDM-RESPONSE-SYSTEM/INCIDENT_RESPONSE_ENGINE.md`*
