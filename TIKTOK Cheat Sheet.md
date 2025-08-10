# TikTok OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only (no credentialed access). Use ethically and abide by local law & TikTok ToS._

---

## 1) Fast pivots (copy/paste)
**Keyword search (web):**
- `https://www.tiktok.com/search?q={query}`  
  _Tip:_ If a shared link forces “Open App,” strip tracking params after `?` (see §7).

**Profile (handle):**
- `https://www.tiktok.com/@{username}`

**Single video (ID):**
- `https://www.tiktok.com/@{username}/video/{video_id}`

**Hashtag:**
- `https://www.tiktok.com/tag/{hashtag}`  
  _(Use raw term or URL-encode emojis/symbols.)_

**Sound (audio track):**
- `https://www.tiktok.com/music/{slug}-{sound_id}`

**Effect / Sticker:**
- `https://www.tiktok.com/sticker/{slug}-{effect_id}`

**LIVE surfaces (desktop web):**
- Browse: `https://www.tiktok.com/live`
- Following: `https://www.tiktok.com/live/following`

---

## 2) Discovery & collection workflow
1) **Seed**  
   - Start with **keyword** or **hashtag** search (web), then pivot into profiles and sounds/effects tied to the niche.
2) **Expand entities**  
   - From a **video page**, collect: handle, display name, caption text, hashtags, linked **sound page**, and any visible external **bio link** on the profile.
   - From a **sound page**, enumerate videos using that sound → identify recurring handles, niches, geos.
3) **Corroborate & date**  
   - Prefer **profile grids** (newest first). If timestamps are relative, cross-check via **Google time filters** (see §3).
4) **Capture**  
   - Save stable URLs (clean of tracking params), screenshots of critical metadata, and the short list of pivot entities (handles, hashtags, sound IDs, effect IDs).

site:tiktok.com "@{handle}"
site:tiktok.com inurl:"/video/" "{keyword}"
site:tiktok.com/tag "{topic or slogan}"
site:tiktok.com/music "{song or meme name}"

_Why:_ Google often indexes public profile/video/tag pages and lets you restrict by recency when TikTok’s own UI lacks robust filters.

---

## 4) What each surface gives you
- **Profile pages**: Handle, display name, bio text, external link, follower/like counts (approx), grid of public videos.
- **Video pages**: Caption text, referenced **hashtags**, **sound** link, handle, like/comment/share counts (variable visibility), and relative post time.
- **Hashtag pages**: Video corpus around the tag—useful to map trends & participating accounts.
- **Sound pages**: Corpus of videos using the same audio—good for tracing meme propagation and creator clusters.
- **Effect/Sticker pages**: Who’s using a particular effect (useful for campaign/theme tracing).
- **LIVE**: Snapshot of active streams; useful for real-time situational awareness (desktop web surfaces are more stable).

---

## 5) Cross-platform and handle pivoting
- Reuse the same **handle** across platforms to expand the identity graph (IG, X/Twitter, YouTube, Discord, Telegram, etc.).
- From the profile **bio link**, pivot to websites/link hubs to enumerate additional identifiers (domains, emails, other social links).

---

## 6) Third-party viewers (use cautiously)
If the web UI is login-gated or geo-nudged, third-party viewers can help you **locate** public content (availability varies, links change).  
_Examples:_ UrleBird, Brainans, Vidnice.  
**Caveats:** Coverage and freshness are inconsistent; avoid downloading or processing content in ways that breach ToS or local law.

---

## 7) Stabilizing URLs (share links → canonical)
- Many shared links include tracking params (e.g., `?_t=...&_r=...`).  
  **Action:** Delete the `?` and everything after it to get a stable, loadable URL:
  - Before: `https://www.tiktok.com/@user/video/1234567890?_t=...&_r=...`
  - After:  `https://www.tiktok.com/@user/video/1234567890`

---

## 8) LIVE & desktop behaviors (2025)
- Desktop web exposes **/live** and **/live/following** feeds and **Live Studio** docs; mobile browsers may push to app.
- Some actions (commenting, following, etc.) require login; **viewing** public content is often possible as guest on desktop.

---

## 9) Research API (for approved researchers)
- TikTok’s **Research API** offers programmatic access to public data for vetted researchers (queries support boolean logic such as `AND/OR/NOT`).
- If you have access, prefer official endpoints for metadata over brittle scraping.  
_Reference:_ developers.tiktok.com → Research API.

---

## 10) Rate limits, gating & practical tips
- Expect **rate-limits** and intermittent **login prompts** on the web UI. If blocked:
  - Try desktop mode, add `?lang=en`, or revisit later.
  - Use Google pivots (with time filters) to jump directly into target pages.
- **EXIF** is typically stripped; rely on page-visible metadata and cross-platform corroboration.
- **Region/age gating** may hide certain content; note these limitations in your report.

---

## 11) Documentation hygiene (for this sheet)
- Always store: **canonical URL**, capture time (UTC), entity type (profile/video/hashtag/sound/effect), and key pivots discovered.
- Keep a small **changelog** with “Last verified” date and the exact surfaces tested.

---

### Changelog (2025-08-10)
- Added **LIVE** surfaces and current desktop behaviors.
- Documented **URL stabilization** by stripping tracking params from share links.
- Included **sound** and **sticker/effect** URL patterns.
- Expanded **Google pivots** section + date filtering for recency.
- Added note on **Research API** for vetted access.


---

## 3) Google pivots (use when web search is gated)
Use Google operators to find TikTok assets and apply **date filters** (Tools → Past 24h/Week/Month):
