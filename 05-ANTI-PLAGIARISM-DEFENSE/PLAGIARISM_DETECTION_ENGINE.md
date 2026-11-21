# PLAGIARISM DETECTION ENGINE
## YOUR DEAD MEAT — Core Suspected Plagiarism Detection Methodology

---

**Purpose:** Core suspected plagiarism detection methodology and investigation framework.  
**Scope:** All investigation scenarios involving suspected unauthorized copying.  
**Version:** 1.0.0  
**Dependencies:** `CASE_INTAKE_PROTOCOL.md`, `SIMILARITY_ANALYSIS.md`, `FALSE_POSITIVE_PROTECTION.md`  

---

## DETECTION PHILOSOPHY

**YDM does not use the word "plagiarism" lightly.**

Before concluding that plagiarism has occurred, the system must rule out:
1. Independent creation (two people had the same idea)
2. Common source (both drew from the same public inspiration)
3. Generic conventions (the similarity is industry-standard)
4. Fair use or permitted use (the alleged copy is lawfully made)
5. Coincidence (surface similarities without substantive copying)

Only after these are properly assessed should the word "plagiarism" or "infringement" appear in any formal document.

---

## DETECTION WORKFLOW

```
SUSPECTED PLAGIARISM DETECTED
         │
         ▼
STEP 1: INTAKE
  Collect: original work details, suspected copy details
  → CASE_INTAKE_PROTOCOL.md
         │
         ▼
STEP 2: TYPE IDENTIFICATION
  What type of work was allegedly copied?
  ├── Image/Art → IMAGE_COPY_DETECTION.md
  ├── Code → CODE_COPY_DETECTION.md
  ├── Document/Text → DOCUMENT_COPY_DETECTION.md
  ├── 3D Assets → 3D_ASSET_SIMILARITY.md
  └── Brand/Logo → BRAND_IMPERSONATION_DETECTION.md
         │
         ▼
STEP 3: SIMILARITY ANALYSIS
  Apply structured comparison methodology
  → SIMILARITY_ANALYSIS.md
         │
         ▼
STEP 4: FALSE POSITIVE CHECK
  Rule out innocent explanations
  → FALSE_POSITIVE_PROTECTION.md
         │
         ▼
STEP 5: EVIDENCE QUALITY ASSESSMENT
  Rate confidence level
  → ORIGINALITY_CONFIDENCE_ENGINE.md
         │
         ▼
STEP 6: CASE CLASSIFICATION
  Assign case type and severity
  → PLAGIARISM_CASE_CLASSIFICATION.md
         │
         ▼
STEP 7: RECOMMENDED ACTION
  Route to appropriate response
  → ESCALATION_MATRIX.md
```

---

## DETECTION TRIGGERS

### Strong Investigation Triggers
- Highly distinctive elements appear in both works
- The alleged copy appeared after the original was published
- Multiple specific, non-obvious similarities exist
- The alleged infringer had documented access to the original

### Weak Investigation Triggers (Require More Analysis)
- General style similarity
- Same subject matter or genre
- Similar color palette or general aesthetic
- Same function or purpose

---

## INVESTIGATION LIMITATIONS

| Limitation | Impact | Mitigation |
|-----------|--------|-----------|
| Cannot access private accounts | May miss private copies | Focus on publicly accessible evidence |
| Cannot verify original creation independently | Relies on creator's records | Strong internal documentation compensates |
| Cannot determine intent | Intent is irrelevant to copyright infringement, but affects some claims | Note intent as circumstantial factor only |
| AI similarity is harder to assess | AI models train on existing work | Require human expert assessment for AI-related cases |

---

*→ Next: `WEB_SIMILARITY_INVESTIGATION.md`*  
*→ Full response: `../07-YDM-RESPONSE-SYSTEM/INCIDENT_RESPONSE_ENGINE.md`*
