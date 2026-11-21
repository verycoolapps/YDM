# JURISDICTION INTELLIGENCE
## YOUR DEAD MEAT — Legal & Rights Intelligence Module

---

**Purpose:** Identifies relevant legal jurisdictions for IP matters.
**Scope:** All projects with legal rights considerations.  
**Version:** 1.0.0  
**Dependencies:** `GLOBAL_RULES.md`, `LEGAL_LIMITATIONS.md`  

---

## JURISDICTION IDENTIFICATION

IP law is territorial — rights, remedies, and procedures differ significantly by country.

### Jurisdiction Identification Decision Tree

```
JURISDICTION IDENTIFICATION
━━━━━━━━━━━━━━━━━━━━━━━━━━━

Q1: Where was the creator/rights holder located when creating the work?
    → This is often the primary jurisdiction for initial rights

Q2: Where is the work primarily used or published?
    → This may be a relevant enforcement jurisdiction

Q3: Where is the alleged infringer located?
    → This determines where legal action must be filed

Q4: Where are the infringing copies distributed?
    → May be multiple jurisdictions

Q5: Is there a governing law clause in any relevant contract?
    → If yes, that jurisdiction governs the contract
```

### Key Jurisdiction Notes

#### Indonesia
- Primary copyright law: Undang-Undang No. 28 Tahun 2014 tentang Hak Cipta
- Trademark: UU No. 20 Tahun 2016 tentang Merek
- Registration authority: DJKI (Direktorat Jenderal Kekayaan Intelektual) — dgip.go.id
- Copyright protection duration: Life + 70 years for most works

#### United States
- Copyright: Title 17, U.S. Code — automatic protection
- Trademark: Lanham Act — registration with USPTO
- Formal copyright registration enables statutory damages suits

#### Berne Convention Countries (Most of the World)
- Mutual recognition of copyright without formalities
- 179 member states as of 2024
- Protection extends automatically in member countries

### Jurisdiction Record

```yaml
jurisdiction_record:
  creator_location: "[COUNTRY/STATE]"
  work_creation_location: "[COUNTRY]"
  primary_publication_location: "[COUNTRY]"
  infringer_location: "[IF KNOWN — COUNTRY]"
  applicable_law:
    primary: "[JURISDICTION]"
    secondary: "[IF MULTIPLE JURISDICTIONS APPLY]"
  berne_convention_applies: "Yes | Partially | No"
  legal_counsel_jurisdiction: "[WHAT JURISDICTION SHOULD COUNSEL BE LICENSED IN]"
```

---
