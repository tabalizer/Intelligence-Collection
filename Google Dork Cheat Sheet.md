# Google Dork OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only. All search techniques must comply with local laws and platform ToS._

---

## 🎯 1) Purpose
Google Dorking (a.k.a. Google advanced search operators) is the practice of using specific syntax in search queries to uncover publicly accessible information that may not be obvious through normal browsing.

---

## 🛠 2) Core Tool Arsenal

### Primary Search Engines Supporting Dorking
- **Google** — https://www.google.com (primary and most up-to-date operator support).  
- **Bing** — https://www.bing.com (some operators work; differences in syntax).  
- **Yandex** — https://yandex.com (supports partial dorking syntax).  
- **DuckDuckGo** — https://duckduckgo.com (limited operator compatibility).

### Dork Testing Tools
- **Google Hacking Database (GHDB)** — https://www.exploit-db.com/google-hacking-database — Repository of known dork patterns.  
- **DorkSearch** — https://dorksearch.com — Minimalistic interface for quick operator testing.  
- **Pentest-Tools.com Dork Search** — Automated queries (security-focused; be mindful of ToS).

---

## 🔍 3) Common Dork Operators

| Operator | Function | Example |
|----------|----------|---------|
| `site:` | Restrict to a specific site/domain | `site:linkedin.com "osint investigator"` |
| `inurl:` | Search in the page URL | `inurl:"admin/login"` |
| `intitle:` | Search in the page title | `intitle:"index of"` |
| `filetype:` | Find specific file types | `filetype:pdf site:example.com` |
| `ext:` | Same as filetype | `ext:xls "confidential"` |
| `intext:` | Search for text within a page body | `intext:"internal use only"` |
| `cache:` | View Google’s cached version of a page | `cache:example.com` |
| `allinurl:` | All terms in URL | `allinurl:secure login` |
| `allintitle:` | All terms in page title | `allintitle:report confidential` |
| `allintext:` | All terms in page body | `allintext:"project phoenix"` |
| `OR` | Logical OR between terms | `"osint" OR "open source intelligence"` |
| `-` | Exclude terms | `"project x" -movie` |
| `*` | Wildcard placeholder | `"project * report"` |
| `..` | Numeric range | `2020..2024 filetype:pdf` |

---

## 🧩 4) Pivoting Opportunities
- Locate open directories containing sensitive files (`intitle:"index of"` with filetypes).  
- Find exposed device panels (`inurl:"/admin/login"`).  
- Search for config files or backup data (`filetype:sql` or `filetype:bak`).  
- Identify internal documents inadvertently published.  
- Cross-reference email addresses in cached pages.

---

## 📌 5) Key OSINT Applications
- **Personnel intel** — Discover resumes, org charts, or staff bios.  
- **Technical recon** — Identify exposed dev/test environments.  
- **Historical recovery** — Use `cache:` operator for recently changed/removed pages.  
- **Event mapping** — Search event pages, flyers, or schedules with location details.

---

## 🌐 6) Cross-Platform Verification
- Test same dork on Bing, Yandex, and DuckDuckGo for alternative indexing.  
- Compare cached pages between engines for differences in captured content.  
- Use GHDB as inspiration, but adapt queries for specificity.

---

## ⚠️ 7) 2025 Environment & Cautions
- Frequent Google syntax updates — some operators deprecated or altered.  
- High-frequency querying with certain dorks may trigger CAPTCHAs.  
- Accessing sensitive, non-public data may be illegal — stick to publicly available content.

---

## 🛡 8) Investigator Tips
- Chain operators for precision (e.g., `site:example.com filetype:pdf "confidential"`).  
- Use `OR` and `-` strategically to widen/narrow searches.  
- Archive valuable results — indexed pages may disappear quickly.

---

## 🗂 9) Documentation Hygiene
- Record: dork used, search engine, date/time, and top relevant results.  
- Keep a private repository of effective dorks for recurring use.

---

### 📜 Changelog (2025-08-10)
- Updated operator table for 2025 syntax compatibility.  
- Added Bing/Yandex/duckduckgo operator parity notes.  
- Expanded OSINT pivot use cases.
