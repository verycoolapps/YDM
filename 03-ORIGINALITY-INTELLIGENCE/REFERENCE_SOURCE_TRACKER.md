# REFERENCE SOURCE TRACKER
## YOUR DEAD MEAT — References, Inspirations & Third-Party Source Documentation

---

**Purpose:** Records all references, inspirations, and third-party sources used or consulted in a project.  
**Scope:** All projects. Source tracking strengthens originality claims and identifies potential licensing issues.  
**Version:** 1.0.0  
**Dependencies:** `ORIGINALITY_ENGINE.md`, `LICENSING_ENGINE.md`  

---

## WHY DOCUMENT REFERENCES?

Paradoxically, documenting your references **strengthens** your originality claim. It demonstrates:
1. You are aware of existing works in your field
2. Your work is different from those works in documented ways
3. You acted in good faith regarding third-party content
4. Any similarity to those works is acknowledged and contextual

---

## REFERENCE SOURCE RECORD

```yaml
# REFERENCE SOURCE TRACKER
# Project ID: YDM-[ID]

reference_sources:
  
  inspiration_sources:
    - source_name: "[WORK/CREATOR/ARTICLE/WEBSITE]"
      source_type: "Artwork | Software | Writing | Presentation | Research | Tutorial | Other"
      url_or_location: "[WHERE IT CAN BE FOUND — if public]"
      how_used: "Visual inspiration | Conceptual direction | Technical reference | Mood board"
      relationship_to_own_work: >
        "[HOW YOUR WORK IS DIFFERENT FROM THIS INSPIRATION]"
      license_check_done: "Yes | No | Not Required"
      
  third_party_assets_used:
    - asset_name: "[ASSET NAME]"
      asset_type: "Image | Font | Icon | Sound | Video | Code snippet | Dataset | Other"
      source: "[WHERE OBTAINED]"
      license: "[LICENSE TYPE — e.g., CC BY 4.0, MIT, Proprietary]"
      license_url: "[LICENSE DOCUMENT URL]"
      usage_restrictions:
        commercial_use_permitted: "Yes | No | Unclear"
        modification_permitted: "Yes | No | Unclear"
        attribution_required: "Yes | No | Unclear"
        attribution_format: "[HOW TO CREDIT — if required]"
      usage_in_project: "[HOW IT'S USED IN THE PROJECT]"
      license_complied_with: "Yes | In Progress | Verification Needed"
      
  research_sources:
    - source: "[ARTICLE/BOOK/PAPER CONSULTED]"
      citation: "[PROPER CITATION]"
      usage: "Background research | Direct quotation | Paraphrase | Data source"
      
  tools_and_software:
    - tool: "[SOFTWARE USED TO CREATE THIS WORK]"
      version: "[VERSION]"
      license: "[YOUR LICENSE TYPE]"
      
  public_domain_elements:
    - element: "[ELEMENT SOURCED FROM PUBLIC DOMAIN]"
      source: "[WHERE IT CAME FROM]"
      public_domain_basis: "[WHY IT IS PUBLIC DOMAIN — age, government work, explicit release]"
```

---

## LICENSE COMPLIANCE CHECKLIST

Before publishing or distributing a project:

```
LICENSE COMPLIANCE REVIEW
━━━━━━━━━━━━━━━━━━━━━━━━━

□ All third-party assets identified
□ License type confirmed for each asset
□ Commercial use permitted (if applicable)
□ Modification rights confirmed (if applicable)
□ Attribution requirements met
□ Attribution format follows license requirements
□ Incompatible licenses identified and resolved
□ Open source license obligations met (for software)
□ License compliance documented in project records
```

---

*→ Next: `SIMILARITY_ANALYSIS.md`*  
*→ Licensing details: `../06-LEGAL-RIGHTS-INTELLIGENCE/LICENSING_ENGINE.md`*
