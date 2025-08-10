# Archived Web OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only. All activities must comply with local law, copyright rules, and platform ToS._

---

## 🎯 1) Purpose
To retrieve and analyze **archived web content** from multiple sources beyond the Internet Archive’s Wayback Machine, enabling investigators to recover deleted or modified information for verification, attribution, or historical analysis.

---

## 🛠 2) Core Tool Arsenal

### Web Archives
- **Wayback Machine** — https://web.archive.org — Largest and most widely used.  
- **Archive.today / archive.is** — Static page snapshots, often bypasses robots.txt restrictions.  
- **Perma.cc** — Permanent archiving by academic/legal institutions.  
- **Memento Time Travel** — https://timetravel.mementoweb.org — Aggregates multiple archives.  
- **UK Web Archive** — https://www.webarchive.org.uk — UK-centric web content.  
- **Arquivo.pt** — https://arquivo.pt — Portuguese web archive, with unique coverage.

### Search Engine Caches
- **Google Cache** — `cache:example.com` in Google search.  
- **Bing Cache** — Similar to Google, often holds different dates.  
- **Yandex Cache** — Preserves content even after removal in some regions.

### Specialty Archives
- **GitHub Archive** — Historical code and commit data for repos.  
- **Text-Only Archive Tools** — Text-Only versions for quick keyword searches in archived pages.  
- **Common Crawl** — Massive open dataset of crawled web data.

---

## 🔍 3) Investigation Workflow
1. **Identify Target URL or Domain** — The page, section, or full site of interest.  
2. **Query Multiple Archives** — Avoid relying on one source; each has different capture policies.  
3. **Compare Snapshots** — Look for removals, edits, or inserted content over time.  
4. **Corroborate** — Match findings against official statements or contemporaneous reporting.  
5. **Capture** — Save multiple dated versions locally for verification.

---

## 🧩 4) Pivoting Opportunities
- Discover legacy employee lists, contact info, or product specs.  
- Identify previously visible subdomains from archived menus.  
- Recover deleted social media embeds or images hosted on third-party servers.  
- Extract versioned documents (e.g., PDFs) from archived file directories.

---

## 📌 5) Key Clues from Archived Web Data
- **Domain changes** — Redirects, ownership changes, or platform migrations.  
- **Content gaps** — Time ranges with missing captures may indicate deliberate suppression.  
- **Visual branding shifts** — Rebrands or mergers.  
- **Technical footprint** — Outdated JavaScript, analytics codes, or CMS details.

---

## 🌐 6) Cross-Platform Verification
- Compare archived policies/prices to consumer complaints or court filings.  
- Match contact data to WHOIS historical records.  
- Use archived images in reverse image searches to find their reuse.

---

## ⚠️ 7) 2025 Environment & Cautions
- Some archives (e.g., Google Cache) purge data very quickly — capture ASAP.  
- Archive.today may strip scripts — useful for static content but not dynamic pages.  
- Many government or corporate sites have legal carve-outs preventing archiving.

---

## 🛡 8) Investigator Tips
- Automate multi-archive checks via tools like **Memento** or **Wayback Machine Downloader**.  
- When archiving proactively, capture both **HTML + media**.  
- Save text-only versions for quick keyword searching in large sets.

---

## 🗂 9) Documentation Hygiene
- Record: URL, snapshot date(s), archive source, observed changes, and confidence rating.  
- Preserve both rendered screenshots and raw HTML.

---

### 📜 Changelog (2025-08-10)
- Added multi-archive aggregation tools.  
- Expanded pivoting opportunities with file/document recovery.  
- Updated cautions for rapid cache expiration in 2025.
