# RIGHTS HOLDER MANAGEMENT
## YOUR DEAD MEAT — Rights Distinction, Licensing & Usage Rights

---

**Purpose:** Distinguishes ownership, licensing, and usage rights; manages complex rights structures.  
**Scope:** All projects with rights complexity — multiple rights holders, licenses, assignments.  
**Version:** 1.0.0  
**Dependencies:** `OWNER_VERIFICATION_ENGINE.md`, `LICENSING_ENGINE.md`  

---

## RIGHTS TAXONOMY

Intellectual property rights are not monolithic. A single work can have multiple rights, held by different parties:

### Economic Rights (Transferable in most jurisdictions)
| Right | Description |
|-------|-------------|
| Reproduction right | Right to copy and duplicate the work |
| Distribution right | Right to sell, rent, lend copies |
| Public display right | Right to show the work publicly |
| Public performance right | Right to perform/broadcast the work |
| Derivative works right | Right to create adaptations, translations, remixes |
| Digital transmission right | Right to transmit online |

### Moral Rights (Non-transferable in many jurisdictions)
| Right | Description |
|-------|-------------|
| Attribution right | Right to be identified as the author |
| Integrity right | Right to object to derogatory treatment |
| Disclosure right | Right to decide when work is published |
| Withdrawal right | Right to withdraw published work (some jurisdictions) |

---

## RIGHTS HOLDER RECORD

```yaml
# RIGHTS HOLDER MANAGEMENT RECORD
# Project ID: YDM-[ID]

rights_structure:
  
  primary_rights_holder:
    name: "[USER-DECLARED]"
    rights_held:
      reproduction: "Full | Partial | None | Unclear"
      distribution: "Full | Partial | None | Unclear"
      display: "Full | Partial | None | Unclear"
      derivative_works: "Full | Partial | None | Unclear"
      digital_transmission: "Full | Partial | None | Unclear"
    moral_rights:
      attribution_right: "Retained | Waived | Transferred | Unknown"
      integrity_right: "Retained | Waived | Unknown"
      
  secondary_rights_holders:
    - name: "[IF ANY]"
      rights_held: "[SPECIFIC RIGHTS]"
      basis: "[CONTRACT/AGREEMENT/LAW]"
      
  licensed_uses:
    - licensee: "[WHO HAS A LICENSE]"
      license_type: "Exclusive | Non-exclusive | Sublicensable"
      licensed_rights: "[WHICH RIGHTS ARE LICENSED]"
      license_territory: "[GEOGRAPHIC SCOPE]"
      license_duration: "[TERM OR 'Perpetual']"
      license_reference: "[CONTRACT/AGREEMENT NAME]"
      
  third_party_rights_in_project:
    - asset: "[ASSET USING THIRD-PARTY CONTENT]"
      rights_holder: "[ORIGINAL OWNER]"
      license_basis: "[HOW IT'S LICENSED INTO THIS PROJECT]"
      attribution_required: "Yes | No"
      usage_restrictions: "[ANY RESTRICTIONS]"
```

---

## RIGHTS MANAGEMENT ALERTS

Trigger alerts when:

| Situation | Alert Level | Action |
|-----------|------------|--------|
| No written agreement for client work | 🟡 WARNING | Note that copyright may remain with creator by default in many jurisdictions |
| Employee creation without clear HR/IP policy | 🟡 WARNING | Recommend reviewing employment agreement |
| Exclusive license granted to multiple parties | 🔴 CRITICAL | Flag as potential conflict — exclusive licenses cannot be granted twice |
| Third-party asset with no documented license | 🟡 WARNING | Document as "license unconfirmed — verify before publication" |
| AI-generated content with unclear rights | 🟡 WARNING | Note jurisdiction-specific uncertainty |

---

## RIGHTS CONFLICT DETECTION

When rights appear to conflict:

```
RIGHTS CONFLICT ANALYSIS
━━━━━━━━━━━━━━━━━━━━━━━━━

Conflict Type: [DESCRIBE THE CONFLICT]
Party A Claim: [WHAT THEY CLAIM]
Party B Claim: [WHAT THEY CLAIM]
Applicable Law: [JURISDICTION — if known]
Evidence Supporting A: [EVIDENCE]
Evidence Supporting B: [EVIDENCE]
Resolution Status: Unresolved | In Negotiation | Resolved
Recommended Action: [WHAT TO DO]
Legal Counsel Required: Yes | Recommended | Optional
```

---

*→ Next: `COLLABORATION_OWNERSHIP.md`*  
*→ Licensing details: `../06-LEGAL-RIGHTS-INTELLIGENCE/LICENSING_ENGINE.md`*
