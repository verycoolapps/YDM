# PRE-CREATION GATE
## YOUR DEAD MEAT — Mandatory 6-Stage Pre-Creation Protection Workflow

---

**Purpose:** Defines the mandatory pre-creation protection workflow that must execute before any creative work begins.  
**Scope:** All Mode A (Full Protection) activations. Abbreviated version for Mode B.  
**Version:** 1.0.0  
**Dependencies:** `CREATOR_IDENTITY_ENGINE.md`, `PROVENANCE_ENGINE.md`, `ORIGINALITY_ENGINE.md`, `AUTHORSHIP_DECLARATION.md`  

---

## GATE PHILOSOPHY

The Pre-Creation Gate exists because **documentation created before and during a project is exponentially more credible than documentation created after a dispute arises.**

A creator who can show:
- Their initial concept notes
- Their creation timeline
- Their tool and process records
- Their version history from day one

...is in a vastly stronger position than one who tries to reconstruct evidence after the fact.

**The gate takes minutes. It protects for years.**

---

## STAGE 1 — CREATOR IDENTIFICATION

### Objective
Establish who made this work and who holds the relevant rights.

### Questions to Ask

```
1. What is your full name? (as the creator/author)
2. How would you like to be credited publicly?
   (This may differ from your legal name)
3. Is this for yourself personally, or for an organization?
4. If for an organization: what is the entity name?
5. Are there any other contributors or collaborators?
6. Who is the rights holder / owner of this project?
   (If different from creator — e.g., client, employer, company)
```

### Record Format

```yaml
# STAGE 1 OUTPUT — CREATOR IDENTIFICATION
# STATUS: [USER-DECLARED — Not independently verified]

stage_1_creator_identification:
  creator_full_name: "[USER-DECLARED]"
  public_attribution_credit: "[USER-DECLARED]"
  creator_type: "Individual | Organization | Collaborative"
  organization_name: "[IF APPLICABLE]"
  collaborators:
    - name: "[COLLABORATOR NAME IF ANY]"
      role: "[THEIR SPECIFIC CONTRIBUTION]"
      rights_arrangement: "[USER-DECLARED ARRANGEMENT]"
  rights_holder: "[USER-DECLARED]"
  rights_holder_relationship: "Same as creator | Employer | Client | Joint | Other"
  
  declaration: >
    Creator information above is USER-DECLARED as of [DATE].
    This record does not constitute legal proof of authorship
    or ownership. Independent verification is recommended
    for formal legal purposes.
```

### Stage 1 Completion Criteria
- [ ] At least one creator name provided
- [ ] Public attribution preference noted
- [ ] Rights holder / owner identified (even if "same as creator")
- [ ] Collaboration arrangements noted if applicable

---

## STAGE 2 — PROJECT REGISTRATION

### Objective
Generate a unique, documented project identity.

### YDM Project ID Generation

Format: `YDM-[8-character hexadecimal]`

Generation algorithm:
1. Take current timestamp (Unix epoch, milliseconds)
2. Add project name string (first 8 characters, normalized)
3. Apply SHA-256, take first 8 hex characters
4. Prefix with `YDM-`

Example: `YDM-4A7F2E91`

**Note:** The YDM Project ID is an internal reference identifier. It is not a registered trademark, copyright registration number, or government-issued identifier. Its value is as an internal tracking reference.

### Record Format

```yaml
# STAGE 2 OUTPUT — PROJECT REGISTRATION

stage_2_project_registration:
  project_id: "YDM-[8-CHAR-HEX]"
  project_title: "[PROJECT NAME]"
  project_category: >
    Software | Game | Digital Art | 3D Model | Brand Identity |
    Written Work | Architectural | Business Framework | 
    Multimedia | Research | Other
  project_subcategory: "[SPECIFIC TYPE — e.g., 'Mobile App', 'Logo System']"
  project_description: "[1-3 sentence description of what this project is]"
  initial_creation_timestamp: "[ISO 8601 — YYYY-MM-DDTHH:MM:SSZ]"
  version: "1.0.0"
  protection_classification: "Standard | Elevated | Critical"
  
  creator_declaration: >
    I declare that I am the original creator of this project
    as described, and that the information provided is accurate
    to the best of my knowledge. I understand this record is
    not a substitute for formal copyright registration.
  
  declared_by: "[CREATOR NAME]"
  declaration_date: "[ISO 8601 DATE]"
```

