# BRAND IMPERSONATION DETECTION
## YOUR DEAD MEAT — BRAND IMPERSONATION DETECTION Module

---

**Purpose:** Identifies potential unauthorized brand identity usage.  
**Scope:** Specialized detection for this asset type.  
**Version:** 1.0.0  
**Dependencies:** `PLAGIARISM_DETECTION_ENGINE.md`, `SIMILARITY_ANALYSIS.md`, `FALSE_POSITIVE_PROTECTION.md`  

---

## BRAND IMPERSONATION DETECTION

### Brand Similarity Framework

Brand IP involves trademark law, which uses a **"likelihood of confusion"** standard. Key factors:

1. **Mark similarity** — How similar are the marks visually, phonetically, conceptually?
2. **Goods/services similarity** — Are both marks used in the same industry?
3. **Market channel** — Do they reach the same consumers?
4. **Consumer sophistication** — Would typical consumers be confused?
5. **Mark strength** — Is the original mark well-known?

### Visual Brand Comparison

```
BRAND COMPARISON CHECKLIST
━━━━━━━━━━━━━━━━━━━━━━━━━━

□ Logo visual comparison (shape, symbol, composition)
□ Color system comparison (primary brand colors)
□ Typography comparison (fonts, weight, spacing)
□ Name/wordmark comparison (spelling, phonetic similarity)
□ Tagline comparison
□ Overall visual language and system
□ Industry/market overlap
□ Target audience overlap
□ Domain name similarity
□ Social media handle similarity
```

### Brand Comparison Record

```yaml
brand_comparison:
  original_brand:
    name: "[BRAND NAME]"
    registration_status: "Registered — [JURISDICTION] | Unregistered"
    registration_number: "[IF REGISTERED]"
    primary_industries: "[LIST]"
    distinctive_elements:
      - "[SPECIFIC BRAND ELEMENT]"
      
  suspected_copy:
    name: "[OTHER BRAND NAME]"
    location: "[WHERE FOUND]"
    industry: "[THEIR INDUSTRY]"
    similarity_elements:
      - element: "[WHAT IS SIMILAR]"
        similarity_level: "Identical | Very similar | Similar | Somewhat similar"
        
  confusion_analysis:
    visual_confusion_risk: "High | Moderate | Low"
    market_overlap: "Yes | Partial | No"
    consumer_confusion_likely: "Yes | Possible | Unlikely"
    
  trademark_search_done: "Yes | No"
  recommendation: "[WHAT TO DO]"
```

---
