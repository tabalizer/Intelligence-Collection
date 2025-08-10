# Signal OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only. Use ethically and comply with local law, privacy regulations, and Signal’s ToS._

---

## 🎯 Purpose
Practical reference for what is and is not possible with Signal using only open sources. Signal is end-to-end encrypted and intentionally exposes very little public data. Most OSINT pivots are indirect — working from numbers, usernames, or links published elsewhere — and involve careful preservation of artifacts.

---

## 🛠 Public Entry Points
- signal.me links — Direct contact links shared by a user or organisation.
  - Format: https://signal.me/#eu/{token} (username-based)
  - Format: https://signal.me/#p/{phone} (phone-based)
- signal.group links — Public or semi-public group invite links.
  - Format: https://signal.group/#C{invite_token}
- Publication sources — These links/numbers are typically discovered in press releases, social media bios, websites, PDFs, GitHub READMEs, or resumes.

---

## 🔍 Discovery Workflow
1. Seed  
   Start with a known phone number, username/handle, domain, or Signal link found off-platform.
2. Search  
   Use search engines for:
     - site:signal.me "#eu" OR "#p"
     - site:signal.group "#C"
     - "Signal" AND ("contact me" OR "reach me on Signal") "{name/org}"
   Search social bios, code repositories, and documents.
3. Corroborate  
   Match the Signal contact to the subject using context like name, role, organisation, or associated accounts.
4. Capture  
   Screenshot with URL and timestamp visible.  
   Save archive URLs (Wayback, Archive.today).  
   Hash any downloaded files (SHA-256).

---

## 🧩 Pivoting Opportunities
- Phone number → reverse lookup, breach data, WHOIS/domain connections.
- Username → check reuse across other platforms.
- Linked domain → WHOIS, DNS history, certificate transparency logs.
- Group link → analyse source page for group theme and related entities.

---

## ⚠️ Limitations & Cautions
- No public user directory on Signal — all discovery relies on external publication.
- Group links can be revoked at any time.
- Avoid probing or testing numbers on Signal — may violate law or ToS.
- Do not access private groups or messages without explicit lawful authorisation.

---

## 📌 Search Recipes
site:signal.me "#eu" OR "#p" "contact" OR "reach me" OR "Signal"  
site:signal.group "#C" "{keyword or organisation name}"  
"Signal" AND ("contact" OR "reach me") "{full name}" "{company}"  
inurl:signal.me "{brand}" OR "{domain}"  
inurl:signal.group "{topic or campaign}"  

---

## 🛡 Preservation & Verification
- Preserve: screenshot + archive URL + capture date/time (UTC).
- Verify: ensure the contact is published by the actual person/org and appears in ≥2 independent sources.
- Context: document where and why the contact was published.
- Refresh: re-check quarterly — Signal contacts can change or expire.

---

## 🗂 Documentation Hygiene
Record in your case log:
- Entity/Subject name
- Raw Signal link/number
- Normalised phone number (E.164 format)
- Source URL(s)
- Archived URL(s)
- Capture date/time (UTC)
- Corroborating sources
- SHA-256 hashes for any downloaded files
- Analyst notes on limitations or risks

---

### 📜 Changelog (2025-08-10)
- Fully rewritten in single-block Markdown format.
- Removed nested code blocks to preserve formatting integrity.
- Matches format used in updated TikTok/X/Facebook sheets.
```
