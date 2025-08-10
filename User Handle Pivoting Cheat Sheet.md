# User Handle Pivoting OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only (no credentialed access). Use ethically and abide by local law & platform ToS._

## 1) Purpose
User handle pivoting is the process of taking a known username or handle from one platform and finding the same or related handles across other platforms, services, and datasets. This helps build an identity graph and uncover related accounts.

## 2) Discovery & collection workflow
1) Seed  
   - Start with one confirmed handle from a trusted source.  
2) Expand entities  
   - Search exact handle across multiple social media, forums, marketplaces, and gaming platforms.  
   - Look for close variants (leet speak, underscores, numbers, shortened forms).  
3) Corroborate & date  
   - Verify matches by comparing bio text, profile pictures, posting style, and linked websites.  
4) Capture  
   - Save URLs, screenshots, and metadata for each matched profile.

## 3) Search techniques
- Manual Google/Bing search: `"username" site:twitter.com OR site:instagram.com ...`  
- Specialized tools:  
  - **WhatsMyName** (whatsmyname.app) — checks hundreds of platforms.  
  - **Namechk.com** — checks username availability across domains and platforms.  
  - **Namecheckup.com** — similar to Namechk, with extended coverage.  
- API-based queries (where allowed) to confirm username existence.

## 4) What each surface gives you
- **Social media profiles**: Bio text, external links, posting frequency.  
- **Gaming handles**: Achievements, associated communities.  
- **Marketplaces**: Seller ratings, item listings, contact info.  
- **Forums/communities**: Post history, join date, topic focus.

## 5) Cross-platform patterns to check
- Same handle reused exactly across multiple services.  
- Handle plus a predictable number suffix (e.g., johnsmith → johnsmith123).  
- Reverse of handle or initials combined with numbers.  
- Domain names registered matching handle.

## 6) Third-party tools & archives (use cautiously)
- **Namecheckup** — profile and domain search.  
- **Usersearch.org** — cross-platform profile discovery.  
- **Social-Searcher.com** — keyword and handle mentions across social/web.  
- **Wayback Machine** — historical username use on now-deleted profiles.  
**Caveats:** Many tools return false positives—manual verification is essential.

## 7) Stabilizing URLs
- Store canonical profile URLs without session or referral parameters.  
- Example: `https://x.com/username` instead of `https://x.com/username?ref=xyz`.

## 8) Current 2025 behaviors
- Some major platforms hide profiles from public search unless logged in—tools may miss these.  
- Username squatting and impersonation can lead to false matches; check join date and content.  

## 9) Rate limits, gating & tips
- Many username checkers have request limits—rotate between services.  
- Consider batch lookups in low-volume intervals to avoid tool throttling.

## 10) Documentation hygiene
- Record: handle searched, platforms checked, matched URLs, match confidence level, capture time (UTC).  
- Maintain a pivoting log to track search coverage and reduce duplicate effort.

### Changelog (2025-08-10)
- Added updated username discovery tools with 2025 coverage.  
- Expanded common handle variant patterns to investigate.  
- Included verification tips to reduce false positives.
