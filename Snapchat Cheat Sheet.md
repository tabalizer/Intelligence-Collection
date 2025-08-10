# Snapchat OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only (no credentialed access). Use ethically and abide by local law & Snapchat ToS._

## 1) Fast pivots (copy/paste)
- Public profile: https://www.snapchat.com/add/{username}
- Snap Map (global): https://map.snapchat.com  
- Place-based view: https://map.snapchat.com/@{lat},{lng},{zoom}z
- Spotlight content: https://www.snapchat.com/spotlight
- Story Explorer (from map interface) for localized stories.

## 2) Discovery & collection workflow
1) Seed  
   - Start with known username, location, or observed Snap Map hotspot.  
2) Expand entities  
   - From public profiles: capture display name, username, profile picture, bio, and linked accounts (Bitmoji, external links).  
   - From Snap Map: identify hotspots, events, and local story clusters.  
   - From Spotlight: collect trending content and creator handles.  
3) Corroborate & date  
   - Use Snap Map’s timeline slider to approximate posting time.  
   - Cross-reference with external social posts or known events.  
4) Capture  
   - Save stable profile/add links, Snap Map coordinates, and screenshots (with timestamps).  

## 3) Snap Map usage
- Global view: browse trending areas and events.  
- Zoom to street-level to reveal specific story bubbles.  
- Time filter slider lets you view stories from the past ~24 hours.  
- “Our Story” content is curated and public; personal stories require connection or public profile access.  

## 4) What each surface gives you
- **Public profile**: Display name, username, Snapcode, bio, profile image, external links.  
- **Snap Map hotspot**: Approximate geolocation, related public snaps, time posted.  
- **Spotlight**: Short-form videos, creator handles, and engagement metrics.  
- **Event/Story Explorer**: Curated story collections tied to a specific theme or location.  

## 5) Cross-platform and handle pivoting
- Many Snapchat users link Instagram, TikTok, or YouTube in their bio—pivot accordingly.  
- Bitmoji avatars may be reused across platforms; visual match can aid attribution.  

## 6) Third-party viewers & archives (use cautiously)
- Snap Map content can be previewed via embedded maps on third-party sites, but coverage is incomplete.  
- Archived Snap Map datasets exist for research purposes—check academic OSINT repositories.  
**Caveats:** Limited retention; most snaps expire after 24 hours unless archived in Spotlight or public profiles.  

## 7) Stabilizing URLs
- Snap profile URLs are stable (`/add/{username}`).  
- Snap Map links contain coordinates and zoom level; copy directly from browser to preserve view.  

## 8) Current 2025 behaviors
- Snap Map is accessible without login on desktop browsers.  
- Spotlight content viewable without login if direct link is known.  
- Public profiles visible without login, but some elements (full story list) may be gated.  

## 9) Rate limits, gating & tips
- Snap Map usage without login is not heavily rate-limited, but heavy automated access may trigger blocks.  
- For geolocation work, record coordinates and zoom—map visuals may change quickly.  

## 10) Documentation hygiene
- Record: username, profile URL, Snap Map coordinates, capture time (UTC), type of content (profile/map/story/spotlight).  
- Note ephemeral nature—include archive screenshots or screen recordings when permissible.  

### Changelog (2025-08-10)
- Added direct Spotlight and Story Explorer references.  
- Updated Snap Map coordinate URL pattern.  
- Noted current guest-access capabilities for web users.  
