# Forum & Community Monitoring OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only (no credentialed access). Use ethically and abide by local law & platform ToS._

## 1) Types of forums & communities
- **Traditional web forums** (phpBB, vBulletin, XenForo, SMF)
- **Special interest communities** (hobby, tech, sports, etc.)
- **Dark web forums** (Tor hidden services)
- **Q&A platforms** (Stack Exchange, Quora)
- **Niche regional boards** (language or country-specific)

## 2) Discovery & collection workflow
1) Seed  
   - Start with known username, email, topic keyword, or domain.  
2) Expand entities  
   - From user profiles: capture join date, post history, location (if shared), contact links.  
   - From posts: identify writing style, recurring topics, and external links.  
3) Corroborate & date  
   - Compare registration details across multiple forums.  
   - Use quotes from posts in search engines to find other occurrences.  
4) Capture  
   - Archive profile pages, threads, and media attachments.

## 3) Search techniques
- Google dorking:  
  `"keyword" site:forumdomain.com`  
  `site:boardreader.com "{keyword}"` (if indexed)  
- Use advanced search features on forum software (by user, date, keyword).  
- Search post excerpts in quotes to locate cross-posts.

## 4) What each surface gives you
- **Profile page**: Join date, post count, last active date, contact info, signature block.  
- **Thread page**: Original post, replies, timestamps, usernames.  
- **Attachment/media links**: Sometimes retain EXIF data or filenames revealing device info.

## 5) Cross-platform and handle pivoting
- Forum handles often reused on Reddit, Discord, and gaming platforms.  
- Signature blocks and profile bios may contain social media links, websites, or email addresses.

## 6) Third-party tools & archives (use cautiously)
- **Wayback Machine** — recover deleted threads or profiles.  
- **Archive.today** — capture full pages without JavaScript issues.  
- **ahmia.fi** — Tor hidden service search engine (for dark web forums).  
**Caveats:** Dark web access requires Tor; follow local laws.

## 7) Stabilizing URLs
- Many forums use numeric thread IDs in URLs—these remain stable even if titles change.  
- Example: `viewtopic.php?t=12345` will still work if the thread is renamed.

## 8) Current 2025 behaviors
- Many forums are moving to closed or invite-only registration to reduce spam.  
- Search engines increasingly exclude forum content unless specifically dorked.  
- Mobile-friendly skins sometimes hide metadata—check desktop view for full info.

## 9) Rate limits, gating & tips
- Some forums block guest access to profiles—create passive accounts for viewing.  
- Use multiple archive services to capture volatile threads.

## 10) Documentation hygiene
- Record: forum URL, profile/thread link, capture date (UTC), username, post excerpts, and discovered pivots.  
- Archive key threads as PDF or static HTML.

### Changelog (2025-08-10)
- Added notes on invite-only trend and mobile skin limitations.  
- Updated dark web discovery tools list.  
- Expanded Google dork examples for forum-specific targeting.
