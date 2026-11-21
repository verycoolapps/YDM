# TRADEMARK PROTECTION
## YOUR DEAD MEAT — Legal & Rights Intelligence Module

---

**Purpose:** Defines trademark identification and protection workflows.
**Scope:** All projects with legal rights considerations.  
**Version:** 1.0.0  
**Dependencies:** `GLOBAL_RULES.md`, `LEGAL_LIMITATIONS.md`  

---

## TRADEMARK PROTECTION WORKFLOW

### Trademark Basics
A trademark is a word, name, symbol, or design (or combination) that identifies and distinguishes the source of goods or services from others.

**TM Symbol (™):** Claims trademark rights without formal registration.  
**® Symbol:** Indicates federally registered trademark. Use only after registration is confirmed.

### Trademark Registration Authorities

| Region | Authority | Website |
|--------|-----------|---------|
| United States | USPTO | uspto.gov |
| Indonesia | DJKI | dgip.go.id |
| European Union | EUIPO | euipo.europa.eu |
| International | WIPO Madrid System | wipo.int/madrid |

### Trademark Search (Before Applying)

Always conduct a clearance search before investing in a brand:

1. **USPTO TESS (US):** tmsearch.uspto.gov — Free search
2. **EUIPO eSearch:** euipo.europa.eu/eSearch — EU marks
3. **WIPO Global Brand Database:** branddb.wipo.int — International
4. **Indonesia DJKI:** pdki-indonesia.dgip.go.id
5. **Google/Web search:** Identify unregistered uses

### Trademark Strength Spectrum

| Mark Type | Strength | Example |
|-----------|---------|---------|
| Fanciful (invented) | Strongest | Kodak, Xerox, Zoom |
| Arbitrary | Strong | Apple (for computers) |
| Suggestive | Moderate | Netflix, Coppertone |
| Descriptive | Weak (unless acquired distinctiveness) | "Best" |
| Generic | No protection | "Bicycle" for bicycles |

### Trademark Record

```yaml
trademark_record:
  mark: "[MARK NAME OR DESCRIPTION]"
  mark_type: "Word | Logo | Combined | Trade dress"
  registration_status: "Registered | TM claim | Unregistered | Pending"
  registration_number: "[IF REGISTERED]"
  jurisdiction: "[WHERE REGISTERED]"
  classes: "[NICE CLASSIFICATION CLASSES]"
  first_use_date: "[DATE OF FIRST USE IN COMMERCE]"
```

---
