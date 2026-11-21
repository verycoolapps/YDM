# IMAGE COPY DETECTION
## YOUR DEAD MEAT — IMAGE COPY DETECTION Module

---

**Purpose:** Detects visual similarities and potential unauthorized reuse of images, illustrations, and visual art.  
**Scope:** Specialized detection for this asset type.  
**Version:** 1.0.0  
**Dependencies:** `PLAGIARISM_DETECTION_ENGINE.md`, `SIMILARITY_ANALYSIS.md`, `FALSE_POSITIVE_PROTECTION.md`  

---

## VISUAL SIMILARITY DETECTION

### Detection Levels for Images

| Level | Characteristics | Action |
|-------|----------------|--------|
| Exact copy | Pixel-identical or near-identical | Strong case — investigate |
| Color swap | Same composition, different palette | Investigate |
| Style copy | Same style, different elements | Note style influence; not copying per se |
| Element copy | Specific isolated elements reused | Investigate the specific elements |
| Thematic similarity | Same subject/theme | Note; not copying |

### Visual Comparison Checklist

```
IMAGE COPY DETECTION CHECKLIST
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

□ Compare overall composition (rule of thirds placement, focal points)
□ Compare specific element positions and proportions
□ Compare color palette (hex values, not just impressions)
□ Compare distinctive details at high zoom level
□ Compare negative space treatment
□ Compare stylistic markers (brush strokes, texture patterns)
□ Compare any embedded text or typography
□ Check for mirrored/flipped versions
□ Check for color-shifted versions
□ Check for cropped versions
□ Compare at different resolutions (upscaled copies show artifacts)
```

### Image Investigation Record

```yaml
image_comparison:
  original:
    file_hash: "[SHA-256]"
    dimensions: "[WIDTH x HEIGHT]"
    dominant_colors: "[HEX VALUES]"
    distinctive_elements: "[LIST]"
    
  suspected_copy:
    location: "[PUBLIC URL]"
    dimensions: "[IF KNOWN]"
    color_comparison: "Identical | Shifted | Different"
    
  match_analysis:
    composition_match: "Exact | High | Moderate | Low"
    element_match: "Exact | High | Moderate | Low"
    overall_similarity: "Level 1-5"
    
  evidence_captured: "[SCREENSHOT + HASH + DATE]"
```

---
