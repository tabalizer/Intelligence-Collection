# Bluesky OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only. Activities must comply with local law, privacy regulations, and platform ToS._

---

## 🎯 1) Purpose
To collect and analyze open-source intelligence from **Bluesky Social** — a decentralized, AT Protocol–based social network — for investigative, research, or situational awareness purposes.

---

## 🛠 2) Core Tool Arsenal

### Official Access
- **Bluesky Web Client** — https://bsky.app — Search by handle, display name, or keyword.  
- **Bluesky Mobile App** — iOS/Android official clients for real-time monitoring.  
- **AT Protocol API** — https://atproto.com — Programmatic access to public posts, profiles, and feeds.

### Third-Party Tools & Search
- **Skyview** — https://skyview.social — Enhanced search & filtering for Bluesky posts.  
- **Bsky Search** — https://search.bsky.social — Full-text post and profile search.  
- **Deck.blue** — Multi-column dashboard (TweetDeck-style) for keyword and user tracking.  
- **Bluesky Graph Explorer** — Visualization of follower/following relationships.  

### Data Enrichment & Cross-Platform
- **Handle Verification** — Check if Bluesky handle matches a verified domain (`_dns` TXT record in DNS).  
- **Cross-Identity Search** — Compare profile photos, bios, and handles against Twitter, Mastodon, LinkedIn.  
- **Wayback Machine** — Archive profiles/posts that may later be deleted.

---

## 🔍 3) Investigation Workflow
1. **Identify** — Start with handle (`@username.bsky.social`) or display name.  
2. **Search** — Use both official app search and third-party tools for posts, hashtags, and mentions.  
3. **Map Network** — Examine follower/following connections via Graph Explorer or API queries.  
4. **Correlate** — Match visual and textual clues with other platforms.  
5. **Archive** — Save screenshots, post URLs, and JSON exports via API.

---

## 🧩 4) Pivoting Opportunities
- Search unique hashtags to identify thematic groups or events.  
- Identify linked domains from user profiles for further OSINT (WHOIS, DNS, etc.).  
- Follow repost chains to locate original sources.  
- Analyze language/time zone patterns in posting history.

---

## 📌 5) Key Clues in Bluesky Data
- **Handle format** — Often includes custom domains (e.g., `@john.example.com`) that reveal affiliations.  
- **Bio** — May include job title, location, or other identifiers.  
- **Linked Websites** — Potential OSINT targets for deeper domain analysis.  
- **Post Media** — Images, videos, or documents attached to posts can be analyzed with image OSINT tools.

---

## 🌐 6) Cross-Platform Verification
- Reverse image search on profile pictures and post media.  
- Compare language and activity patterns across other social platforms.  
- Match known usernames to email patterns for breach or contact searches.

---

## ⚠️ 7) 2025 Environment & Cautions
- Bluesky search is still evolving; some older posts may not be discoverable in the official client.  
- The decentralized nature of AT Protocol means data can be hosted on multiple personal servers — results vary.  
- Deleted content may persist on some mirrors; handle with ethical and legal care.

---

## 🛡 8) Investigator Tips
- Use API exports for high-volume analysis rather than manual search.  
- Archive early — Bluesky posts can be edited or deleted without visible history.  
- Build watchlists of handles, hashtags, and domains for ongoing monitoring.

---

## 🗂 9) Documentation Hygiene
- Record: handle, display name, query terms, tools used, and archive locations.  
- Store JSON exports and media files separately with metadata.

---

### 📜 Changelog (2025-08-10)
- Updated third-party tool list with active 2025 search services.  
- Added decentralized hosting considerations.  
- Expanded pivoting opportunities for domain-linked handles.
