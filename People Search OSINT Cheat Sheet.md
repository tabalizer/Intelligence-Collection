# 🧠 People Search OSINT Cheat Sheet 🔍

**Purpose:** Locate, verify, and correlate publicly available information about individuals using ethical OSINT techniques.

---

## 🛠️ Tools for People Search

| Tool                  | Description                                                    | Link                                             |
|-----------------------|----------------------------------------------------------------|--------------------------------------------------|
| **Pipl**              | Premium search for deep identity data, including emails and usernames. | [pipl.com](https://pipl.com)                     |
| **Spokeo**            | Aggregates social profiles, phone numbers, and home addresses. | [spokeo.com](https://www.spokeo.com)             |
| **Whitepages**        | Phone number and address lookup, reverse search features.       | [whitepages.com](https://www.whitepages.com)     |
| **TruePeopleSearch**  | Free people search engine offering phone, email, and relatives. | [truepeoplesearch.com](https://www.truepeoplesearch.com) |
| **FamilyTreeNow**     | Genealogy + public records, ideal for link analysis.            | [familytreenow.com](https://www.familytreenow.com) |

Bonus:
- **Radaris**, **BeenVerified**, **ZabaSearch**, and **PeekYou** offer additional pivots depending on jurisdiction and language.

---

## 🧭 Methodology & Techniques

### 1. **Name-Based Searches**
- Use multiple variations: full name, nicknames, maiden names.
- Apply quotation marks in search engines: `"First Last"` + city/state.
- Use tools like Google, Yandex, and DuckDuckGo for different index scopes.

### 2. **Email Address Lookup**
- Search past breaches using tools like:
  - **HaveIBeenPwned**, **Dehashed** (login required), **BreachDirectory**
- Pivot from email to social media with hunter.io or public email lookups.

### 3. **Phone Number Tracing**
- Use reverse lookup platforms:
  - Whitepages, NumLookup, TrueCaller
- Pivot phone numbers into messaging platforms (Telegram, WhatsApp).

### 4. **Social Media Profiling**
- Start with known usernames and handle pivoting (Sherlock, WhatsMyName).
- Analyze linked accounts, follower/following graphs, and bio patterns.
- Use Google and site-specific operators:
  - `site:facebook.com "John Doe"` or `inurl:"/john.doe"`

### 5. **Public Records Examination**
- Search property records, court documents, marriage licenses, or voter rolls (region dependent).
- In the U.S., use state/local .gov portals, or FOIA requests.
- Use FamilyTreeNow for connections between relatives and addresses.

---

## 🔄 Correlation Techniques

- **Cross-reference data**: name ⇄ email ⇄ phone ⇄ address ⇄ social.
- Use Maltego (Community Edition) or SpiderFoot HX to visualize relationships.
- Build identity timelines by combining:
  - Domain registrations
  - WHOIS email reuse
  - Past social bios and archived data

---

## ⚠️ Ethical Considerations

- ✅ Only access and analyze **publicly available** or **user-consented** data.
- ❌ Never attempt to access private accounts, databases, or paid info illegally.
- ⚖️ Be aware of data protection laws (GDPR, CCPA) and country-specific privacy laws.
- 🧭 Always have a clearly defined, ethical purpose for the search (e.g., due diligence, journalism, threat research).

---

**Stay sharp. Think critically. Work ethically.** 🚀🔍
