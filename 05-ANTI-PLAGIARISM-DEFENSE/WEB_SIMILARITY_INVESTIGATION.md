# WEB SIMILARITY INVESTIGATION
## YOUR DEAD MEAT — Authorized Public-Source Similarity Research

---

**Purpose:** Defines authorized public-source similarity research methodology.  
**Scope:** All investigations using publicly accessible web sources.  
**Version:** 1.0.0  
**Dependencies:** `PLAGIARISM_DETECTION_ENGINE.md`, `EVIDENCE_VAULT.md`  

---

## AUTHORIZED RESEARCH METHODS

YDM supports only **lawful, public-source research**. This means:

✅ Searching publicly accessible websites  
✅ Using public image search tools  
✅ Reviewing publicly posted social media content  
✅ Checking public repositories  
✅ Using Wayback Machine for historical evidence  
✅ Reviewing public marketplace listings  

❌ Accessing private accounts or systems  
❌ Using authentication bypass techniques  
❌ Scraping beyond public access  
❌ Creating fake accounts to access private content  
❌ Accessing employment records, private databases  

---

## WEB INVESTIGATION TOOLS

### Reverse Image Search (for Visual Works)
- **Google Images:** images.google.com → "Search by image"
- **TinEye:** tineye.com — specialized reverse image search
- **Yandex Images:** yandex.com/images — often finds more than Google
- **Bing Visual Search:** bing.com/visualsearch

### Historical Evidence
- **Wayback Machine:** web.archive.org — find when content first appeared
- **Google Cache:** cached version of pages (via "cache:[URL]")

### Code Similarity Search
- **GitHub Search:** github.com/search
- **Searchcode:** searchcode.com — searches open source code
- **SourceGraph:** sourcegraph.com

### Brand/Logo Research
- **USPTO TESS:** USPTO trademark database
- **EUIPO:** euipo.europa.eu
- **WIPO Madrid Monitor:** branddb.wipo.int

---

## WEB INVESTIGATION RECORD

```yaml
# WEB INVESTIGATION RECORD
# Case ID: YDM-CASE-[ID]
# Date: [DATE]

web_investigation:
  
  searches_conducted:
    - search_type: "Reverse image | Text search | Code search | Brand search"
      tool_used: "[TOOL NAME]"
      search_query_description: "[WHAT WAS SEARCHED — without sensitive details]"
      date_conducted: "[DATE]"
      results_summary: "[WHAT WAS FOUND]"
      evidence_captured: "Yes — stored at [LOCATION] | No results"
      
  suspect_work_locations:
    - url: "[PUBLIC URL OF SUSPECTED COPY]"
      platform: "[WEBSITE/PLATFORM NAME]"
      first_seen: "[DATE — approximate if unknown]"
      wayback_archive: "[WAYBACK URL IF ARCHIVED]"
      screenshot_stored: "Yes — EVD-[ID] | No"
      
  findings_summary:
    suspected_copies_found: "[NUMBER]"
    oldest_public_appearance_of_original: "[DATE — from Wayback or first post]"
    oldest_public_appearance_of_suspect: "[DATE]"
    chronology_supports_original_claim: "Yes | Unclear | No | Uncertain"
```

---

## EVIDENCE CAPTURE PROTOCOL

When finding suspected copies online:

```
EVIDENCE CAPTURE STEPS
━━━━━━━━━━━━━━━━━━━━━

1. Screenshot the full page (include URL in browser bar)
2. Note the date and time of capture
3. Submit URL to Wayback Machine: web.archive.org/save/[URL]
4. Download any publicly accessible versions
5. Record the platform, username, and posting date
6. Hash the screenshot and downloaded files
7. Store in Evidence Vault → 07-CORRESPONDENCE folder
```

---

*→ Next: `IMAGE_COPY_DETECTION.md`*  
*→ Back: `PLAGIARISM_DETECTION_ENGINE.md`*
