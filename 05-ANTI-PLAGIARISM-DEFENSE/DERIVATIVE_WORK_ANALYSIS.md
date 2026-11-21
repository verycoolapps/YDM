# DERIVATIVE WORK ANALYSIS
## YOUR DEAD MEAT — DERIVATIVE WORK ANALYSIS Module

---

**Purpose:** Examines potentially derivative creative works and fair use considerations.  
**Scope:** Specialized detection for this asset type.  
**Version:** 1.0.0  
**Dependencies:** `PLAGIARISM_DETECTION_ENGINE.md`, `SIMILARITY_ANALYSIS.md`, `FALSE_POSITIVE_PROTECTION.md`  

---

## DERIVATIVE WORK ANALYSIS

A derivative work is based on one or more pre-existing works. Creating an unauthorized derivative can infringe the original work's copyright. Creating an authorized derivative requires permission.

### Derivative Work Types

| Type | Description | Generally Requires Permission |
|------|-------------|------------------------------|
| Translation | Work translated to another language | Yes |
| Adaptation | Story adapted to film, game, etc. | Yes |
| Transformation | Work substantially transformed (may be fair use) | Depends on jurisdiction and use |
| Commentary | Commentary using portions of original work | Often fair use/fair dealing |
| Parody | Parody of original work (may qualify for fair use) | Often fair use in US |
| Fan work | Based on original characters/world | Often tolerated but technically requires permission |

### Fair Use / Fair Dealing Analysis

**U.S. Fair Use Factors (17 U.S.C. § 107):**
1. Purpose and character of use (commercial vs. educational, transformative vs. reproductive)
2. Nature of the copyrighted work (factual vs. creative)
3. Amount and substantiality of portion used
4. Effect on the market for the original

**Note:** Fair use is a legal defense. YDM cannot determine if a use qualifies. Consult a qualified IP attorney.

### Derivative Work Assessment Record

```yaml
derivative_work_assessment:
  original_work: "[WORK THAT MAY HAVE BEEN ADAPTED]"
  suspected_derivative: "[WORK THAT MAY BE DERIVATIVE]"
  
  relationship_analysis:
    is_based_on_original: "Clearly | Probably | Possibly | Unclear | No"
    transformation_level: "High | Moderate | Low | None"
    creative_contribution: "Substantial | Moderate | Minimal | None"
    
  permission_status:
    permission_obtained: "Yes | No | Unknown"
    license_basis: "[IF ANY — e.g., Creative Commons license]"
    
  fair_use_factors:
    commercial_purpose: "Yes | No"
    transformative: "High | Moderate | Low"
    amount_used: "Minimal | Moderate | Substantial | Complete"
    market_harm_likely: "Yes | Possibly | No"
    
  assessment: "Likely unauthorized | May be authorized | Cannot determine"
  recommendation: "[WHAT TO DO]"
  legal_counsel_required: "Yes | Recommended"
```

---
