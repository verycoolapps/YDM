# DESIGN ORIGINALITY
## YOUR DEAD MEAT — Visual & Design Project Originality Analysis

---

**Purpose:** Analyzes originality in visual design and art projects; documents distinctive visual characteristics.  
**Scope:** Digital art, illustration, graphic design, brand identity, UI/UX, and all visual creative projects.  
**Version:** 1.0.0  
**Dependencies:** `ORIGINALITY_ENGINE.md`, `CREATIVE_FINGERPRINTING.md`  

---

## VISUAL ORIGINALITY INDICATORS

### High Distinctiveness (Strongest Protection Potential)
- Invented characters or creatures with unique design language
- Original illustration style with identifiable personal marks
- Novel visual concept not following existing genre conventions
- Custom typefaces or extensively modified letterforms
- Invented visual symbols, iconography, or glyphs

### Moderate Distinctiveness
- Original composition within existing style conventions
- Unique color system with specific application rules
- Personal interpretation of an established genre or style
- Original decorative elements or pattern systems

### Low Distinctiveness (Use with Caution)
- Geometric shapes used in common arrangements
- Color palettes that are common in the field
- Typography using standard typefaces without modification
- Layout structures that are industry-standard

---

## DESIGN ORIGINALITY RECORD

```yaml
# DESIGN ORIGINALITY RECORD
# Project ID: YDM-[ID]

design_originality:
  
  visual_style_signature:
    color_system:
      primary_palette: "[HEX VALUES — e.g., #D7193F, #08090D]"
      palette_uniqueness: "Custom designed | Industry common | Mixed"
      application_rules: "[HOW COLORS ARE SPECIFICALLY USED]"
      
    typography:
      typefaces_used: "[FONT NAMES]"
      typeface_origin: "Custom designed | Modified | Standard licensed font"
      text_treatment: "[SPECIFIC TEXT STYLING CHOICES]"
      
    compositional_approach:
      layout_system: "[DESCRIBE THE LAYOUT PRINCIPLES]"
      distinctive_placement: "[WHAT IS PLACED UNUSUALLY]"
      negative_space_use: "[HOW NEGATIVE SPACE IS TREATED]"
      
    illustration_style:
      line_quality: "[DESCRIBE LINE CHARACTER — weight, variation, style]"
      rendering_approach: "[HOW FORMS ARE RENDERED]"
      texture_treatment: "[TEXTURE APPROACH]"
      
  distinctive_elements:
    - element_name: "[ELEMENT NAME]"
      description: "[DETAILED DESCRIPTION OF THIS ELEMENT]"
      appears_at: "[WHERE IN THE WORK]"
      uniqueness_basis: "[WHY THIS IS DISTINCTIVE]"
      
  referenced_styles:
    - style: "[STYLE/MOVEMENT/ARTIST THAT INFLUENCED THIS]"
      relationship: "Inspired by | Reacts against | Extends | Independent but similar"
      how_original_work_differs: "[SPECIFIC DIFFERENCES]"
      
  originality_assessment: "High | Moderate | Low"
  assessment_basis: "[REASONING]"
```

---

## VISUAL SIMILARITY WARNING THRESHOLDS

| Similarity Level | Action |
|-----------------|--------|
| Identical composition, color, elements | Immediate investigation required |
| Same concept, different execution | Document differences clearly |
| Same style, different elements | Note style influence, document independent creation |
| Same color palette | Note; palette alone rarely establishes copying |
| Same subject matter | Note; subject alone does not establish copying |

---

*→ Next: `CODE_ORIGINALITY.md`*  
*→ Image copy detection: `../05-ANTI-PLAGIARISM-DEFENSE/IMAGE_COPY_DETECTION.md`*
