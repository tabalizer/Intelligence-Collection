# Discord OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only (no credentialed access). Use ethically and abide by local law & Discord ToS._

## 1) Fast pivots (copy/paste)
- Invite link (public): https://discord.gg/{invite_code}
- Vanity invite: https://discord.gg/{custom_name}
- Server widget (if enabled): https://discord.com/widget?id={server_id}
- CDN file link: https://cdn.discordapp.com/attachments/{channel_id}/{message_id}/{filename}
- User profile (in-app only; no public web profile for non-partners)

## 2) Discovery & collection workflow
1) Seed  
   - Start with known invite link, CDN media link, or server name.  
2) Expand entities  
   - From invites: gather server name, icon, description, approximate member count.  
   - From server widgets: capture online member list, channel names, and presence info.  
   - From CDN links: identify originating server/channel IDs, file metadata.  
3) Corroborate & date  
   - Cross-reference usernames and IDs with other platforms.  
   - Use timestamp in CDN URL metadata or file properties.  
4) Capture  
   - Save invite codes, widget URLs, CDN file URLs, and relevant screenshots.

## 3) Discord-specific search tips
- Google dorking:  
  site:discord.gg "{keyword}" — find public invite links.  
  site:cdn.discordapp.com "{filename or keyword}" — locate hosted files.  
- Use `inurl:discord.com/invite` for variant formats.  

## 4) What each surface gives you
- **Invite link preview**: Server name, icon, description, member counts (approx), and join button.  
- **Server widget**: Real-time online members, text/voice channels, server ID.  
- **CDN file link**: Direct file access; path reveals channel and message IDs.  

## 5) Cross-platform and handle pivoting
- Discord usernames often contain identical branding as Twitch, Steam, or gaming-related accounts.  
- Server names/descriptions may list associated social links or websites.

## 6) Third-party tools & archives (use cautiously)
- **Disboard.org** — directory of public Discord servers.  
- **Discord.me**, **Top.gg** — community listings.  
- Archive invite previews via Wayback Machine before they expire.  
**Caveats:** Expired/vanity invites may be reused or reassigned.

## 7) Stabilizing URLs
- Discord invite codes are stable until revoked or expired.  
- CDN URLs remain active unless the file is deleted or the server is purged.

## 8) Current 2025 behaviors
- Invite previews work without login on desktop browsers.  
- Server widgets require server setting to be enabled; not all servers have them public.  
- CDN links remain accessible without login unless access controls are applied post-upload.

## 9) Rate limits, gating & tips
- Discord applies rate limits to API calls and excessive link previews; pace access.  
- Avoid automated joining of servers without permission—breaches ToS.

## 10) Documentation hygiene
- Record: server name, ID, invite code, CDN URLs, capture time (UTC), and any pivoted external links.  
- Archive server description text and member counts for context.

### Changelog (2025-08-10)
- Confirmed invite preview and widget behavior without login.  
- Updated Google dork examples for CDN and invite discovery.  
- Added note on stability of CDN URLs and server ID extraction.
