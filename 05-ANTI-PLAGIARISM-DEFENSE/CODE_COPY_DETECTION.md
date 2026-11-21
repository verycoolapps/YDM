# CODE COPY DETECTION
## YOUR DEAD MEAT — CODE COPY DETECTION Module

---

**Purpose:** Detects suspicious code similarities and copied software components.  
**Scope:** Specialized detection for this asset type.  
**Version:** 1.0.0  
**Dependencies:** `PLAGIARISM_DETECTION_ENGINE.md`, `SIMILARITY_ANALYSIS.md`, `FALSE_POSITIVE_PROTECTION.md`  

---

## CODE SIMILARITY DETECTION

### Code Copying Indicators (Strongest First)

| Indicator | Strength | Description |
|-----------|---------|-------------|
| Identical code blocks | Very Strong | Same logic, same variable names |
| Variable rename only | Strong | Logic identical, names changed |
| Comment preservation | Strong | Copied code retains original comments |
| Identical unusual bug | Strong | Same non-obvious bug appears in both |
| Structural clone | Moderate | Same architecture, different implementation |
| Algorithm similarity | Weak | Same algorithm (may be independent) |
| Standard pattern | None | Industry-standard pattern |

### Code Comparison Methodology

```
CODE COPY DETECTION PROCESS
━━━━━━━━━━━━━━━━━━━━━━━━━━━

1. Identify distinctive code sections in original
   (focus on non-standard, non-obvious implementations)
   
2. Extract key identifiers:
   - Unusual variable/function names
   - Non-standard algorithm implementations
   - Custom comments and documentation
   - Specific logic sequences
   
3. Search suspected copy for exact matches first
   (copy unique string → paste in GitHub search)
   
4. If exact match found: document precisely
   (file name, line numbers in both works)
   
5. If modified match: document the modification pattern
   (variable renaming, whitespace changes, etc.)
   
6. Assess access: could infringer have seen original?
   (Was original published? On public GitHub? Open source?)
```

### Code Comparison Record

```yaml
code_comparison:
  original_file: "[FILENAME]"
  original_commit: "[GIT SHA — if available]"
  
  matching_elements:
    - type: "Exact match | Variable rename | Structural clone"
      original_location: "[FILE:LINE]"
      original_excerpt: "[SHORT EXCERPT — no sensitive data]"
      suspected_location: "[FILE:LINE in suspected copy]"
      match_quality: "Identical | Near-identical | Similar"
```

---
