# People Search OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only (no credentialed access). Use ethically and abide by local law & data protection rules._

## 1) Common people search engines & directories
- **Pipl** — https://pipl.com (paid, deep web coverage)
- **TruePeopleSearch** — https://www.truepeoplesearch.com (US-focused)
- **FastPeopleSearch** — https://www.fastpeoplesearch.com (US-focused)
- **411.com** — https://www.411.com
- **Whitepages** — https://www.whitepages.com
- **Spokeo** — https://www.spokeo.com (paid)
- **ThatsThem** — https://thatsthem.com
- **WebMii** — https://webmii.com
- **PeekYou** — https://peekyou.com

## 2) Discovery & collection workflow
1) Seed  
   - Start with name, email, phone number, or username.  
2) Expand entities  
   - From search results: capture full name variations, addresses, relatives, age ranges.  
   - Identify linked social media accounts, domains, or other contact info.  
3) Corroborate & date  
   - Verify addresses against property records, business registrations, or recent public mentions.  
4) Capture  
   - Save URLs, screenshots, and structured data (names, addresses, contact numbers).

## 3) Search techniques
- Google dorking:  
  `"full name" "city" site:linkedin.com`  
  `"email@example.com"`  
  `"phone number" site:facebook.com`  
- Use reverse image search for profile pictures to locate accounts on other sites.  
- Search by username across multiple platforms using **Namechk** or **WhatsMyName**.

## 4) What each surface gives you
- **Public directories**: Name, address history, phone numbers, relatives, age ranges.  
- **Social media profiles**: Photos, employment, education, connections.  
- **Property records**: Ownership history, valuations, mortgage details (varies by jurisdiction).  

## 5) Cross-platform and handle pivoting
- Email addresses and usernames can be used to search dozens of platforms.  
- Reverse WHOIS lookups may reveal domains registered by the person.

## 6) Third-party tools & archives (use cautiously)
- **HaveIBeenPwned** — breach data lookup for email addresses.  
- **Hunter.io** — email pattern discovery for organizations.  
- **Wayback Machine** — old versions of social profiles and directories.  
**Caveats:** Some people search sites scrape outdated or inaccurate data—always corroborate.

## 7) Stabilizing URLs
- Many directory links include search session parameters—strip these for a clean URL.  
- Example: Remove `?searchId=...` from Whitepages results.

## 8) Current 2025 behaviors
- Many free people search services have moved to paid models; US-centric services still have strong open coverage.  
- GDPR and similar laws limit EU visibility—pivot to social media, public registers, and news sources.

## 9) Rate limits, gating & tips
- Automated lookups can trigger CAPTCHAs; rotate services for heavy research.  
- Focus on cross-referencing rather than single-source reliance.

## 10) Documentation hygiene
- Record: source name, URL, capture date (UTC), identifiers searched, and key findings.  
- Archive structured findings in CSV/JSON for easy cross-referencing.

### Changelog (2025-08-10)
- Added updated people search engines list with 2025 availability.  
- Included GDPR impact notes.  
- Expanded Google dork examples for multi-field targeting.
