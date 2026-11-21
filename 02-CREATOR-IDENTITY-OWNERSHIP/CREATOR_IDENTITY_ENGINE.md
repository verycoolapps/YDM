# CREATOR IDENTITY ENGINE
## YOUR DEAD MEAT — Creator Identity Declaration & Attribution Management

---

**Purpose:** Manages creator identity declaration, attribution records, and identity verification workflows.  
**Scope:** All projects. Creator identity is the foundation of every protection record.  
**Version:** 1.0.0  
**Dependencies:** `PRE_CREATION_GATE.md`, `ATTRIBUTION_ENGINE.md`  

---

## THE CREATOR IDENTITY RECORD

The Creator Identity Record (CIR) is the most foundational document in the YDM system. Everything else builds on it.

```yaml
# CREATOR IDENTITY RECORD
# YOUR DEAD MEAT — Creator Identity Engine
# ══════════════════════════════════════════

creator_identity_record:
  
  # UNIQUE IDENTIFIERS
  creator_id: "YDM-CR-[AUTO: YYYY-MM-DD-XXXX]"
  associated_project_ids: []
  
  # IDENTITY INFORMATION (All fields: USER-DECLARED unless otherwise noted)
  creator_name:
    legal_name: "[FULL LEGAL NAME — USER-DECLARED]"
    professional_name: "[STAGE/STUDIO/PEN NAME IF DIFFERENT]"
    attribution_preference: "[HOW THEY WANT TO BE CREDITED]"
    
  contact_reference:
    # NOTE: Store only what's needed for record context.
    # Do not store sensitive personal information in creation records.
    identifier_type: "Email prefix | Username | Organization | Other"
    identifier_value: "[REFERENCE ONLY — not for surveillance]"
    
  professional_context:
    organization: "[COMPANY/STUDIO/INSTITUTION — if applicable]"
    role_title: "[JOB TITLE — if relevant to ownership]"
    employment_relationship: >
      Employed full-time | Employed part-time | Freelance contractor |
      Self-employed | Student | Personal project | Other
      
  # CREATIVE PROFILE
  creative_disciplines:
    - "[PRIMARY DISCIPLINE]"
    - "[SECONDARY DISCIPLINE IF ANY]"
  experience_level: "Emerging | Professional | Established | Expert"
  public_portfolio: "[URL IF USER CHOOSES TO PROVIDE]"
  
  # DECLARATION
  declaration:
    statement: >
      I declare that I am the original creator of the works
      associated with this identity record. The information
      provided is accurate to the best of my knowledge.
    declared_date: "[ISO 8601]"
    declaration_status: "USER-DECLARED — Not independently verified"
    
  # VERIFICATION STATUS
  verification:
    status: "Unverified | Partially Verified | Verified"
    verification_method: "[If verified: how was identity confirmed?]"
    verification_date: "[If verified: when?]"
    verifying_party: "[If verified: who or what confirmed?]"
```

---

## IDENTITY COLLECTION DIALOGUE

### Standard Dialogue Flow

```
YDM: "Let's establish your creator identity for this project.

What is your full name as the creator?
(This is for your internal records — it won't be shared without your control)"

USER: "[Provides name]"

YDM: "How would you like to be credited publicly?
(This may be your real name, a studio name, a pen name, or a pseudonym)"

USER: "[Provides preferred credit]"

YDM: "Is this project for yourself personally, or for an organization
or client?"

USER: "[Answers]"

YDM: "[If for organization] What is the organization's name, and
what is your role within it?"

[After collecting]:
YDM: "Creator identity established. Your record:

Creator: [NAME] (declared)
Attribution: [PUBLIC CREDIT]
Owner: [OWNER]
Creator ID: YDM-CR-[ID]

This information is stored in your project's protection record."
```

---

## MULTIPLE CREATOR SCENARIOS

### Scenario: Solo Creator
Most common. Creator = Owner. Attribution is straightforward.

### Scenario: Work for Client
Creator is the maker. Owner may be the client depending on contract.
→ Route to `CONTRACTUAL_RIGHTS.md` for ownership determination.

### Scenario: Employment
Creator is the employee. Owner may be the employer (work-made-for-hire).
→ Note potential employer ownership. Recommend reviewing employment agreement.
→ Route to `ORGANIZATION_OWNERSHIP.md`.

### Scenario: Collaboration
Multiple creators. Ownership must be explicitly negotiated.
→ Route to `COLLABORATION_OWNERSHIP.md`.

### Scenario: AI-Assisted Creation
Human creator + AI generator. 
→ Note AI contribution explicitly.
→ Route to `AI_GENERATION_DISCLOSURE.md` for proper documentation.
→ Note that copyright protection for AI-generated elements may be limited in some jurisdictions.

---

## ATTRIBUTION FORMAT STANDARDS

Standard attribution format for embedding in project deliverables:

```
© [YEAR] [ATTRIBUTION NAME] — All Rights Reserved
YDM Project ID: [YDM-XXXXXXXX]
Created: [DATE]
Protected under: YOUR DEAD MEAT IP Defense System
```

Minimal attribution (for tight spaces):
```
© [YEAR] [NAME] | YDM-[ID]
```

---

*→ Next: `OWNER_VERIFICATION_ENGINE.md`*  
*→ Back: `../01-CORE-INTELLIGENCE/QUALITY_CONTROL.md`*
