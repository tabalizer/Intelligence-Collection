# 🗂️ Archived Web OSINT Cheat Sheet 🕵️‍♀️

**Purpose:** Retrieve and analyze historical or deleted web content using open-source archiving services and tools to track digital footprints, monitor content changes, or uncover removed evidence.

---

## 🛠️ Essential Archive Tools

| Tool                 | Description                                                  | Link                                           |
|----------------------|--------------------------------------------------------------|------------------------------------------------|
| **Wayback Machine**  | Snapshots of web pages over time.                            | [archive.org/web](https://archive.org/web)     |
| **archive.today**    | Manual and real-time webpage capture with screenshot view.   | [archive.today](https://archive.today)         |
| **Memento Time Travel** | Aggregates results from multiple web archives.           | [timetravel.mementoweb.org](https://timetravel.mementoweb.org) |
| **CachedView**       | Google/Bing/Yandex cached page viewer.                       | [cachedview.com](https://cachedview.com)       |
| **Page History (Chrome Ext.)** | Shows archived versions via context menu.          | [Chrome Web Store](https://chrome.google.com/webstore/) |
| **Webcite (legacy)** | Citation-level archiving for academic/legal use.             | [webcitation.org](http://www.webcitation.org/) |

---

## 🧭 Methodology & Techniques

### 1. **Find Archived Versions**
- Use `Wayback Machine` or `archive.today` with full URLs:
  - Example: `https://archive.org/web/*/example.com/article.html`
  - OR: Paste URL into archive.today to manually trigger capture.

### 2. **Compare Versions Over Time**
- Investigate content changes (text, links, media):
  - Use Wayback's diff tools or download two versions and run `diff` locally.
- Useful for:
  - Tracking evolving narratives
  - Identifying deleted or reworded claims
  - Disinformation mapping

### 3. **Uncover Deleted Pages**
- Use search engine operators to retrieve cached pages:
  - `cache:example.com/page.html`
  - Or use CachedView to view Google/Yandex/Bing stored versions
- If missing: plug URL into Memento Time Travel for alt archives

### 4. **Pre-emptive Archiving (Defensive OSINT)**
- Proactively archive sensitive content (e.g., tweets, blog posts, defaced websites)
- Tools:
  - `SingleFile` (browser extension) for offline .html saving
  - `archive.today` for permanent public archiving

### 5. **Capture Evidence With Metadata**
- Use `Wayback Machine` HTTP headers or JSON API:
  - Shows timestamp, server headers, and crawl info
- Archive pages while logged out to avoid session-specific content

### 6. **Discover Unlinked or Obscure Content**
- Use `Common Crawl` or scrape archived sitemaps for:
  - Deindexed content
  - Shadow domains/subdomains that were once live

---

## 🧩 Advanced Tactics

- **Pivot on URLs**: Use archived outbound links to discover associated infrastructure (domains, platforms, etc.).
- **Regex on HTML Snapshots**: Extract emails, API endpoints, or JavaScript artifacts from archived raw source.
- **Capture Before It’s Deleted**: Use scripts (e.g., `waybackpy`, `screenshotapi.net`) to auto-archive pages on load or via alerts.
- **Investigate Redirect Chains**: Archived versions sometimes show redirect destinations that are now obfuscated live.

---

## ⚠️ Ethical & Operational Notes

- ✅ Archiving public data is generally legal — but always verify local laws.
- ⚠️ Never archive login sessions or personal inboxes (privacy violation).
- ❌ Avoid capturing behind-paywall content if it violates copyright.

---

**Deleted doesn't mean gone. Archive smart. Investigate sharp.** 🧠🕸️
