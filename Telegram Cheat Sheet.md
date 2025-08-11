# Telegram OSINT Master Cheat Sheet
_Last verified: 2025-08-11 • Scope: open-source collection only (no credentialed access). Use ethically and abide by local law & Telegram ToS._

## 1) Purpose
A concise, global, platform-agnostic reference for finding, pivoting, verifying, and documenting open Telegram data (usernames, public channels/groups, messages, phone numbers, emails) without breaching privacy, law, or ToS.

## 2) Why Telegram Matters for OSINT
- Hybrid model: **encrypted private chats** + **public channels/groups** = large open data surface.
- Public selectors (usernames, message links, media, outlinks) enable cross-platform pivots.
- Key use cases: disinformation mapping, protest/event monitoring, cybercrime/fraud tracking, due diligence, threat intelligence.

## 3) Core Entity Types
- **Profiles/Usernames** — `@handle` visible in public contexts.
- **Channels/Groups** — public or invite-only; often interconnected via pinned posts/links.
- **Messages/Media** — posts, forwards, captions, attachments, external links.
- **Contact Selectors** — phone numbers/emails sometimes exposed in bios, descriptions, pinned messages, or recruitment posts.

## 4) Fast Pivots
- Public channel/group: `https://t.me/{channel_or_group_username}`
- Message (public): `https://t.me/{channel_or_group_username}/{message_id}`
- Invite link (may expire): `https://t.me/+{invite_code}`
- User profile: `https://t.me/{username}`
- Web preview (no client): `https://t.me/s/{channel_or_group_username}`

## 5) Discovery & Collection Workflow (SEED → EXPAND → CORROBORATE → CAPTURE)
1) **Seed** — start with a username, channel link, invite link, or keyword.
2) **Expand** — collect title, description, member count, posting cadence, pinned messages, linked channels, and outlinks.
3) **Corroborate** — use `/s/` web preview for timestamped browsing; pivot handles to other platforms; verify media externally.
4) **Capture** — store canonical URLs, screenshots, hashes, and (where permissible) exports for reproducibility.

## 6) Search Tactics
**External engines:**
site:t.me "{keyword}"
site:t.me/s/ "{keyword}"
site:t.me "username"
site:twitter.com "username"
site:github.com "username"
"Telegram: @username"
"contact me on Telegram"

- Add context terms: `"contact us"`, `"admin"`, `"rules"`, `"apply"`, `"email"`, `"phone number"`.
- Run queries in multiple languages and with synonyms.

**In-app:**
- Use global search by keyword/handle; inspect “linked channels” and pinned posts for networks and selectors.

## 7) Profile / Username OSINT
- Extract display name, bio, profile photo, visible group/channel memberships.
- Cross-match handles with:
  - [WhatsMyName](https://whatsmyname.app/)
  - [NameChk](https://namechk.com/)
  - [Maigret](https://github.com/soxoj/maigret)
  - [Maltego](https://www.maltego.com/)
  - [OSINT Industries](https://www.osint.industries/)
- Look for avatar reuse, identical bios, and contact details across platforms.

## 8) Phone Number OSINT
- **Contact-sync check** (if policy allows): saving a number in your device may reveal a linked Telegram profile if user settings allow.
- Search for numbers in public descriptions or pinned messages:
  - `"phone number" site:t.me`
  - `"contact us" site:t.me`
  - `"admin" site:t.me`
- Reverse lookup services:
  - [Truecaller](https://www.truecaller.com/)
  - [Sync.me](https://sync.me/)
  - [OSINT Industries Phone Lookup](https://www.osint.industries/)

## 9) Email OSINT
- Scan recruitment/professional groups and pinned messages:
  - `"email" site:t.me`
  - `"send your CV" site:t.me`
  - `"resume" OR "CV" site:t.me`
- Cross-reference:
  - `"Telegram: @username" site:linkedin.com`
  - `"Contact me on Telegram" site:github.com`
- Tools:
  - [Hunter.io](https://hunter.io/)
  - [EmailRep.io](https://emailrep.io/)
  - [OSINT Industries Email Lookup](https://www.osint.industries/)

## 10) Third-Party Telegram Search & Analytics
- [TGStat](https://tgstat.com/) — analytics/search for public channels.
- [Telemetr.io](https://telemetr.io/) — post tracking & stats.
- [Tlgrm.eu](https://tlgrm.eu/) — channel discovery.
- [Telegago (CSE)](https://cse.google.com/cse?cx=006368593537057042503:efxu7xprihg) — Google custom search for Telegram.
**Caveat:** Indexing coverage and history depth vary; free tiers are limited.

## 11) Media Verification & Archiving
- Reverse image/video: [Yandex Images](https://yandex.com/images/), [TinEye](https://tineye.com/), [Google Images](https://images.google.com/).
- Video forensics: [InVID plugin](https://www.invid-project.eu/tools-and-services/invid-verification-plugin/).
- Archiving: [archive.ph](https://archive.ph/), [Wayback Machine](https://web.archive.org/), [Hunchly](https://www.hunch.ly/).
- Preserve captions, forwards, and outlinks with the media.

## 12) Stabilizing URLs & Current Behaviors (2025)
- `/s/` previews work for public viewing without login; large channels may only show recent posts when logged out.
- Some public channels set “join to view history” — older messages hidden until you join.
- Username-based URLs remain stable unless the username changes.

## 13) Rate Limits & Gating
- Web previews have light rate limiting; high-volume scraping can trigger blocks.
- Private/invite-only spaces remain inaccessible without joining.
- Actor ecosystems often mirror across Telegram, X, Discord, and forums.

## 14) Ethics & Legal Boundaries
- Public data only — never access private messages or restricted resources.
- Respect [Telegram ToS](https://telegram.org/tos) — no automated scraping without permission.
- Avoid phishing, social engineering, hacking.
- Maintain data minimization, retention limits, and secure storage.

## 15) Documentation Hygiene
- Log: handle, channel URL, capture time (UTC), link type (public/invite/web preview), and pivots.
- Take screenshots, export messages where allowed, record hashes.
- Note any language/context relevant to the capture.

## 16) Investigative Recipes
- **Username → Multi-platform map**: `site:t.me "username"` → `/s/` review → cross-match with WhatsMyName/NameChk → archive.
- **Contact discovery**: `"email" OR "phone number" site:t.me` → reverse lookup for validation.
- **Channel network mapping**: extract linked channels from pinned/description → analyze with TGStat/Telemetr.
- **Disinfo chain trace**: capture seed post → hash/reverse-search media → compare timestamps across `/s/`, X, YouTube → archive.
- **Alerting**: use Visualping/Distill on `/s/` pages; re-run saved dorks regularly.

## 17) Global Dork Pack
site:t.me "contact us"
site:t.me "phone number"
site:t.me "email"
site:t.me "admin"
site:t.me "rules"
site:t.me "apply"
site:t.me "resume" OR "CV"
site:t.me "LinkedIn"
site:t.me "GitHub"
site:t.me "Signal" OR "WhatsApp" OR "Discord"
site:t.me "press release" OR "announcement"
site:t.me "white paper"
site:t.me "API key" OR "token" (lawful use only)
site:t.me/s/ "live" OR "breaking"
"Telegram: @username" site:linkedin.com
"Contact me on Telegram" site:github.com
site:t.me inurl:/s/ "has joined"
site:t.me "pinned message"
site:t.me "channel rules"


### Changelog (2025-08-11)
- Delivered as a single, uninterrupted markdown code block.
- Global scope only — no regional references.
- Added full tool links, investigative workflows, and dork pack.
