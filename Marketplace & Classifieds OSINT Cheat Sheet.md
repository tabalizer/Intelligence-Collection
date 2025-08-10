# Marketplace & Classifieds OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only (no credentialed access). Use ethically and abide by local law & platform ToS._

## 1) Common marketplaces & classified platforms
- **Facebook Marketplace**: https://www.facebook.com/marketplace/  
- **Craigslist**: https://www.craigslist.org/  
- **eBay**: https://www.ebay.com/  
- **Leboncoin** (FR): https://www.leboncoin.fr/  
- **Gumtree** (UK/AU): https://www.gumtree.com/  
- **OLX** (various countries): https://www.olx.com/  
- **Finn.no** (NO): https://www.finn.no/  
- **Avito** (RU): https://www.avito.ru/  
- **Car and property portals** vary by region (e.g., Autotrader, Zillow).

## 2) Discovery & collection workflow
1) Seed  
   - Start with seller username, phone number, email, or listing ID.  
2) Expand entities  
   - From listings: capture title, description, price, location, seller profile, contact details, and images.  
   - Reverse search images for reused photos across platforms.  
3) Corroborate & date  
   - Check identical item descriptions on multiple platforms.  
   - Cross-reference phone/email in OSINT people search tools.  
4) Capture  
   - Save listing URL, screenshots, posted date, and any seller identifiers.

## 3) Search techniques
- Google dorking:  
  `"keyword" site:facebook.com/marketplace`  
  `"keyword" site:craigslist.org`  
  `"phone number" OR "email"` across marketplaces.  
- Use cached pages from Google or Bing to access removed listings.  
- Search image hashes on Yandex, Google Lens, TinEye.

## 4) What each surface gives you
- **Listing page**: Item details, seller info, posted date, location.  
- **Seller profile**: Other items for sale, join date, reviews/ratings.  
- **Image metadata**: Occasionally retained on less-moderated sites (EXIF may reveal GPS).  

## 5) Cross-platform and handle pivoting
- Many sellers use same phone/email across multiple marketplaces and social media.  
- Reused images often lead to original source or additional listings.

## 6) Third-party tools & archives (use cautiously)
- **SearchTempest** — multi-city Craigslist search.  
- **Wayback Machine** — historical listing snapshots.  
- **OSINT Combine Image Tools** — bulk reverse image search.  
**Caveats:** Platform ToS may prohibit automated scraping—review before use.

## 7) Stabilizing URLs
- Some platforms include session or referral parameters—strip for a clean permanent link.  
- Example: Remove `?ref=...` from Facebook Marketplace URLs.

## 8) Current 2025 behaviors
- Facebook Marketplace restricts some views without login; direct listing URLs sometimes bypass this.  
- Craigslist remains fully public; older posts are removed after ~30-45 days.  
- Many regional classifieds hide seller contact until logged in or inquiry sent.

## 9) Rate limits, gating & tips
- Heavy image reverse searches may trigger rate limits—spread across multiple engines.  
- Use VPN/location spoofing for region-locked marketplaces.

## 10) Documentation hygiene
- Record: listing URL, capture date (UTC), seller handle, contact details, item description, price, and photos.  
- Archive screenshots and downloaded images for analysis.

### Changelog (2025-08-10)
- Added Facebook Marketplace login bypass notes.  
- Updated reverse image search recommendations.  
- Listed top regional marketplace URLs for OSINT reference.
