# 🔍 Social Media Lookup & Hidden Profiles OSINT Cheat Sheet

_Last verified: 2025-08-10 • Use ethically and comply with applicable laws, privacy regulations, and platform ToS._

---

## 🎯 Overview
Techniques and tools for discovering **hidden, pseudonymous, or private social media profiles**. Combine **manual investigative work** with **automation** to reveal digital footprints while respecting legal boundaries.

---

## 📡 What is SOCMINT?
**SOCMINT (Social Media Intelligence)** is the collection, analysis, and interpretation of data from social platforms for investigative, security, or analytical purposes.

**Primary Uses:**
- **Threat Analysis** — Identify potential risks or malicious actors.  
- **Cybersecurity** — Detect cyberstalking, impersonation, or fraud.  
- **Crisis Management** — Monitor events and emerging threats in real time.  
- **Brand & Reputation Management** — Counter fake profiles and misinformation.

---

## 🔎 Social Media Lookup
**Definition:**  
Locating accounts on platforms (Facebook, Instagram, X/Twitter, TikTok, LinkedIn, etc.) using publicly available information.

**Goals:**  
- Connect aliases or handles to real identities.  
- Find alternate or hidden accounts.  
- Expand subject profiles for verification or intelligence gathering.

---

## 🛠️ Methods to Find Hidden Profiles

### 1) Manual Lookups
- **Reverse Image Search** — Use Google Images, Yandex, or TinEye to find profile pictures elsewhere.  
- **Username Reuse Search** — Check for same/similar handles across platforms (namechk.com, whatsmyname.app).  
- **Email/Phone Search** — Facebook, LinkedIn, and some niche sites allow lookups via contact details (privacy settings permitting).  
- **Connections Mapping** — Review public followers/following lists, group memberships, and tagged posts.  

### 2) Automated OSINT Tools
- **Data Aggregators** — Tools that compile public profiles from multiple sources.  
- **Social Graph Visualisation** — Maltego, SpiderFoot, IntelligenceX for mapping relationships.  
- **Monitoring & Alerts** — Tools to flag changes in public profiles or mentions.  
- **Export & Analysis** — Save findings in CSV, JSON, PDF for structured reporting.

---

## 🌐 Google Dorking for SOCMINT
- **`site:`** — Restrict to a specific platform. Example:  
  `site:facebook.com "full name"`  
- **Quotes `" "`** — Force exact matches. Example:  
  `"Johnathan M. Doe"`  
- **Combine Operators** — Example:  
  `site:instagram.com "alias" "location"`  
- **Exclude Terms** — Example:  
  `site:twitter.com "username" -jobs`  

---

## 💡 Investigator Tips
- Always pivot from confirmed identifiers (username, email, image) to minimise false positives.  
- Cross-verify with at least **two independent sources** before confirming an account link.  
- Track changes over time — hidden profiles may become public temporarily.  
- Monitor groups and communities connected to known profiles.  

---

## ⚠️ Limitations & Ethics
- Respect platform ToS — avoid unauthorised access or automated scraping where prohibited.  
- Some search capabilities may be region-restricted or removed over time.  
- Consider the **false positive risk** of username matches without corroboration.  

---

## 📌 Documentation Checklist
For each identified profile:  
- Platform name & URL  
- Username/handle  
- Associated identifiers (email, phone, image hash)  
- Source & date found  
- Screenshots & archived link  
- Confidence level in association  
- Relevant context (how it links to investigation)

---

### 📜 Changelog (2025-08-10)
- Updated to align with current search operator behaviour.
- Added investigator tips and documentation checklist.
- Incorporated automation + manual hybrid workflow guidance.
