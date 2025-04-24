# 🛒 Marketplace & Classifieds OSINT Cheat Sheet 🕵️‍♂️

**Purpose:** Investigate individuals, groups, or items across regional online marketplaces and classifieds. This includes identifying fraudulent listings, seller networks, stolen goods, or illicit services.

---

## 🌍 Region-Specific Marketplaces

### 🇺🇸 United States
- **Craigslist** – Major metro-based classifieds: vehicles, rentals, personals.
- **OfferUp / Letgo (now merged)** – Peer-to-peer item sales, often mobile-first.
- **Facebook Marketplace** – Common for local sales; can reveal identity through social profiles.
- **Armslist** – Firearms classifieds (controversial/legal grey area).

### 🇪🇺 Europe (General)
- **eBay Kleinanzeigen (Germany)** – Now **KleiderKreisel**, Germany's main P2P classifieds.
- **Leboncoin (France)** – Cars, property, jobs, and local sales.
- **Wallapop (Spain)** – App-based secondhand market.
- **Marktplaats (Netherlands)** – Broad classifieds portal.

### 🇳🇴🇸🇪🇩🇰 Scandinavia
- **FINN.no (Norway)** – Real estate, cars, jobs, and general classifieds.
- **Blocket.se (Sweden)** – Popular for secondhand goods and vehicles.
- **dba.dk (Denmark)** – Denmark’s leading private classifieds portal.

### 🌍 Africa
- **Jiji (Nigeria, Kenya, Uganda, Ghana)** – Dominant classified platform across West/East Africa.
- **Gumtree South Africa** – Similar to Craigslist; jobs, rentals, electronics.

### 🌍 Middle East
- **OpenSooq** – Widely used in Jordan, Iraq, Gulf countries for cars, housing, phones.
- **Haraj (Saudi Arabia)** – Dominant Arabic classifieds platform.
- **Dubizzle (UAE)** – Cars, rentals, jobs, and electronics.

### 🇷🇺 Russia & Post-Soviet
- **Avito.ru** – The #1 Russian classifieds site for jobs, goods, and more.
- **Youla.ru** – Mobile-first competitor to Avito.
- **Izi.kz / olx.kz (Kazakhstan)** – Common for local and regional buying/selling.

### 🇨🇳 China
- **58.com** – General classifieds (jobs, housing, cars).
- **Ganji.com** – Often used alongside 58; job and rental scams commonly flagged.
- **Taobao (C2C)** – While not a classic classifieds site, used for tracking sellers of banned/recalled goods.

### 🌏 Asia-Pacific
- **Carousell (Singapore, Malaysia, Taiwan, Philippines)** – Social classifieds app.
- **OLX India** – India’s widespread general classifieds.
- **Mercari (Japan)** – Consumer-to-consumer e-commerce (especially collectibles).

---

## 🧭 Investigation Techniques

### 1. **Seller Profile Analysis**
- Check usernames, phone numbers, profile photos, post timing.
- Compare across platforms (e.g., same number on Craigslist and Facebook Marketplace).

### 2. **Reverse Image Search**
- Extract and reverse search item photos:
  - Stolen goods: reused stock images, copied listings
  - Tools: Google Images, Yandex, TinEye

### 3. **Phone Number Tracing**
- Use TrueCaller, Sync.me, or regional reverse lookup tools.
- Search numbers in scam reporting databases (e.g., `scammer.info`, `numberguru.com`).

### 4. **Handle Pivoting**
- Use known usernames or seller handles in:
  - Forums, Reddit, Telegram marketplaces
  - Social platforms for seller identification (use Sherlock, WhatsMyName)

### 5. **Archived Listings**
- Use `archive.today` or `Wayback Machine` to capture disappearing listings.
- Some sites auto-expire posts — archive fast.

### 6. **Keyword Traps**
- Monitor unusual keywords or pricing (e.g., high-end goods at absurd discounts).
- Useful for scam spotting and sting setups (law enforcement context).

---

## 🧩 Advanced Correlation

- **Cross-reference item details** across platforms and countries.
  - Stolen vehicle VINs, serial numbers (IMEI), specific item IDs
- **Currency mismatch, language irregularities** = sign of offshore scammers
- **Compare GPS coordinates or location metadata** in image EXIF (where legal)

---

## ⚠️ Ethical & Legal Considerations

- ✅ Stick to public listings and user profiles.
- ❌ Do not attempt to access backend dashboards, impersonate buyers/sellers, or use scraping bots without permission.
- ⚖️ Be aware of GDPR, data localization laws, and platform TOS.
- 🧭 If working with law enforcement, follow proper evidence handling and chain-of-custody rules.

---

**Track smarter. Think globally. Investigate ethically.** 🛍️🕵️‍♀️
