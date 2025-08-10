```markdown
# OSINT Africa Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only. Use ethically and comply with local law, privacy regulations, and platform ToS._

---

## 🎯 1) Purpose
Practical, country-aware pivots for investigations across the African continent: people/org discovery, corporate records, phones, media, geolocation, and due-diligence checks.

---

## 🧭 2) Discovery Workflow (FAST)
1) **Frame** the target: person/org/phone/domain/place + country/region.  
2) **Aggregate** pan-African sources (news, registries, NGO/open-data portals).  
3) **Substitute** local languages/terms (Fr/Ar/Sw/Am/Ts + local spellings).  
4) **Triangulate** with at least one independent, off-platform source per fact.

---

## 🌍 3) Pan-African Meta Sources
- **News/meta indexes:** AllAfrica, AfricaNews, The Africa Report, ISS Today (Institute for Security Studies), Afrobarometer.  
- **Corporate/Trade:** African Development Bank project database; COMESA/SADC/ECOWAS publications; UNGM & World Bank procurement.  
- **Open data portals:** data.humdata.org (HDX), World Bank Data, UN OCHA ReliefWeb, OpenAFRICA (codeforafrica.org).  
- **Sanctions/PEP:** UN / EU / OFAC consolidated lists; regional PEP lists via local watchdog NGOs.  
- **Maps & crises:** ACLED (conflict), MapAction, OpenStreetMap Africa, satellite disaster maps (ReliefWeb).

---

## 🏢 4) Company & NGO Checks (by region/language)
> Many official registries limit search or require fees. Use press releases, tax/Gazette notices, and procurement records to corroborate.

- **Anglophone (sample):**  
  - **Nigeria:** CAC (Corporate Affairs Commission) search; NGX news; FIRS notices.  
  - **Kenya:** eCitizen Business Registration; PPRA tenders; NGO Board register.  
  - **Ghana:** RGD (Registrar-General) basics; Public Procurement Authority; Registrar of Companies Gazette.  
  - **South Africa:** CIPC (entities & docs), CIPRO legacy, Government Gazette; CSD supplier database.  
  - **Uganda/Tanzania/Zambia:** BRELA (TZ), PACRA (ZM), URSB (UG) basic searches + Gazettes/procurement.

- **Francophone (sample):**  
  - **OHADA** space: RCCM numbers appear in Gazettes/court bulletins; Journal Officiel per country.  
  - **Senegal/Côte d’Ivoire/Benin:** Journal Officiel + tax/GUFE portals; BCEAO filings for banking notices.  
  - **DRC:** GUCE/Journal Officiel; RCCM references in legal notices.

- **Lusophone (sample):**  
  - **Angola/Mozambique:** Diário da República, IGEPE/AIPEX releases; company bulletins and procurement portals.

- **Maghreb/Arabic (sample):**  
  - **Morocco:** OMPIC (RC/ICE searches), BO (Bulletin Officiel), CNSS employer lists.  
  - **Tunisia:** INNORPI trademarks, JORT (Journal Officiel), RNE enterprise search.  
  - **Egypt:** GAFI business registry basics, EGX disclosures; Egyptian Gazette.

> Where official lookup is closed, pivot via: **Gazettes**, **stock exchange filings**, **tax/VAT lists**, **tender portals**, **court bulletins**, and **press releases**.

---

## 👤 5) People/Identity Pivots
- **Local platforms:** Facebook, X, Instagram, TikTok (high penetration); LinkedIn for formal roles.  
- **Name variants:** Consider French/Arabic transliteration, compound surnames, maiden names, Yoruba/Igbo/Akan name order, Arabic nisbas, Portuguese diacritics.  
- **Media hits:** Community radio websites, church/mosque bulletins, alumni groups, union pages.  
- **Education:** University graduation lists/newsletters; professional councils (medical, law, engineering) per country.

---

## ☎️ 6) Phones & Messaging (very important)
- **E.164 formatting**; validate with country plans. Mobile dominance is high; multiple SIMs common.  
- Check in **Truecaller/Numlookup** (coverage varies), WhatsApp/Telegram contact presence (lawfully), and marketplace listings.  
- **Mobile money** context: M-Pesa (KE/TZ), MTN Mobile Money (GH/NG/UG/CM), Orange Money (Francophone). Mentions may appear in classifieds/receipts.

---

## 🛰 7) Geolocation & Places
- **OpenStreetMap Africa** (often better detail than commercial basemaps in rural areas).  
- **Mapillary/Street View** coverage uneven—pivot to **YouTube vlogs**, local real-estate tours, and **Facebook event photos**.  
- **Official gazetteers:** national statistics offices often publish admin boundaries; HDX hosts shapefiles.  
- **Languages on signs**: Arabic/French/Portuguese/local scripts help narrow region quickly.

---

## 💬 8) Languages & Search Recipes
- **French:** *“avis d’attribution”, “journal officiel”, “registre du commerce”, “appel d’offres”*.  
- **Arabic (Maghreb/Egypt):** try Arabic queries and Latin transliteration for names/orgs.  
- **Portuguese:** *“Diário da República”, “certidão”, “NIF/NUIT”*.  
- **Swahili:** *“tangazo”, “tenda/ zabuni”, “kampuni”*.  
- Rotate English/French/Arabic/Portuguese synonyms for the same query across Google/Bing/Yandex.

---

## 🌐 9) Domains, IPs & Tech
- Local ccTLD registries: **.za .ng .ke .gh .tz .ug .dz .ma .tn .eg .ao .mz** (WHOIS/proxy varies).  
- Certificate Transparency (crt.sh) for domain discovery; passive DNS via SecurityTrails/Censys.  
- Government subdomains often listed in Gazette PDFs—scrape for URLs.

---

## 📰 10) Media & Verification
- **Cross-verify** with at least one **independent** outlet (state vs private vs regional).  
- Use **AllAfrica** mirrors + primary newsroom sites; compare wording to avoid syndication loops.  
- **Archive early**: many outlets change URLs or purge archives.

---

## ⚠️ 11) Constraints & Pitfalls
- **Registry opacity** and paywalls; rely on **Gazettes**, court notices, and market filings.  
- **Name collision** in large populations—confirm with multiple attributes (city, employer, school).  
- **Low address standardization**; use landmarks and **what3words**/OSM landmarks.  
- **Connectivity volatility**; mirror/backup captures.

---

## 🧩 12) High-Value Pivots (Quick Wins)
- Search `site:.gov.* filetype:pdf "tender" OR "award"` for procurement.  
- Search `"RCCM" OR "RC" "N°" "{name}"` in OHADA countries for company IDs.  
- For SA: CIPC + Government Gazette + company pressroom to triangulate.  
- For KE/GH/NG: tender portals + tax lists + business registries + newsroom coverage.  
- For Maghreb: OMPIC/JORT/BO + Arabic name variant + LinkedIn role.

---

## 🗂 13) Documentation Hygiene
- Record: **canonical URL**, **archived URL(s)** (Wayback/Archive.today), **capture UTC**, **file hashes** for downloads, query strings, and language variants used.  
- Keep a table of **name spellings/transliterations** tried and results.

---

## 🛡 14) Investigator Tips
- Always run **two languages** minimum for key queries (e.g., English + French/Arabic/Portuguese).  
- Prefer **official docs** (Gazettes, registers) for anchor facts; use media/social to fill gaps.  
- Build a small **country profile** sheet (registry links, Gazettes, tender sites, languages) before deep dive.

---

### 📜 Changelog (2025-08-10)
- Consolidated pan-African sources; added procurement & Gazette pivots.  
- Expanded phone/mobile-money context and language recipes.  
- Added verification notes for syndication and archival volatility.
```
