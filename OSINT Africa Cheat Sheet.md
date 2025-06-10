# 🕵️ OSINT in Africa: SOCMINT Cheat Sheet

> **Scope**: Social Media Intelligence (SOCMINT) strategies tailored to African contexts. Focuses on platform use, regional patterns, practical tools, and operational best practices.

---

## 🌍 Regional Platform Dominance

| Region           | Dominant Platforms                     | Notes                                                              |
|------------------|-----------------------------------------|--------------------------------------------------------------------|
| West Africa      | Facebook, WhatsApp, Instagram           | High WhatsApp group activity; Instagram used for business scams    |
| East Africa      | Telegram, TikTok, Twitter               | Telegram used for mobilization; TikTok spreading disinfo fast     |
| North Africa     | Facebook, YouTube, Twitter              | Twitter used for activism; YouTube for long-form propaganda        |
| Central Africa   | Facebook, WhatsApp                      | Encrypted WhatsApp groups common in political movements            |
| Southern Africa  | Facebook, Instagram, LinkedIn           | LinkedIn for corporate footprinting, Instagram scams rising        |

---

## 🔍 Account Discovery Tactics

- **Phone Number Pivoting**
  - Use Truecaller, Sync.me
  - Search numbers on Facebook for linked profiles
- **Username Reuse**
  - Tools: WhatsMyName, Sherlock, Maigret
- **Email Trace**
  - Search emails on haveibeenpwned, Hunter.io, Emailrep.io
- **Language + Slang Filter**
  - Use region-specific slang to narrow results (e.g. “Naija” for Nigeria)

---

## 🎯 Group & Network Infiltration

- **WhatsApp/Telegram Invite Links**
  - Use search operators like:  
    - `site:chat.whatsapp.com "Africa"`  
    - `site:t.me "Nairobi"`
- **Instagram & TikTok**
  - Follow hashtag trails, especially political or local slang hashtags
  - Monitor tagged locations
- **Facebook**
  - Join local buy/sell or job groups—these often double as info hubs

---

## 📊 SOCMINT Tools & Tactics

| Task                     | Tools / Techniques                                      |
|--------------------------|---------------------------------------------------------|
| Hashtag Tracking         | Brand24, Talkwalker, ExportComments, TikTokHashtags     |
| Geolocation from Media   | InVID, SunCalc, Google Earth, Mapillary                 |
| Account Analysis         | Twint, Followerwonk, InstaInsane                        |
| Telegram Archive & Search| Telegram Open Archive, Telegago                         |
| Facebook Investigation   | Facebook Graph Search (manual), Lookup-ID.com           |
| URL Metadata             | Unshorten.it, Redirect Detective                        |

---

## 🧠 Behavioral Analysis

- **Engagement Time Patterns**
  - Determine location/timezone via post timing consistency
- **Linguistic Profiling**
  - Analyze slang and language mix to infer ethnicity or region
- **Network Mapping**
  - Manual scraping + Maltego or Obsidian for visualization

---

## 🪤 Disinformation & Scam Detection

- **Red Flags**
  - Too-good-to-be-true giveaways, heavy emoji use, urgent calls to action
- **Typical Scams**
  - Crypto investments (West/East Africa)
  - Fake job offers (Southern Africa)
  - Romantic/military scams (Pan-African)
- **Image Verification**
  - Reverse image search: Yandex > Google > Bing
  - EXIF tools: Exif.tools, Metadata2Go

---

## 🛡️ OPSEC & Ethical Notes

- Always use burner accounts or VMs (Tails, Whonix)
- Consider regional laws on digital surveillance & privacy
- Build cultural context before interpreting content

---

## 🔗 Useful Boolean Operators (Custom for Africa)

- `"Giveaway" OR "Win a phone"` AND `site:facebook.com`
- `("scam alert" OR "419") AND ("Lagos" OR "Accra")`
- `"job offer" AND ("WhatsApp" OR "DM") AND site:instagram.com`

---

## 🧰 Bonus Tools Directory

- **African-Focused Telegram Channels**: Search public index on tgstat.com
- **Local News Feeds for OSINT**: Google Alerts + Feedly
- **Mobile Metadata**: Mobilsnumbuster, SimCard Info apps
- **Archive Sites**: Archive.ph, Ghost Archive, Wayback Machine

---

**⚠️ Disclaimer**: Always verify before acting. Regional dialects, misinformation, and anonymized sources demand high skepticism and cross-validation.

---
