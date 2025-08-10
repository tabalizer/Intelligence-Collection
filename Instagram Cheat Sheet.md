# Instagram OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only (no credentialed access). Use ethically and abide by local law & Instagram ToS._

## 1) Fast pivots (copy/paste)
- Profile (handle): https://www.instagram.com/{username}/
- Hashtag: https://www.instagram.com/explore/tags/{hashtag}/
- Location: https://www.instagram.com/explore/locations/{location_id}/{slug}/
  (Location IDs found via page source, third-party tools, or legacy patterns.)
- Post (shortcode): https://www.instagram.com/p/{shortcode}/
  (Shortcodes are base64-like strings in the post URL.)
- Reels: https://www.instagram.com/reel/{shortcode}/
- Stories:
  - Highlights: https://www.instagram.com/stories/highlights/{highlight_id}/
  - Current 24h stories require login (even for public accounts).

## 2) Discovery & collection workflow
1) Seed
   - Start with a known username, hashtag, or location ID.
2) Expand entities
   - From profile: handle, display name, bio, external URL, follower/following counts, public grid.
   - From post: caption text, hashtags, tagged users, location tag.
3) Corroborate & date
   - Note posted date (visible on post page / HTML meta). Use Google date filters when IG UI is limited.
4) Capture
   - Save stable URLs, screenshots, and pivots (handles, hashtags, locations).

## 3) Google pivots (bypass login walls / enhance recency)
site:instagram.com "{username}"
site:instagram.com inurl:/p/ "{keyword}"
site:instagram.com/explore/tags "{topic}"
site:instagram.com/explore/locations "{place name}"
(Apply date filters: Tools → Past 24h/Week/Month.)

## 4) What each surface gives you
- Profile: handle, display name, profile pic, bio, external link, follower/following counts (approx), public post grid.
- Post: caption, hashtags, tagged accounts, location, like/comment counts (variable), timestamp.
- Hashtag: public posts using the tag; related tags.
- Location: posts geotagged to a place.
- Reels: short video with caption/hashtags/tagged accounts.
- Highlights: persistent story collections.

## 5) Cross-platform and handle pivoting
- Reuse the same handle across platforms (IG, X/Twitter, TikTok, YouTube, Discord, Telegram).
- Follow bio links to websites/link hubs to enumerate additional identifiers (domains, emails, other socials).

## 6) Third-party viewers & archives (use cautiously)
- Examples: imginn, dumpor, insta-stories.online, pikdo.
- Caveats: coverage inconsistent; content may be stale; respect ToS and local law.

## 7) Stabilizing URLs
- Strip tracking params (e.g., ?utm_source=...) for canonical links.
  Before: https://www.instagram.com/p/ABC123/?utm_source=ig_web_copy_link
  After:  https://www.instagram.com/p/ABC123/

## 8) Current 2025 behaviors
- Web UI prompts for login after limited scroll; direct post/profile URLs often load without login.
- Hashtag/location pages show limited results when logged out.
- Stories require login except for public highlights.
- Reels often viewable when you have the direct URL.

## 9) Rate limits, gating & tips
- Heavy browsing when logged out triggers modal blocks; pace requests, clear cookies, or change IP.
- Use Google pivots to jump straight to target pages and avoid infinite scroll.
- EXIF is stripped; rely on page metadata and cross-platform corroboration.

## 10) Documentation hygiene
- Capture: canonical URL, capture time (UTC), entity type (profile/post/hashtag/location/reel/story/highlight), discovered pivots.
- Note any gating/unavailability for transparency.

### Changelog (2025-08-10)
- Updated Reels and Highlights URL patterns.
- Added current login wall behavior and practical bypass tips.
- Expanded Google pivot examples.
- Documented URL parameter stripping for stability.
