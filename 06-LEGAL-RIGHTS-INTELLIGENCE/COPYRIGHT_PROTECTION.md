# COPYRIGHT PROTECTION
## YOUR DEAD MEAT — Legal & Rights Intelligence Module

---

**Purpose:** Defines copyright protection workflows and registration guidance.
**Scope:** All projects with legal rights considerations.  
**Version:** 1.0.0  
**Dependencies:** `GLOBAL_RULES.md`, `LEGAL_LIMITATIONS.md`  

---

## COPYRIGHT PROTECTION WORKFLOW

### Automatic Protection
Copyright protection in most countries attaches automatically upon creation of an original work fixed in a tangible medium. No registration is required.

**However, registration provides:**
- Public record of ownership
- Legal presumption of validity (in jurisdictions that require it)
- Ability to sue for statutory damages and attorney fees (US)
- Stronger enforcement position generally

### Copyright Registration Authorities by Region

| Region | Authority | Website |
|--------|-----------|---------|
| United States | U.S. Copyright Office | copyright.gov |
| Indonesia | DJKI (Direktorat Jenderal Kekayaan Intelektual) | dgip.go.id |
| European Union | National offices (no EU-wide copyright registration) | — |
| United Kingdom | Intellectual Property Office | ipo.gov.uk |
| Australia | Copyright is automatic; no registration | — |
| International (Berne Convention) | Automatic in member countries | wipo.int |

### Copyright Notice Best Practice

Standard format: `© [YEAR] [RIGHTS HOLDER]. All rights reserved.`

- The © symbol is not legally required in most Berne Convention countries, but is excellent practice
- The year is the year of first publication
- The rights holder is the owner (not necessarily the creator)

### Copyright Duration Guide

| Work Type | Duration (General) |
|-----------|-------------------|
| Original literary/artistic works | Life of author + 70 years (US, EU) |
| Works made for hire | 95 years from publication or 120 from creation |
| Anonymous works | 95 years from publication or 120 from creation |
| Indonesian works | Life + 70 years (Undang-Undang No. 28 Tahun 2014) |

**Note:** Always verify current law for specific jurisdiction.

### Copyright Protection Record

```yaml
copyright_status:
  registration_status: "Registered | Unregistered | In Progress"
  registration_number: "[IF REGISTERED]"
  jurisdiction: "[WHERE REGISTERED]"
  registration_date: "[IF REGISTERED]"
  copyright_notice_applied: "Yes | No"
  notice_format: "[FORMAT USED]"
```

---

*→ Next: \`TRADEMARK_PROTECTION.md\`*

---
