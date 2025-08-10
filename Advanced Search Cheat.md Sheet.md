# Advanced Search Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only. Use ethically and comply with local law & platform ToS._

## 1) Purpose
A practical, engine-agnostic reference for constructing precise web searches across Google, Bing, and Yandex to surface hard-to-find OSINT signals quickly.

## 2) Core Workflow (FIND)
1) **Frame** the question → define entities (who/what/where/when).  
2) **Intent** → decide whether you need people, docs, media, code, or news.  
3) **Narrow** → add site:, filetype:, date range, language/region.  
4) **Double-check** → run variants across multiple engines and compare top 20 results.

## 3) High-signal operators (cross-engine)
- `site:domain.tld` — restrict results to a site or TLD (`site:*.gov`, `site:co.uk`).  
- `"exact phrase"` — force literal match; combine with site: for bios/quotes.  
- `-term` — exclude noisy terms (`-job -hiring -template`).  
- `OR` — broaden with synonyms (`"resume" OR "cv"`).  
- `filetype:pdf` / `ext:pdf` — documents; try `ppt`, `pptx`, `xls`, `xlsx`, `doc`, `docx`, `csv`, `txt`.  
- `intitle:` — target page titles; stack with keywords.  
- `inurl:` — target URL path/params (good for `admin`, `profile`, `view` patterns).

> Tip: Chain operators: `site:example.com (policy OR guideline) filetype:pdf "2024"`

## 4) Google specifics
- **Date filter:** Tools → Time → Past 24h/Week/Month/Custom (YYYY-MM-DD).  
- **Numeric range:** `2019..2025` (useful for reports/versions).  
- **Cache view:** `cache:example.com/page` (snapshot may be stale).  
- **Verbatim mode:** Settings → **All results → Verbatim** to reduce synonyms/autocorrect.  
- **Region/language:** `&lr=lang_en` or search settings → Language/Region to de-bias local results.

## 5) Bing specifics
- Accepts most Google-style operators; differences:  
  - `contains:` surfaces pages linking to specific filetypes.  
  - Strong image/video verticals; use **Filters → Date/Resolution** quickly.  
  - Often less aggressive personalization—useful for “second look” on the same query.

## 6) Yandex specifics
- Strong for Cyrillic/non-Latin and visual similarity; try the same dorks in Russian.  
- Good geographic biasing by selecting Interface Language + Region in settings.  
- Reverse image search can return matches Google misses.

## 7) Personas & de-biasing
- Use clean browser profiles (no history/cookies) and switch **language/region**.  
- Compare logged-out vs logged-in results (when policy allows) to surface hidden items.  
- Try synonyms in target language(s): e.g., `"press release" OR "communiqué" OR "pressemelding"`.

## 8) People & org discovery patterns
- People: `site:linkedin.com/in "Title" "Company"`, `site:twitter.com "@handle"`, `"Full Name" "city"`.  
- Orgs: `site:{company.tld} (orgchart OR team OR "leadership")`, `"@company.tld" email`.  
- Docs: `site:{domain} filetype:(pdf OR pptx OR xlsx) (budget OR roadmap OR policy)`.

## 9) Technical & code intel
- GitHub: `site:github.com "{company}" (token OR api_key OR password) -fork`, `inurl:.env "SECRET="`.  
- Cloud buckets: `"index of" backup site:storage.googleapis.com` (be lawful; do not access non-public data).  
- Device footprints: combine with Shodan/Censys results (see Domain & IP sheet).

## 10) Media & local evidence
- Events: `"event program" filetype:pdf "City" 2024..2025`.  
- Local news/blogs: `site:*.localnews.tld "keyword"`, add language terms.  
- Images: Use engine’s **Tools → Size** (large) and date filters for investigative timelining.

## 11) Date & freshness tactics
- Always re-run promising dorks with **custom date ranges** to see evolution.  
- For breaking topics: add `after:2025-07-01` (Bing supports `after:`/`before:`), or Google custom dates.  
- Use quotes + month names to pin time (`"March 2025" "Project X"`).

## 12) Noise control
- Exclusions: `-site:pinterest.* -site:facebook.com -site:youtube.com` when they swamp results.  
- Template suppression: add `-template -sample -placeholder`.  
- Job spam: `-jobs -careers -hiring`.

## 13) Internationalization
- Translate the query nouns/verbs; run in target languages.  
- Swap locale numerals/units (e.g., `km` vs `miles`, comma vs dot decimals).

## 14) Documentation hygiene
- Log **query string**, **engine**, **time**, **filters**, and **top results**.  
- Capture screenshots or export SERPs to PDF for reproducibility.  
- Note **language/region settings** used for each run.

## 15) Quick recipes
- **Policy change trace:** `site:example.com (policy OR terms) filetype:pdf 2023..2025` then use Wayback for diffs.  
- **Org chart hunt:** `site:example.com ("organization chart" OR orgchart OR "team structure") filetype:(pdf OR pptx)`.  
- **Contact leads:** `"@example.com" -site:example.com -site:linkedin.com` to find external mentions.  
- **Event sourcing:** `"call for papers" "{topic}" 2025 filetype:(pdf OR docx)`.

### Changelog (2025-08-10)
- Consolidated cross-engine operator set; clarified Google/Bing/Yandex deltas.  
- Added de-biasing/persona tactics and noise-control patterns.  
- Included reproducibility checklist for investigative documentation.
