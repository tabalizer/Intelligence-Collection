# Wayback Machine OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only. All activities must comply with local law, copyright rules, and platform ToS._

---

## 🎯 1) Purpose
To leverage the Internet Archive’s **Wayback Machine** for retrieving historical versions of websites, uncovering deleted content, and tracking changes over time for OSINT investigations.

---

## 🛠 2) Core Tool Arsenal

### Primary Interface
- **Wayback Machine Web UI** — https://web.archive.org — Search by URL and select snapshots by date/time.
- **Wayback Machine Chrome/Firefox Extension** — Quick archive check and save from browser.
- **Save Page Now** — https://web.archive.org/save — Immediate manual archiving of a live page.

### APIs & Bulk Access
- **Wayback CDX API** — Query snapshot lists programmatically.  
  Example: `http://web.archive.org/cdx/search/cdx?url=example.com&output=json`
- **Wayback Availability API** — Check if a page is archived without loading it.  
  Example: `https://archive.org/wayback/available?url=example.com`

### Third-Party Helpers
- **Wayback Machine Downloader** (CLI tool) — Download full archived sites.  
- **Archive.today** — Alternate archiving service (captures pages Wayback may miss).  
- **Memento Time Travel** — Aggregate multiple web archives.

---

## 🔍 3) Investigation Workflow
1. **Identify Target URL** — Domain, subdomain, or specific page.  
2. **Query Archive** — Search in Wayback for earliest and latest snapshots.  
3. **Compare Versions** — Identify additions, removals, or edits using side-by-side tools.  
4. **Corroborate** — Verify removed content via other archives or cached search engine results.  
5. **Capture** — Download relevant snapshots and store locally.

---

## 🧩 4) Pivoting Opportunities
- Find deleted product listings, blog posts, or policy pages.  
- Recover old employee directories or team pages.  
- Extract metadata from archived images/documents hosted on the site.  
- Discover legacy subdomains via archived navigation menus.

---

## 📌 5) Key Clues from Archived Pages
- **Text Changes** — Policy updates, contact info, organizational changes.  
- **Image Changes** — Logo updates, product photos, event pictures.  
- **Hyperlink Patterns** — Changes in outbound or internal link structures.  
- **Tech Stack Evidence** — Legacy scripts, analytics codes, server headers.

---

## 🌐 6) Cross-Platform Verification
- Use **WHOIS historical data** alongside archived contact details.  
- Check old social media embeds for now-deleted posts.  
- Compare archived pricing/policies with customer complaints or legal filings.

---

## ⚠️ 7) 2025 Environment & Cautions
- Some sites block crawling by archive.org — use alternate archives.  
- Not all snapshots are complete — embedded media may be missing.  
- Robots.txt changes may hide older content from current view.

---

## 🛡 8) Investigator Tips
- Use **URL wildcards** (e.g., `example.com/*`) to discover subpages.  
- Check **snapshot frequency** — bursts of activity can indicate major site changes.  
- Archive pages immediately upon discovery if they may be removed.

---

## 🗂 9) Documentation Hygiene
- Record: target URL, snapshot dates, archive URLs, key findings, and confidence rating.  
- Store downloaded HTML and media files in local investigation folders.

---

### 📜 Changelog (2025-08-10)
- Added API and bulk download tools.  
- Included pivot opportunities for metadata extraction.  
- Updated cautions for 2025, including robots.txt impacts.
