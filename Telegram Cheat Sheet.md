# Telegram OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only (no credentialed access). Use ethically and abide by local law & Telegram ToS._

## 1) Fast pivots (copy/paste)
- Public channel/group (t.me link): https://t.me/{channel_or_group_username}
- Message link (public): https://t.me/{channel_or_group_username}/{message_id}
- Invite link (may expire): https://t.me/+{invite_code}
- User profile: https://t.me/{username}
- Web preview: https://t.me/s/{channel_or_group_username} (view without client)

## 2) Discovery & collection workflow
1) Seed  
   - Start with known public username, channel link, or invite link.  
2) Expand entities  
   - From public channels: capture title, description, member count, message frequency, linked media, and pinned messages.  
   - From pinned messages: find invite links, related channels, or contact handles.  
3) Corroborate & date  
   - Use web previews (`/s/`) for timestamped browsing without installing Telegram.  
   - Cross-reference handles in other platforms.  
4) Capture  
   - Save canonical URLs, key screenshots, and export message history where permissible.  

## 3) Telegram-specific search tips
- Use in-app search for public channels and bots if you have the client installed.  
- Use external search engines:  
  site:t.me "{keyword}"  
  site:t.me/s/ "{keyword}"  
- Search engines index public channels but not private ones.  

## 4) What each surface gives you
- **Public channel/group page**: Title, description, member count, message list, media previews.  
- **Web preview (/s/)**: Publicly viewable messages with timestamps, limited media previews.  
- **Pinned messages**: Often contain onboarding info, rules, or related links.  
- **User profiles**: Username, display name, bio, profile picture, and public groups/channels (if visible).  

## 5) Cross-platform and handle pivoting
- Telegram handles often match usernames on X, Instagram, or other platforms.  
- Channel descriptions and pinned messages frequently include external links.  

## 6) Third-party search engines & tools
- **tgstat.com** — analytics and search for public Telegram channels.  
- **telemetr.io** — tracks channel stats and posts.  
- **tlgrm.eu** — channel discovery.  
**Caveats:** Coverage varies; some tools have limited free tiers.  

## 7) Stabilizing URLs
- `/s/` format is best for stable, direct viewing without the Telegram app.  
- Public username-based links are permanent unless the username changes.  

## 8) Current 2025 behaviors
- `/s/` links still functional for public content viewing without login.  
- Telegram web previews show up to ~10-15 most recent posts for some large channels when viewed logged out.  
- Many public channels have set “join to view history” — older messages may be hidden unless you join.  

## 9) Rate limits, gating & tips
- Web previews have minimal rate limiting; heavy scraping may trigger temporary blocks.  
- Private groups and invite-only channels are inaccessible without joining.  

## 10) Documentation hygiene
- Record: channel/group/user handle, capture time (UTC), link type (public/invite/web preview), and key discovered pivots.  
- Archive pinned messages and channel descriptions for context.  

### Changelog (2025-08-10)
- Confirmed `/s/` web preview still works for public channels.  
- Updated discovery tools list.  
- Added note on “join to view history” gating for some public channels.  
