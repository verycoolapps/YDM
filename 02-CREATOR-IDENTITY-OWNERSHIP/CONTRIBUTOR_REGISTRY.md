# CONTRIBUTOR REGISTRY
## YOUR DEAD MEAT — Contributor Documentation & Contribution Tracking

---

**Purpose:** Records all contributors and their specific contributions to a project.  
**Scope:** All projects with more than one contributor.  
**Version:** 1.0.0  
**Dependencies:** `CREATOR_IDENTITY_ENGINE.md`, `COLLABORATION_OWNERSHIP.md`  

---

## CONTRIBUTOR RECORD TEMPLATE

```yaml
# CONTRIBUTOR REGISTRY
# Project: [NAME] | ID: YDM-[ID]

contributors:
  - contributor_id: "YDM-CONTRIB-[ID]"
    name: "[USER-DECLARED NAME]"
    attribution_preference: "[HOW THEY WANT TO BE CREDITED]"
    contact_reference: "[OPTIONAL — email prefix, username]"
    
    contribution_details:
      contribution_type: >
        Original Creation | Derivative Work | Technical Implementation |
        Editorial | Art Direction | Consultation | Licensing | Other
      contribution_description: "[SPECIFIC DESCRIPTION OF WHAT THEY MADE]"
      contribution_scope: "Major | Moderate | Minor | Incidental"
      contribution_dates:
        start: "[DATE]"
        end: "[DATE OR 'Ongoing']"
        
    work_product:
      deliverables: "[LIST OF FILES/ELEMENTS THEY CREATED]"
      format: "[FILE TYPES — e.g., .psd, .py, .blend]"
      version_delivered: "[VERSION NUMBER WHEN DELIVERED]"
      
    ownership_arrangement:
      arrangement_type: >
        Work-for-Hire | License Grant | Joint Ownership |
        Rights Retained by Contributor | Assignment | Other
      arrangement_documented: "Yes — reference: [DOC NAME] | No | Verbal"
      compensation_basis: "Paid | Unpaid | Revenue Share | Other"
      rights_transferred: "[WHAT RIGHTS WERE TRANSFERRED IF ANY]"
      
    declaration:
      contributor_acknowledged: "Yes | No | Not Requested"
      attribution_agreed: "Yes | No | Disputed"
      date_documented: "[DATE]"
```

---

## CONTRIBUTION TRACKING LOG

For ongoing projects, maintain a running log:

```
CONTRIBUTION LOG — [PROJECT NAME] — [YDM-ID]
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

[DATE] | [CONTRIBUTOR NAME] | [WHAT THEY CONTRIBUTED]
       | Scope: [Major/Moderate/Minor] | Rights: [Arrangement]

[DATE] | [CONTRIBUTOR NAME] | [WHAT THEY CONTRIBUTED]
       | Scope: [Major/Moderate/Minor] | Rights: [Arrangement]
```

---

## CONTRIBUTION OWNERSHIP RULES

### Work-for-Hire Contributors
If a contributor was paid and there's a written work-for-hire agreement:
- Their contribution may be owned by the commissioning party
- Document: agreement reference, payment record, delivery confirmation

### Licensed Contributors
If a contributor provided elements under a license:
- Document: license type, usage terms, attribution requirements
- Note: licensed elements are NOT owned by the project owner

### Uncredited Contributors (Anonymized)
Some contributions may need to be documented without public attribution:
- Record: contribution type and scope
- Note: "[CONTRIBUTOR IDENTITY WITHHELD BY REQUEST]"
- Anonymized records still have evidentiary value

### AI as "Contributor"
If AI tools generated specific elements:
- Document: AI model, general prompt intent, output description
- Note: AI is a tool, not a legal contributor with rights
- Human direction of AI still represents creative contribution
- Route to: `AI_GENERATION_DISCLOSURE.md`

---

## CONTRIBUTOR ATTRIBUTION STANDARDS

Default attribution line for credits:

```
[ELEMENT/ROLE]: [CONTRIBUTOR NAME]
```

Example credits block:
```
ORIGINAL CONCEPT & DIRECTION: [CREATOR NAME]
CHARACTER DESIGN: [CONTRIBUTOR A]
MUSIC COMPOSITION: [CONTRIBUTOR B]
ADDITIONAL CODE: [CONTRIBUTOR C]
3D MODELING: [CONTRIBUTOR D]
```

---

*→ Next: `AUTHORSHIP_DECLARATION.md`*  
*→ Collaboration ownership: `COLLABORATION_OWNERSHIP.md`*
