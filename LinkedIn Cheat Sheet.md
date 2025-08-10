# LinkedIn OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only (no credentialed access). Use ethically and abide by local law & LinkedIn ToS._

## 1) Fast pivots (copy/paste)
- Profile (public): https://www.linkedin.com/in/{custom_or_numeric_id}
- Company page: https://www.linkedin.com/company/{company_id_or_slug}
- Group page: https://www.linkedin.com/groups/{group_id}
- Job listing: https://www.linkedin.com/jobs/view/{job_id}
- Search (keyword): https://www.linkedin.com/search/results/all/?keywords={keyword}
- Alumni tool: https://www.linkedin.com/school/{school_id}/people/

## 2) Discovery & collection workflow
1) Seed  
   - Start with a known name, company, school, or keyword.  
2) Expand entities  
   - From profiles: capture headline, summary, work history, education, skills, recommendations, and public activity.  
   - From company pages: record description, industry, size, HQ, employees on LinkedIn, and recent posts.  
3) Corroborate & date  
   - Cross-reference employment claims with press releases, company websites, or other social media.  
4) Capture  
   - Save canonical URLs, profile snapshots, and any public posts or comments.

## 3) Google pivots (public LinkedIn data)
site:linkedin.com/in "{full name}"  
site:linkedin.com/in "{keyword}" "{location}"  
site:linkedin.com/company "{company name}"  
site:linkedin.com/pub/dir "{first name}" "{last name}"  
_Use date filters for recent changes._

## 4) What each surface gives you
- **Public profile**: Name, headline, location, industry, about section, work and education history, skills, and public endorsements.  
- **Company page**: Overview, specialties, size, employee count, HQ location, and recent activity.  
- **Groups**: Title, description, member count, recent discussions (public groups only).  
- **Job listings**: Title, company, location, requirements, and post date.  

## 5) Cross-platform and handle pivoting
- LinkedIn usernames often differ from other platforms but bios and company names can be used to pivot.  
- Email addresses, phone numbers, and websites may appear in the “Contact info” section for public profiles.  

## 6) Third-party tools & archives (use cautiously)
- **Hunter.io** — extract potential emails from domains found on LinkedIn profiles.  
- **PhantomBuster**, **TexAu** — automation for data collection (requires login; ToS implications).  
- **Wayback Machine** — view older versions of profiles and company pages.  
**Caveats:** LinkedIn actively detects and blocks automated scraping; use sparingly and ethically.

## 7) Stabilizing URLs
- Public profile URLs can be customized; numeric IDs are permanent unless deleted.  
- Remove query strings like `?trk=...` for cleaner URLs.

## 8) Current 2025 behaviors
- Most profile data beyond name and headline requires login to view.  
- Logged-out Google cache previews may still show recent data but are updated irregularly.  
- “People also viewed” sidebar is sometimes hidden based on privacy settings.  

## 9) Rate limits, gating & tips
- Unauthenticated views are heavily restricted; pace logged-in views to avoid temporary blocks.  
- Use the alumni tool for large-scale pivoting on school networks.  
- Monitor “activity” section for recent posts, comments, and engagement clues.  

## 10) Documentation hygiene
- Record: profile/company URL, capture date (UTC), visible fields, and any pivots discovered.  
- Archive key details with screenshots for time-sensitive investigations.

### Changelog (2025-08-10)
- Added alumni tool URL pattern.  
- Updated notes on Google cache and login gating.  
- Refined Google pivot examples for better targeting.  