### Protection Classification Guide

| Classification | Use When |
|---------------|---------|
| Standard | Personal projects, low commercial value, exploratory work |
| Elevated | Commercial projects, significant creative investment, potential public release |
| Critical | High-value IP, commercial products, work likely to attract copying |

---

## STAGE 3 — ORIGINALITY BASELINE

### Objective
Document the original creative contribution before it is mixed with executed work. This creates a "before" record that is critical for future comparison.

### Questions to Establish

```
1. What is the central creative concept of this project?
   (In your own words — what makes it yours?)
2. What distinctive visual, functional, or conceptual characteristics 
   does this project have?
3. What is the intended creative direction?
4. What pre-existing elements, templates, or frameworks are you 
   building upon?
5. Are you using any third-party assets, libraries, fonts, 
   stock elements, or references?
6. Where did your inspiration come from? (Sources, mood boards, 
   references — honesty here strengthens your position)
7. Are there any other works that may appear similar due to 
   common conventions in this discipline?
```

### Record Format

```yaml
# STAGE 3 OUTPUT — ORIGINALITY BASELINE
# This is a creative declaration, not a legal patent application.

stage_3_originality_baseline:
  central_creative_concept: "[USER-DESCRIBED IN THEIR OWN WORDS]"
  distinctive_characteristics:
    - "[CHARACTERISTIC 1]"
    - "[CHARACTERISTIC 2]"
    - "[CHARACTERISTIC 3]"
  intended_creative_direction: "[BRIEF DESCRIPTION]"
  pre_existing_elements:
    - element: "[NAME]"
      type: "Template | Framework | Library | Style Influence"
      license: "[LICENSE TYPE IF KNOWN]"
  third_party_assets:
    - asset: "[ASSET NAME/DESCRIPTION]"
      source: "[WHERE OBTAINED]"
      license: "[LICENSE TYPE]"
      attribution_required: "Yes | No | Unknown"
  inspiration_sources:
    - "[SOURCE 1]"
    - "[SOURCE 2]"
  similar_works_awareness:
    - work: "[SIMILAR WORK IF KNOWN]"
      relationship: "Inspiration | Coincidental | Common Convention"
  
  originality_note: >
    This baseline records the creative intent before execution.
    Not all described elements may receive copyright protection —
    ideas, methods, and common design patterns may not be protectable.
    Original expression of these elements is what copyright protects.
```

---

## STAGE 4 — CREATION PROTECTION (During-Creation Protocol)

### Objective
Establish a protocol for documenting the creative process as it happens.

### During-Creation Checklist

```
ACTIVE CREATION PROTECTION PROTOCOL
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

□ Maintain a creation log (even brief notes with timestamps)
□ Save version snapshots at meaningful milestones
□ Record significant creative decisions in writing
□ Document any AI-assisted generation with model/prompt details
□ Preserve source files, not just exported outputs
□ Record tool and software versions used
□ Screenshot or export intermediate states for key assets
□ Note any third-party assets added during development
□ Record any references consulted during creation
□ Commit to version control with meaningful commit messages (for code)
```

### Creation Log Template

```
CREATION LOG — [PROJECT NAME] — [DATE]
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

[HH:MM] — [What was created/decided/modified]
[HH:MM] — [Next milestone]
[HH:MM] — [Significant decision: WHY this direction was chosen]

TOOLS USED TODAY: [Tool name v.X.X]
AI ASSISTANCE TODAY: [None | Model name — describe what was generated]
SOURCE FILES SAVED: [Yes/No — location]
VERSION SNAPSHOT: [v1.0.X — description]
```

---

## STAGE 5 — OWNERSHIP DECLARATION

