# 🔍 Advanced Search Techniques for OSINT

Advanced search techniques are essential for navigating the web like an intelligence professional. They allow you to extract buried data, surface deleted content, and pinpoint sources others overlook. This cheat sheet breaks down the most powerful techniques with **realistic**, **practitioner-level examples** — no fluff.

## 🔢 Boolean Operators

**What it is:**  
Boolean operators control how keywords interact in a search. They help you combine, exclude, or prioritize terms to filter the signal from the noise.

**Core operators:**
- `AND`: Results must include both terms  
- `OR`: Results can include either term  
- `NOT` or `-`: Excludes results with a term  
- `""`: Exact phrase  
- `()`: Groups terms for structured logic

**Real OSINT Examples:**
- `"equipment manifest" AND ("UK MOD" OR "Ministry of Defence")`  
- `(telegram OR signal) AND "user ID"`  
- `"flight plan" AND NOT "training exercise"`  
- `"police incident report" AND "Milwaukee" AND "August 2023"`

✅ **Why it works:** Useful in breach investigations, insider threat detection, and cross-referencing leaks with local context.

---

## 🌐 Site-Specific Searches

**What it is:**  
Tells a search engine to look **only** within a specific website or domain.

**Syntax:** `site:domain.com search terms`

**Real OSINT Examples:**
- `site:facebook.com "lives in Tripoli" "works at airport"` — useful for geo-linked human targeting  
- `site:pastebin.com "database dump" AND "gov.bd"` — finding exposed Bangladeshi government data  
- `site:sec.gov "cyber incident disclosure"` — regulatory breach confirmations  
- `site:weibo.com AND "Huawei employee"` — sourcing profiles from Chinese-language platforms

✅ **Why it works:** Ideal for platform-specific searches, breach tracking, and identifying sensitive info buried in niche sources.

---

## 📄 File Type Searches

**What it is:**  
Searches for specific document types like PDFs, Excel files, PowerPoints, etc.

**Syntax:** `filetype:pdf`, `filetype:xls`, `filetype:ppt`, etc.

**Real OSINT Examples:**
- `filetype:xls "guest list" site:marriott.com` — targeting exposed travel data  
- `filetype:pdf "strategic planning meeting" site:.gov.ph` — finding internal government documents from the Philippines  
- `filetype:ppt "threat intelligence briefing" AND "Lockheed Martin"` — leaked corporate decks  
- `filetype:csv "employee directory" site:*.edu` — academic institutions leaking HR records

✅ **Why it works:** Perfect for uncovering internal reports, planning documents, credential lists, or regulatory filings.

---

## 🌍 Language-Specific Searches

**What it is:**  
Searching in native languages or localized domains to access region-specific data.

**Real OSINT Examples:**
- `"contrabando de armas" site:.mx` — firearm smuggling in Mexico  
- `"информационная безопасность" site:.ru` — Russian cyber policy documents  
- `"protestas estudiantiles" site:.cl` — Chilean student protest activity  
- Use DeepL or native sources to generate accurate search terms before querying

✅ **Why it works:** Critical when monitoring international incidents, region-specific disinformation, or domestic narratives in native languages.

---

## ⏱️ Time-Restricted Searches

**What it is:**  
Filters search results by date, allowing you to analyze event timelines or retrieve only recent activity.

**Where to use it:**  
Google → Tools → Any Time → Custom Range

**Real OSINT Examples:**
- `"data leak" site:twitter.com` filtered to last 24 hours — tracking new breach chatter  
- `"chemical spill" site:reuters.com` for June 2023 only — environmental event verification  
- `"suspect arrested" site:news.com.au` filtered by month — verifying law enforcement actions  
- Combine with Boolean and site searches for precise timeline mapping

✅ **Why it works:** Crucial in incident response, situational awareness, and tracking how narratives evolve over time.

---

## 🧾 Cached & Archived Content

**What it is:**  
Gives you access to modified, censored, or deleted web pages via caching or archiving platforms.

**Real OSINT Examples:**
- `cache:example.com/press-release` — Google’s last cached version  
- [archive.today](https://archive.today) URL submissions to preserve volatile content  
- Use [Wayback Machine](https://archive.org/web) to retrieve a pre-takedown version of a page  
- Track before/after changes in company policy pages, breach disclosures, or government directives

✅ **Why it works:** You don’t just collect information — you preserve it before it vanishes.

---

## 🖼️ Reverse Image Search

**What it is:**  
Finds other instances of an image online, helps verify origin, spot fakes, or identify people/places.

**Tools:**  
- [TinEye](https://tineye.com) — Best for historical image tracking  
- [Yandex Images](https://yandex.com/images) — Excellent for facial and location recognition  
- [Google Images](https://images.google.com) — Good general-purpose match  
- [InVID](https://www.invid-project.eu/tools/invid-verification-plugin/) — Video/thumbnail forensics

**Real OSINT Examples:**
- Use Yandex to find VK profiles that reused the same selfie  
- Run a building photo through Google Images to identify its location in a conflict zone  
- TinEye a meme image to find its earliest known use (for disinfo analysis)  
- Use InVID to validate a viral protest video’s location and date

✅ **Why it works:** Visual confirmation beats speculation. Reverse search supports attribution, authenticity, and timeline building.

---

## 🌊 Deep Web Discovery

**What it is:**  
Surfacing data that is unindexed, buried in databases, or gated behind search functions.

**Real OSINT Examples:**
- Search customs data inside PIERS or ImportGenius for maritime shipment analysis  
- Use `site:vk.com` + keywords to access Russian-language user data  
- Dive into internal search portals like UN treaty databases, academic journals, or court archives  
- Combine with automation (e.g., n8n, Puppeteer) to extract data behind login walls or session-based pages

✅ **Why it works:** Real intelligence lives where most search engines can't go.

---

## 🧰 OSINT Query Toolkit

| Task                        | Tools / Syntax                                              |
|-----------------------------|-------------------------------------------------------------|
| Complex logic filtering     | `AND`, `OR`, `NOT`, `"..."`, `()`                          |
| Platform-specific targeting | `site:`, `.tld`, language filters                          |
| Data/doc discovery          | `filetype:pdf`, `filetype:xls`, `filetype:csv`             |
| Visual forensics            | TinEye, Yandex, Google Images, InVID                       |
| Archived content recovery   | Wayback Machine, Archive.today, `cache:`                   |
| Time-focused investigations | Google → Tools → Time Range                                |
| Deep web penetration        | Database search, aggregators, custom scraping (n8n, MCP)   |

---

> ⚡ **Pro tip**: Master the syntax. Stack the techniques. Automate where possible. OSINT is as much about logic as it is about discovery.
```

---
