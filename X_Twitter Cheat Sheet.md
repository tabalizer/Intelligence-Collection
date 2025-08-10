# X (Twitter) OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only (no credentialed access). Use ethically and abide by local law & X/Twitter ToS._

## 1) Fast pivots (copy/paste)
- Profile (handle): https://x.com/{username} or https://twitter.com/{username}
- Tweet (ID): https://x.com/{username}/status/{tweet_id}
- Search (keyword): https://x.com/search?q={query}
- Search (hashtag): https://x.com/hashtag/{hashtag}
- Search with filters: https://x.com/search?q={query}%20filter%3Amedia (replace `filter%3Amedia` with other operators from §3)
- Lists: https://x.com/{username}/lists
- Moments: https://x.com/i/moments/{moment_id}
- Spaces: https://x.com/i/spaces/{space_id}

## 2) Discovery & collection workflow
1) Seed  
   - Start with a known username, hashtag, or keyword.  
2) Expand entities  
   - From a tweet: capture handle, display name, timestamp, media URLs, hashtags, mentions, quoted/replied-to accounts.  
   - From a profile: capture bio text, location, URL, join date, follower/following counts, pinned tweet.  
3) Corroborate & date  
   - Use advanced search filters for date ranges, media types, or engagement thresholds.  
4) Capture  
   - Save canonical URLs, full text, media links, and IDs. Consider archiving with the Wayback Machine.  

## 3) Advanced search operators (web)
from:{username} — tweets from a specific user  
to:{username} — tweets sent to a specific user  
@{username} — tweets mentioning a user  
"exact phrase" — exact phrase search  
keyword1 OR keyword2 — logical OR search  
-filter:replies — exclude replies  
filter:media — tweets with any media  
filter:images — tweets with images  
filter:videos — tweets with videos  
filter:links — tweets with URLs  
min_retweets:10 — tweets with at least 10 retweets  
since:2025-01-01 until:2025-02-01 — tweets between dates (UTC)  
lang:en — limit to English tweets  

## 4) What each surface gives you
- Profile: Handle, display name, bio, location, external URL, join date, follower/following counts, pinned tweet.  
- Tweet: Full text, hashtags, mentions, media URLs, timestamp, engagement counts.  
- Hashtag pages: Tweets containing the hashtag; related tags may appear in suggestions.  
- Lists: Curated account collections (public lists only).  
- Spaces: Live audio sessions with metadata (title, participants, start time).  

## 5) Cross-platform and handle pivoting
- Reuse the same handle on other platforms to map an identity graph.  
- External links in bio often lead to link hubs, personal sites, or other social accounts.  

## 6) Third-party tools & archives (use cautiously)
- nitter.net instances (privacy-friendly mirrors; availability varies)  
- Social Bearing, Twiangulate, Twitonomy (analytics and search)  
- Wayback Machine for historical snapshots  
Caveats: Rate limits, coverage issues, and possible ToS implications—use ethically.  

## 7) Stabilizing URLs
- Remove tracking parameters for clean links:  
  Before: https://x.com/user/status/1234567890?ref_src=twsrc%5Etfw  
  After:  https://x.com/user/status/1234567890  

## 8) Current 2025 behaviors
- Web search may require login for full results; direct URLs often load without login.  
- Viewing replies to sensitive tweets may be gated.  
- Older tweets (>3200 from a user) require third-party archives or API access.  
- Spaces metadata visible without joining if you have the space URL.  

## 9) Rate limits, gating & tips
- Heavy unauthenticated browsing triggers login prompts; pace activity or rotate IPs.  
- Advanced search via URL is more stable than the on-page interface.  
- Save tweet IDs—they are immutable and can be used with multiple tools.  

## 10) Documentation hygiene
- Record: canonical URL, tweet ID, capture time (UTC), account ID, and any linked entities.  
- Archive media separately; X/Twitter sometimes removes media while keeping tweet text.  

### Changelog (2025-08-10)
- Updated advanced search operators to reflect current support.  
- Added Spaces URL pattern and current metadata visibility.  
- Noted current search/login gate behavior.  
- Included nitter and archive usage as auxiliary discovery methods.  
