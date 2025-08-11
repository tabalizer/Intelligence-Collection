# OSINT in India – Field Cheat Sheet
_Last verified: 2025-08-11 • Scope: India-focused open-source collection only. Use ethically and comply with local law & platform ToS._

## 1) Purpose
A practical, platform-agnostic reference to collect, verify, and document India-specific OSINT/SOCMINT signals fast—across languages, scripts, and high-velocity social ecosystems, with direct access to public data assets.

## 2) Core Workflow (FIND-IN)
1) **Frame** → entities, place, time, and language(s)/script(s).  
2) **Intent** → people, orgs, media, events, commerce, legal, or geospatial.  
3) **Narrow** → platform, region/language, legal source, and time window.  
4) **Double-check** → cross-platform + cross-language + archive immediately.

## 3) High-signal sources (national)
- **Government & Regulatory**
  - [MCA Company Master Data](https://www.mca.gov.in/mcafoportal/viewCompanyMasterData.do) – corporate registration, directors, CIN/DIN lookups.  
  - [IPIndia](https://ipindiaonline.gov.in/) – patents, designs, trademarks.  
  - [eCourts](https://services.ecourts.gov.in/) – case status, party name search.  
  - [eProcure/CPPP](https://eprocure.gov.in/cppp/) – central tenders & contracts.  
  - [GeM – Government eMarketplace](https://gem.gov.in/) – public procurement database.  
  - [DGFT](https://www.dgft.gov.in/) – trade & export-import records.  
  - [GSTIN Search](https://services.gst.gov.in/services/searchtp) – GST registration verification.  
  - [NGO-Darpan](https://ngodarpan.gov.in/) – registered NGOs, FCRA status.

- **Elections**
  - [Election Commission of India](https://eci.gov.in/) – results, political party info.  
  - [NVSP](https://www.nvsp.in/) – voter services (note: PII risk—query ethically).  

- **Finance/Markets**
  - [SEBI](https://www.sebi.gov.in/) – regulatory filings, enforcement actions.  
  - [BSE](https://www.bseindia.com/) & [NSE](https://www.nseindia.com/) – listed company disclosures.

## 4) Language & script tactics
- 22 official languages; 10+ scripts (e.g., Devanagari, Bengali, Gurmukhi, Tamil).  
- **Transliteration:** search native + Latin script variants (“Hinglish”).  
- **Name variants:** Mumbai/Bombay/मुंबई.  
- **Hashtags/keywords:** add local language tags per region.  
- **Validation:** machine translation misses nuance—validate via native speakers.

## 5) Phone & email patterns (India)
- **Phones:** `+91` + 10 digits. Burners common (prepaid SIMs).  
  - Reverse search via [Truecaller](https://www.truecaller.com/), [Eyecon](https://eyecon.app/), [Sync.me](https://sync.me/).  
- **Emails/domains:**  
  - `.in` (general), `.gov.in` (government), `.nic.in` (IT/gov infra), `.ac.in` (academic).  
  - Pivot using [Hunter.io](https://hunter.io/) or [EmailRep](https://emailrep.io/).

## 6) Platform specifics (SOCMINT-heavy)
- **WhatsApp** – search leaked group links via [Telegram Search](https://t.me/s/) and [Public Group Index](https://whatsgrouplink.com/) (use caution).  
- **YouTube** – reverse search with [AmperVid](https://ampervid.com/) or [InVID](https://www.invid-project.eu/tools-and-services/invid-verification-plugin/).  
- **X (Twitter)** – track hashtags (#FarmersProtest, #CAAProtests) using [TweetDeck](https://tweetdeck.twitter.com/) or [Hoaxy](https://hoaxy.osome.iu.edu/).  
- **Instagram/Facebook** – scrape public profiles with [Sowdust IG Tools](https://github.com/sowdust/instagram-tools) (check ToS).  
- **Telegram** – search channels with [TGStat](https://tgstat.com/) or [Telegago](https://cse.google.com/cse?cx=006368593537057042503:efxu7xprihg).  
- **Regional apps** – [ShareChat](https://sharechat.com/), [Moj](https://mojapp.in/), [Josh](https://josh.onelink.me/), often only accessible via app.

## 7) Geospatial & local media
- **Local news** – e.g., [The Hindu](https://www.thehindu.com/), [Dainik Bhaskar](https://www.bhaskar.com/), [Eenadu](https://www.eenadu.net/) (regional).  
- **Maps/POI** – [OpenStreetMap](https://www.openstreetmap.org/), [Google Maps](https://maps.google.com/) (check user-uploaded media).  
- **Crowdsourced traffic & events** – [Mapillary](https://www.mapillary.com/), [Flickr](https://www.flickr.com/).

## 8) Disinformation monitoring
- Image/video hashing – [PhotoDNA](https://www.microsoft.com/en-us/photodna), [HashLookup](https://hashlookup.circl.lu/).  
- Multi-engine reverse search – [Yandex Images](https://yandex.com/images/), [TinEye](https://tineye.com/).  
- Archive volatile content – [archive.ph](https://archive.ph/), [Hunchly](https://www.hunch.ly/), [Wayback Machine](https://web.archive.org/).

## 9) Legal & policy landscape
- **IT Act (2000)** & **Section 69A** – content blocking & surveillance powers.  
- **DPDP Act 2023** – personal data protection; restricts processing without consent.  
- Stay updated via [PRS Legislative Research](https://prsindia.org/).  
> Always collect within legal boundaries; never access non-public systems.

## 10) OpSec in India
- Separate personas & clean browsers (e.g., [LibreWolf](https://librewolf.net/), [Brave](https://brave.com/)).  
- VPN – [Mullvad](https://mullvad.net/), [ProtonVPN](https://protonvpn.com/).  
- Secure comms – [Signal](https://signal.org/), [Wire](https://wire.com/).  
- Metadata scrubbing – [MAT2](https://0xacab.org/jvoisin/mat2).

## 11) Date & freshness tactics
- Re-run searches in English + local scripts.  
- Use [Google Custom Date Range](https://www.google.com/) and [Bing after:/before:] syntax.  
- Set up keyword alerts via [Talkwalker Alerts](https://www.talkwalker.com/alerts) or [Visualping](https://visualping.io/).

## 12) Noise control
- Exclude entertainment spam: `-song -movie -meme`.  
- Filter by site/language; avoid holiday/festival overload.  
- Suppress job ads: `-job -hiring -vacancy`.

## 13) Documentation hygiene
- Log query, language/script, time, filters, persona.  
- Persist URLs + screenshots + hashes.  
- Store video with subs + metadata.

## 14) Verification & correlation
- Cross-check claims across text/image/video in multiple languages.  
- Geoverify with signage, vehicles, weather data.  
- Match SOCMINT signals with registry/gov records.

## 15) Quick recipes
- **Company due diligence** → MCA → Directors/DIN → eCourts → IPIndia → eProcure → BSE/NSE filings.  
- **Protest mapping** → hashtags on X + local news + Telegram mirrors → archive.  
- **WhatsApp group discovery** → search leaked links → pivot to admins on IG/FB.  
- **Disinfo trace** → seed media → reverse search → ShareChat/Moj variants → timeline diff.

### Changelog (2025-08-11)
- Added verified links to Indian government & platform data sources.  
- Integrated India-specific SOCMINT tools and archive methods.  
- Added OpSec & legal reference resources.

> Notes: This cheat sheet uses public, lawful sources. Always validate legal and platform ToS constraints before collection.
