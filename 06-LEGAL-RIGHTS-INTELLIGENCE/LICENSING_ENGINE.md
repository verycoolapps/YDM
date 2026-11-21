# LICENSING ENGINE
## YOUR DEAD MEAT — Legal & Rights Intelligence Module

---

**Purpose:** Manages licensing information, permissions, and compliance.
**Scope:** All projects with legal rights considerations.  
**Version:** 1.0.0  
**Dependencies:** `GLOBAL_RULES.md`, `LEGAL_LIMITATIONS.md`  

---

## LICENSING FRAMEWORK

A license grants another party permission to use your work under specific conditions — without transferring ownership.

### Common License Types

#### Open / Creative Commons
| License | Commercial? | Modify? | Share-alike? |
|---------|-----------|--------|-------------|
| CC BY | Yes | Yes | No |
| CC BY-SA | Yes | Yes | Yes (same license) |
| CC BY-NC | No | Yes | No |
| CC BY-ND | Yes | No | No |
| CC0 | Yes (public domain) | Yes | No |

#### Software Licenses
| License | Commercial? | Disclose source? | Viral? |
|---------|-----------|-----------------|-------|
| MIT | Yes | No | No |
| Apache 2.0 | Yes | No | No |
| GPL 3.0 | Yes | Yes | Yes |
| LGPL | Yes | Partial | Partial |
| Proprietary | Per agreement | No | No |

### License Record

```yaml
# LICENSING RECORD
# Project ID: YDM-[ID]

licensing:
  
  outgoing_licenses:
    - licensee: "[WHO HAS A LICENSE TO USE THIS WORK]"
      license_type: "[TYPE]"
      grant_date: "[DATE]"
      rights_granted: "[WHAT THEY CAN DO]"
      restrictions: "[WHAT THEY CANNOT DO]"
      territory: "[GEOGRAPHIC SCOPE]"
      duration: "[TERM OR PERPETUAL]"
      compensation: "[PAID | FREE | REVENUE SHARE]"
      
  incoming_licenses:
    - asset: "[THIRD-PARTY ASSET]"
      licensor: "[WHO OWNS IT]"
      license_type: "[TYPE]"
      what_we_can_do: "[OUR PERMITTED USES]"
      attribution_required: "Yes | No"
      attribution_format: "[IF REQUIRED]"
```

### License Compatibility Matrix (Common Cases)

| You Want To Use | Your Project License | Compatible? |
|----------------|---------------------|------------|
| MIT-licensed code | Any | Yes |
| GPL-licensed code | GPL | Yes |
| GPL-licensed code | MIT (proprietary) | No |
| CC BY image | Commercial project | Yes (with attribution) |
| CC BY-NC image | Commercial project | No |

---
