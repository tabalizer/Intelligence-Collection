# 🧠 User Handle Pivoting Cheat Sheet 🔍

**Purpose:** Identify digital footprints by tracing usernames across platforms to uncover associated accounts, behaviors, and identity links.

---

## 🛠️ Tools for Username Searches

| Tool             | Description                                                    | Link                                                                 |
|------------------|----------------------------------------------------------------|----------------------------------------------------------------------|
| **WhatsMyName**  | Search over 500 platforms for exact username matches.          | [whatsmyname.app](https://whatsmyname.app)                           |
| **Namecheckup**  | Checks username availability across domains and social media.  | [namecheckup.com](https://namecheckup.com)                           |
| **Maigret**      | Command-line tool for searching profiles across 1000+ sites.   | [GitHub](https://github.com/soxoj/maigret)                           |
| **Sherlock**     | Python-based scanner for usernames on social platforms.        | [GitHub](https://github.com/sherlock-project/sherlock)              |
| **Blackbird**    | Profile reconnaissance and link analysis for known usernames.  | [GitHub](https://github.com/p1ngul1n0/blackbird)                    |

---

## 🧭 Methodology & Techniques

### 1. **Exact Match Search**
- Run target username through tools like WhatsMyName or Sherlock.
- Confirm active profiles via profile photos, posting dates, or content overlap.

### 2. **Username Variations**
- Create permutations of the original handle:
  - Example: `johndoe` ➝ `john.doe`, `johndoe1`, `j0hnd03`, `doejohn`
- Use regular expressions or scripting for automation with Maigret/Sherlock.

### 3. **Reverse Image Search**
- Save and upload avatars or photos to:
  - [Google Images](https://images.google.com), [Yandex](https://yandex.com/images), [Bing Visual Search](https://www.bing.com/visualsearch)
- Identify reuse of avatars across platforms or fake identities.

### 4. **Email/User Handle Correlation**
- Check if email patterns match usernames (e.g., `j.doe@gmail.com` ⇄ `jdoe`).
- Run the email through:
  - HaveIBeenPwned
  - Dehashed (paid)
  - Hunter.io for domain-linked identities

### 5. **Cross-Platform Validation**
- Compare bios, profile pictures, writing style, timestamps.
- Look for linkages like:
  - Same PFP on GitHub and Twitter
  - YouTube channel links in TikTok bios
  - Linked email or domain in multiple profiles

---

## 🧩 Advanced Tactics

- **Metadata Scraping**: Where legal, analyze platform metadata (e.g., GitHub commits, Reddit post timing).
- **Correlation via Follow Graph**: Analyze shared followers/following lists.
- **Language + Emoji Fingerprint**: People often write similarly across platforms.

---

## ⚠️ Ethical Considerations

- ✅ Stick to public, voluntarily provided, or leaked data that is publicly indexed.
- ❌ Never brute-force or scrape behind logins.
- ⚖️ Respect all applicable privacy laws (GDPR, CCPA, etc.) and platforms' TOS.
- 🧭 Avoid bias: confirmation bias is a major risk in pivot investigations.

---

**Trace with care. Confirm with context. Pivot with ethics.** 🚀🔍
