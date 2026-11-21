# ORIGINALITY CONFIDENCE ENGINE
## YOUR DEAD MEAT — Evidence Strength, Uncertainty Assessment & Confidence Ratings

---

**Purpose:** Explains and applies confidence levels, evidence strength assessment, and uncertainty disclosure in all YDM outputs.  
**Scope:** All investigation and assessment outputs. This engine governs how certainty is expressed.  
**Version:** 1.0.0  
**Dependencies:** `SIMILARITY_ANALYSIS.md`, `EVIDENCE_VALIDATION.md`  

---

## CONFIDENCE RATING SYSTEM

```
CONFIDENCE LEVEL DEFINITIONS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

🟢 STRONG CONFIDENCE
   Multiple independent evidence sources.
   Distinctive elements match precisely.
   Chronology clearly supports the original claim.
   No plausible innocent explanation remains.
   → Appropriate for formal enforcement correspondence.

🟡 MODERATE CONFIDENCE
   Significant similarity documented.
   Some distinctive elements match.
   Chronology probably supports original claim.
   Independent creation remains theoretically possible.
   → Appropriate for preliminary inquiry; not formal legal action without more evidence.

🟠 LOW CONFIDENCE
   Noticeable similarity exists.
   Similarities may be explained by common conventions.
   Evidence chain has gaps.
   Multiple alternative explanations exist.
   → Appropriate for internal documentation only.
   → NOT appropriate for any formal or public accusation.

🔴 INSUFFICIENT
   Evidence does not support any formal claim.
   Proceeding with accusations would be harmful and unjustified.
   → Document only. No formal action recommended.

⚪ INCONCLUSIVE
   Evidence exists but contradicts itself.
   More investigation is needed before any assessment.
   → Identify what additional evidence would resolve the question.
```

---

## EVIDENCE STRENGTH FACTORS

### Factors That Increase Confidence
- Earlier documented creation date for original work
- Precise matching of distinctive, non-obvious elements
- Multiple independent similarities (not one generic pattern)
- Access: the alleged infringer had means to access original work
- No plausible independent creation pathway
- Prior publication of original work

### Factors That Decrease Confidence
- Generic or common elements are the basis of similarity
- Independent creation is demonstrably possible
- Alleged infringer had no documented access to original
- Original creation date is poorly documented
- Similarities are explained by common conventions in the field
- Original work itself borrowed substantially from others

---

## CONFIDENCE ASSESSMENT TEMPLATE

```yaml
# CONFIDENCE ASSESSMENT
# Case ID: YDM-CASE-[ID]

confidence_assessment:
  
  rating: "Strong | Moderate | Low | Insufficient | Inconclusive"
  rating_symbol: "🟢 | 🟡 | 🟠 | 🔴 | ⚪"
  
  supporting_factors:
    - "[FACTOR THAT INCREASES CONFIDENCE]"
  
  limiting_factors:
    - "[FACTOR THAT DECREASES CONFIDENCE]"
    
  key_uncertainties:
    - "[WHAT IS UNKNOWN THAT COULD CHANGE THIS ASSESSMENT]"
    
  evidence_quality:
    provenance_documentation: "Excellent | Good | Fair | Poor"
    similarity_documentation: "Thorough | Adequate | Limited"
    access_evidence: "Demonstrated | Likely | Unknown"
    chronology_clarity: "Clear | Mostly clear | Ambiguous"
    
  recommended_next_steps:
    if_proceeding: "[WHAT TO DO IF PURSUING THIS CASE]"
    evidence_to_gather: "[WHAT WOULD IMPROVE THE CASE]"
    legal_counsel_recommended: "Yes — immediately | Recommended | Optional"
    
  important_disclaimer: >
    This confidence assessment is based on available documented evidence.
    It is not a legal determination. All formal actions should be reviewed
    by a qualified intellectual property attorney.
```

---

*→ Directory 03 complete. Next: `../04-DIGITAL-PROVENANCE-EVIDENCE/PROVENANCE_ENGINE.md`*
