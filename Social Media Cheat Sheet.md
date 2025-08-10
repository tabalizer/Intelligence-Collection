# Social Media OSINT Cheat Sheet (General)
_Last verified: 2025-08-10 • Scope: open-source collection only (no credentialed access). Designed as a high-level reference before pivoting to platform-specific sheets._

## 1) Purpose
To provide a unified checklist for investigating any social media platform, ensuring consistent methodology before diving into platform-specific OSINT techniques.

## 2) Discovery & collection workflow
1) Seed  
   - Start with one or more identifiers: handle, display name, phone number, email, image, or keyword.  
2) Expand entities  
   - Search platform-native and external search engines for the identifier.  
   - Pivot via hashtags, geotags, tagged accounts, shared media, or linked profiles.  
3) Corroborate & date  
   - Confirm account matches through profile pictures, bio text, posting style, location clues, and mutual connections.  
4) Capture  
   - Save stable profile/post URLs, screenshots, and metadata (timestamp, content type, engagement).

## 3) Universal search techniques
- Google dorking:  
  `"username" site:{platform}.com`  
  `"email@example.com" site:{platform}.com`  
  `"phone number" site:{platform}.com`  
- Hashtag search: `{platform_url}/explore/tags/{hashtag}`  
- Geotag search (if supported): `{platform_url}/explore/locations/{location_id}`  
- Image reverse search for profile pics or posted content.

## 4) Core OSINT surfaces on any platform
- **Profile page**: Handle, display name, bio, profile pic, external links, join date, follower/following counts.  
- **Posts**: Text, hashtags, tagged accounts, media, timestamps, engagement.  
- **Hashtag pages**: Trend clusters, recurring accounts.  
- **Location pages**: Posts tied to a place; potential for event detection.  
- **Media hosting links**: Sometimes reveal file naming patterns or metadata.

## 5) Cross-platform pivoting
- Handles reused across platforms.  
- External links in bios leading to other accounts.  
- Shared content (identical photo/video) uploaded to multiple platforms.  

## 6) Third-party tools & directories
- **WhatsMyName** — username checks across hundreds of sites.  
- **Namechk / Namecheckup** — username availability and discovery.  
- **Social Searcher** — mentions and hashtags across platforms.  
- **Exiftool** — check for retained metadata in images/videos (many platforms strip this).  
**Caveats:** Tools may have limited coverage or outdated data—verify matches manually.

## 7) Stabilizing URLs
- Remove tracking parameters (`?utm_source=...`) for long-term stable links.  
- Keep note of both the canonical and any shortened/redirected versions.

## 8) Current 2025 behaviors
- Most major platforms now gate significant content behind login; direct URL access still works in many cases.  
- Rate limits and anti-scraping measures have increased; rotate IPs and limit requests.  

## 9) Rate limits, gating & tips
- Use multiple accounts or logged-out browsing with clean sessions.  
- Archive important profiles/posts immediately—content can be removed at any time.

## 10) Documentation hygiene
- Record: platform name, URL, capture date (UTC), identifiers searched, pivots found, and match confidence.  
- Store findings in a structured format (CSV/JSON) for cross-referencing with other cases.

### Changelog (2025-08-10)
- Added unified search workflow for all platforms.  
- Expanded cross-platform pivot examples.  
- Updated notes on 2025 login gating and anti-scraping trends.
