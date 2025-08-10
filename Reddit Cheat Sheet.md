# Reddit OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only (no credentialed access). Use ethically and abide by local law & Reddit ToS._

## 1) Fast pivots (copy/paste)
- User profile: https://www.reddit.com/user/{username}/
- Subreddit: https://www.reddit.com/r/{subreddit_name}/
- Post (submission): https://www.reddit.com/r/{subreddit_name}/comments/{post_id}/{slug}/
- Comment (direct link): https://www.reddit.com/r/{subreddit_name}/comments/{post_id}/comment/{comment_id}
- Search (keyword): https://www.reddit.com/search/?q={query}
- Search within subreddit: https://www.reddit.com/r/{subreddit_name}/search?q={query}&restrict_sr=1
- Old Reddit view (stable, simpler HTML): https://old.reddit.com/{path}

## 2) Discovery & collection workflow
1) Seed  
   - Start with known username, subreddit, or keyword.  
2) Expand entities  
   - From a user profile: gather posts, comments, karma, trophies, account creation date.  
   - From a subreddit: collect description, creation date, subscriber count, and rules.  
3) Corroborate & date  
   - Use post timestamps and context to cross-reference with external events.  
4) Capture  
   - Save canonical URLs, screenshots, and raw comment/post text.

## 3) Search operators
keyword1 keyword2 — standard AND search  
"exact phrase" — match exact wording  
author:{username} — posts/comments by a user  
site:{domain} — posts linking to a domain  
url:{keyword} — match URLs containing keyword  
title:{keyword} — search in post titles  
nsfw:yes — include NSFW content in search  
timestamp:{unix1}..{unix2} — search by Unix timestamp range (Reddit API/Pushshift only)  

## 4) External search engines (public content)
- Google: site:reddit.com "{keyword}"  
- Pushshift: https://pushshift.io / API mirrors for historical Reddit data  
- Redditsearch.io — advanced filters without login  

## 5) What each surface gives you
- **User profile**: Karma, posts, comments, cake day (creation date), subreddits frequented.  
- **Subreddit**: Rules, description, mod list, subscriber count, related communities.  
- **Post**: Title, body text, media links, engagement metrics, creation date.  
- **Comment**: Parent/child structure, author, timestamp, score.  

## 6) Cross-platform and handle pivoting
- Reddit usernames often appear on other platforms; search the handle across OSINT tools.  
- Linked domains in posts or comments can lead to other social profiles.  

## 7) Third-party tools & archives (use cautiously)
- **Reveddit.com** — view removed/deleted comments and posts.  
- **Camas.ai** — thread visualizer.  
- **Wayback Machine** — archived subreddit snapshots.  
**Caveats:** Pushshift data completeness varies after Reddit API changes in 2023–2024.

## 8) Stabilizing URLs
- Remove tracking params like `?utm_source=...` for clean links.  
- Old Reddit URLs (old.reddit.com) often render faster and more simply for scraping.

## 9) Current 2025 behaviors
- Reddit search logged-out is functional but sometimes omits results.  
- Older posts may load slowly due to API throttling.  
- Deleted accounts show as `[deleted]` but historical data may persist in archives.  

## 10) Rate limits, gating & tips
- Heavy browsing or scraping may trigger bot checks; rotate IPs if necessary.  
- Pushshift remains the most robust for historical analysis, but verify timestamps.  

## 11) Documentation hygiene
- Record: username, subreddit, post/comment URL, capture time (UTC), and any discovered pivots.  
- Archive screenshots for key evidence.

### Changelog (2025-08-10)
- Updated Pushshift status and alternatives.  
- Added URL patterns for posts and comments.  
- Included Old Reddit as a stable HTML source for scraping.  
