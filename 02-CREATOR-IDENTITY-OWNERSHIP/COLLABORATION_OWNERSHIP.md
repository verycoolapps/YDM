# COLLABORATION OWNERSHIP
## YOUR DEAD MEAT — Joint Creation & Collaborative Ownership Documentation

---

**Purpose:** Documents joint creation, collaborative ownership arrangements, and multi-creator rights structures.  
**Scope:** All projects with two or more contributing creators.  
**Version:** 1.0.0  
**Dependencies:** `CONTRIBUTOR_REGISTRY.md`, `RIGHTS_HOLDER_MANAGEMENT.md`  

---

## COLLABORATION OWNERSHIP PRINCIPLES

### Default Rule (Most Jurisdictions)
In the absence of a written agreement, joint creators generally hold equal undivided shares in a jointly created work. This means each co-creator may independently exercise their ownership rights, though specific rules vary by jurisdiction.

**This default is often undesirable.** It is strongly recommended that collaborators document their arrangement explicitly before creation begins.

### YDM Collaboration Protocol
1. Identify all contributing parties before work begins
2. Document each party's intended contributions
3. Record any existing written collaboration agreement
4. If no agreement exists, flag this as a documentation gap
5. Recommend that parties formalize their arrangement before significant investment

---

## COLLABORATION RECORD TEMPLATE

```yaml
# COLLABORATION OWNERSHIP RECORD
# Project ID: YDM-[ID]

collaboration_record:
  project_id: "YDM-[ID]"
  collaboration_type: >
    Equal Joint | Unequal Joint | Lead + Contributor |
    Employer-Employee | Contractor | Open Source | Other
    
  parties:
    - party_id: "YDM-CR-[ID]"
      name: "[USER-DECLARED]"
      role: "Lead Creator | Co-Creator | Contributor | Art Director | Producer"
      creative_contributions:
        - "[ELEMENT/ASPECT THEY CREATED]"
      ownership_share_claimed: "[% OR 'Equal' OR 'None — work-for-hire']"
      rights_arrangement: "[WHAT RIGHTS DO THEY HOLD OR TRANSFER]"
      
  agreement_status:
    written_agreement_exists: "Yes | No | In Progress"
    agreement_reference: "[NAME/DATE OF AGREEMENT IF EXISTS]"
    agreement_covers:
      - "Ownership shares: [YES/NO]"
      - "Credit/attribution: [YES/NO]"
      - "Revenue sharing: [YES/NO]"
      - "Moral rights: [YES/NO]"
      - "Dispute resolution: [YES/NO]"
      - "Project discontinuation: [YES/NO]"
      
  documentation_gap:
    has_gaps: "Yes | No"
    gap_description: "[WHAT IS NOT DOCUMENTED]"
    recommended_action: "[WHAT SHOULD BE DONE]"
```

---

## COLLABORATION DIALOGUE

When collaboration is detected:

```
YDM: "This is a collaborative project with [N] contributors.
Collaborative ownership requires careful documentation.

Questions:
1. Is there a written collaboration or co-creation agreement?
2. How is ownership divided between contributors?
3. Who will be the primary rights holder for enforcement purposes?
4. Are all contributors aware of and agreeable to the ownership arrangement?

Important: Without a written agreement, most jurisdictions default to
equal joint ownership, which may not reflect the parties' actual intent.
I recommend formalizing your arrangement before significant work is invested."
```

---

## OPEN SOURCE / COMMUNITY PROJECTS

For open source or community collaborative projects:

```yaml
open_source_collaboration:
  license: "[MIT | Apache 2.0 | GPL 3.0 | Creative Commons — specify]"
  contribution_model: "[Pull Request | Invitation Only | Open | Other]"
  contributor_license_agreement: "Required | Not Required | In Progress"
  primary_maintainer: "[USER-DECLARED]"
  governance_model: "[BDFL | Committee | Democratic | Other]"
```

---

*→ Next: `ORGANIZATION_OWNERSHIP.md`*  
*→ Contributor details: `CONTRIBUTOR_REGISTRY.md`*
