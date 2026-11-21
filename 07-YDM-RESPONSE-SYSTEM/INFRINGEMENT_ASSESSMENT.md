# INFRINGEMENT ASSESSMENT
## YOUR DEAD MEAT — Potential Infringement Indicators Analysis

---

**Purpose:** Assesses potential infringement indicators without making definitive legal judgments.  
**Scope:** All cases escalated from investigation to response consideration.  
**Version:** 1.0.0  
**Dependencies:** `EVIDENCE_COMPARISON_REPORT.md`, `LEGAL_LIMITATIONS.md`, `ESCALATION_MATRIX.md`  

---

## ASSESSMENT FRAMEWORK

An infringement assessment evaluates the evidence to identify whether formal action is justified. It NEVER declares someone guilty. It evaluates indicators.

### Copyright Infringement Indicators

For copyright claims, assess:

1. **Valid copyright:** Does the original work contain protectable expression?
2. **Ownership:** Does the person asserting infringement own or control the rights?
3. **Copying:** Is there evidence the work was copied (not independently created)?
4. **Substantial similarity:** Are the copied elements substantially similar to protectable expression?

### Trademark Infringement Indicators

For trademark claims, assess:

1. **Valid mark:** Is the mark legally protectable (registered, or used in commerce)?
2. **Priority:** Does the asserting party have prior rights?
3. **Likelihood of confusion:** Would consumers be confused about the source?
4. **Same/related goods/services:** Do both marks operate in the same market?

---

## ASSESSMENT RECORD

```yaml
# INFRINGEMENT ASSESSMENT
# Case ID: YDM-CASE-[ID]

infringement_assessment:
  assessment_type: "Copyright | Trademark | Trade Secret | Mixed"
  
  copyright_analysis:
    protectable_expression_exists: "Yes | Partial | No | Uncertain"
    protectable_expression_description: "[WHAT EXPRESSION IS PROTECTABLE]"
    ownership_documented: "Yes | Partially | No"
    access_evidence: "Strong | Moderate | Weak | None"
    copying_indicators:
      strength: "Strong | Moderate | Weak | None"
      basis: "[WHAT INDICATES COPYING]"
    substantial_similarity:
      overall_assessment: "Strong | Moderate | Weak"
      distinctive_elements_match: "[NUMBER] of [TOTAL DOCUMENTED]"
      
  preliminary_assessment:
    indicators_present: "Strong | Moderate | Weak | Absent"
    formal_action_justified: "Yes | Probably | Possibly | No"
    
  critical_caveats:
    - "[LIMITATION 1]"
    - "[LIMITATION 2]"
    
  mandatory_disclaimer: >
    This assessment identifies potential infringement indicators only.
    It is NOT a legal determination. Copyright and trademark infringement
    are legal conclusions that can only be made by a court, or by qualified
    legal counsel advising on a jurisdiction-specific basis.
    Do not take formal legal action based solely on this assessment.
```

---

*→ Next: `CEASE_AND_DESIST_ENGINE.md`*  
*→ Escalation: `ESCALATION_MATRIX.md`*
