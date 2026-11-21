# OWNERSHIP DISPUTE PROTOCOL
## YOUR DEAD MEAT — Conflicting & Disputed Ownership Claim Handling

---

**Purpose:** Handles conflicting or disputed ownership claims between parties.  
**Scope:** All situations where ownership is contested or unclear between two or more parties.  
**Version:** 1.0.0  
**Dependencies:** `OWNER_VERIFICATION_ENGINE.md`, `COLLABORATION_OWNERSHIP.md`, `LEGAL_COUNSEL_ESCALATION.md`  

---

## DISPUTE TYPES

| Type | Description | Typical Cause |
|------|-------------|--------------|
| Collaboration Dispute | Co-creators disagree on shares or attribution | No written agreement |
| Client-Creator Dispute | Creator and client disagree on who owns | No clear assignment clause |
| Employer-Employee Dispute | Employee claims personal ownership of work-for-hire | Unclear employment scope |
| Inheritance/Succession Dispute | Heirs disagree on inherited IP rights | No estate planning |
| Joint Venture Dispute | Business partners disagree on project IP | No partnership agreement |
| Contractor Dispute | Freelancer and client dispute rights | No written assignment |

---

## DISPUTE INTAKE RECORD

```yaml
# OWNERSHIP DISPUTE RECORD
# ID: YDM-DISPUTE-[ID]

dispute_record:
  dispute_id: "YDM-DISPUTE-[AUTO]"
  project_id: "YDM-[ID]"
  dispute_date: "[DATE DISPUTE IDENTIFIED]"
  
  parties:
    - party_name: "[USER'S NAME]"
      claim_basis: "[BASIS FOR THEIR CLAIM]"
      supporting_evidence: "[WHAT EVIDENCE DO THEY HAVE]"
      
    - party_name: "[OTHER PARTY — if known]"
      claim_basis: "[THEIR BASIS — if known]"
      known_evidence: "[WHAT EVIDENCE DO THEY APPEAR TO HAVE]"
      
  dispute_nature:
    type: "[FROM DISPUTE TYPES ABOVE]"
    primary_issue: "[CORE DISAGREEMENT IN ONE SENTENCE]"
    affected_rights: "[WHICH SPECIFIC RIGHTS ARE DISPUTED]"
    
  documentation_status:
    written_agreement_exists: "Yes | No | Unknown"
    agreement_addresses_dispute: "Yes | No | Partially | Unknown"
    registration_exists: "Yes | No | Unknown"
    
  resolution_status: "Unresolved | In Negotiation | Mediation | Litigation | Resolved"
  
  ydm_position:
    can_resolve: "Yes | No — requires legal counsel"
    recommendation: "[WHAT YDM RECOMMENDS]"
    legal_counsel_required: "Yes | Recommended | Optional"
```

---

## DISPUTE RESOLUTION PATHWAY

```
DISPUTE DETECTED
      │
      ▼
STEP 1: Identify and document the nature of the dispute
      │
      ▼
STEP 2: Collect evidence from the YDM-using party
      │
      ▼
STEP 3: Note what evidence the other party may have
      │
      ▼
STEP 4: Check if any written agreement addresses this
      │
      ├── YES: Review agreement, determine applicable terms
      │
      └── NO: Flag as documentation gap
      │
      ▼
STEP 5: Assess evidence strength for the YDM-using party
      │
      ▼
STEP 6: Recommend resolution pathway:
        
        LOW EVIDENCE: Document carefully, seek negotiation
        MODERATE EVIDENCE: Negotiate or seek mediation
        STRONG EVIDENCE: Formal demand, potential litigation
        COMPLEX: Recommend legal counsel immediately
```

---

## YDM POSITION ON DISPUTES

**IMPORTANT:** YOUR DEAD MEAT is a documentation tool. It cannot:
- Determine legal ownership in a dispute
- Issue binding rulings
- Replace a court, arbitrator, or mediator
- Advise on litigation strategy

What YDM CAN do:
- Document the user's position and evidence
- Identify documentation gaps that weaken their position
- Suggest what documentation would strengthen their position
- Prepare correspondence for professional review
- Recommend when to seek qualified legal counsel

**When to immediately recommend legal counsel:**
- Dispute involves significant financial value
- Other party has taken or threatens legal action
- Employment or business relationship is affected
- Formal legal proceedings have been initiated
- The user is accused of infringement (not just disputing ownership)

---

*→ Directory 02 complete. Next: `../03-ORIGINALITY-INTELLIGENCE/ORIGINALITY_ENGINE.md`*  
*→ Legal escalation: `../06-LEGAL-RIGHTS-INTELLIGENCE/LEGAL_COUNSEL_ESCALATION.md`*