### Objective
Generate a formal ownership declaration that can be attached to all project deliverables.

### Record Format

```yaml
# STAGE 5 OUTPUT — OWNERSHIP DECLARATION
# ══════════════════════════════════════════════════════════
# YOUR DEAD MEAT — PROJECT OWNERSHIP DECLARATION
# ══════════════════════════════════════════════════════════

PROJECT:            "[PROJECT NAME]"
PROJECT ID:         "YDM-[8-CHAR-HEX]"
PROJECT CATEGORY:   "[CATEGORY]"

ORIGINAL CREATOR:   "[USER-DECLARED NAME]"
                    STATUS: USER-DECLARED — Not independently verified

RIGHTS HOLDER:      "[DECLARED RIGHTS HOLDER]"
                    STATUS: USER-DECLARED

CREATION RECORD:    "[ISO 8601 TIMESTAMP]"
                    SOURCE: User declaration

VERSION:            "[VERSION NUMBER]"

CONTRIBUTORS:       "[LIST OR 'None declared']"

AI CONTRIBUTION:    "[None | Partial — describe | Significant — describe]"
                    NOTE: AI-assisted works may face additional legal
                    scrutiny regarding copyright ownership in some
                    jurisdictions. Consult a qualified IP lawyer.

THIRD-PARTY ASSETS: "[List or 'None declared']"

PROTECTION STATUS:  "[Standard | Elevated | Critical]"
RIGHTS STATUS:      "Declared"
VERIFICATION:       "Unverified — Self-declaration only"

IMPORTANT NOTICE:
This declaration is a user-generated record created with the
YOUR DEAD MEAT IP Defense System. It is NOT a copyright
registration certificate, trademark registration, or legally
binding document establishing ownership in any jurisdiction.
For formal legal protection, consult a qualified intellectual
property attorney and register with appropriate government
authorities in your jurisdiction.
```

---

## STAGE 6 — FINAL PROTECTION REVIEW

### Objective
Perform a pre-delivery audit to ensure the protection package is complete.

### Review Checklist

```
FINAL PROTECTION REVIEW
━━━━━━━━━━━━━━━━━━━━━━━

ATTRIBUTION
  □ Creator name documented
  □ Public attribution preference noted
  □ Rights holder identified
  □ Contributor list complete

OWNERSHIP
  □ Ownership arrangement documented
  □ Work-for-hire considerations noted
  □ Collaboration agreements referenced (if applicable)

THIRD-PARTY ASSETS
  □ All third-party assets listed
  □ License type for each asset noted
  □ Attribution requirements identified
  □ License restrictions checked

PROVENANCE
  □ YDM Project ID assigned
  □ Creation timestamp recorded
  □ Version history initiated
  □ Source files preserved

ORIGINALITY
  □ Creative concept documented
  □ Distinctive characteristics noted
  □ AI contribution disclosed (if any)
  □ Reference sources documented

DOCUMENTATION
  □ Ownership declaration generated
  □ Creator certificate generated (if requested)
  □ Protection strategy documented

GAPS
  □ Any missing critical information flagged
  □ User notified of documentation limitations
```

### Gate Completion Notice

```
╔══════════════════════════════════════════════════════════╗
║  YOUR DEAD MEAT — PRE-CREATION GATE COMPLETE             ║
║                                                          ║
║  Project ID: YDM-[ID]                                    ║
║  Creator: [NAME]                                         ║
║  Protection: [CLASSIFICATION]                            ║
║  Status: 🟢 PROTECTED — Ready to Create                  ║
║                                                          ║
║  Documentation package initialized.                      ║
║  Proceeding with creation task.                          ║
╚══════════════════════════════════════════════════════════╝
```

---

*→ Next: `GLOBAL_RULES.md`*  
*→ Creator identity details: `../02-CREATOR-IDENTITY-OWNERSHIP/CREATOR_IDENTITY_ENGINE.md`*  
*→ Provenance details: `../04-DIGITAL-PROVENANCE-EVIDENCE/PROVENANCE_ENGINE.md`*
