# DARKInt (Dark Web Intelligence) Cheat Sheet
_Last verified: 2025-08-11 • Scope: lawful investigative use only. Comply with local/national law, ethics policies, and platform terms._

## 1) Purpose
DARKInt (Dark Web Intelligence) complements OSINT by gathering intelligence from the hidden, encrypted dark web — revealing illicit activities, emerging threats, and sensitive leaks inaccessible via surface web methods.

## 2) Difference Between OSINT & DARKInt
| OSINT | DARKInt |
|-------|---------|
| Public, open sources | Hidden, encrypted sources |
| Indexed by search engines | Accessible only via Tor/I2P |
| Social media, public records, news, databases | Darknet forums, markets, leaks |
| Broad investigative uses | High-risk criminal/cybersecurity investigations |

**Integration:** Combine OSINT for surface/deep data with DARKInt for hidden threat visibility.

## 3) Dark Web Basics
- **Surface Web:** Indexed, public content (Google, Bing).
- **Deep Web:** Unindexed but legitimate (databases, private networks).
- **Dark Web:** Encrypted, anonymized networks (Tor `.onion`, I2P, ZeroNet).

![Internet Iceberg](https://github.com/tabalizer/Intelligence-Collection/edit/main/DarkInt%20Cheat%20Sheet.md#:~:text=iceberg-,.,-png)

**Access Tools:**  
- Tor Browser — `.onion` sites  
- I2P — `.i2p` hidden services  
- Tails OS — live OS with Tor by default  
- Whonix — VM for Tor isolation  

## 4) Common DARKInt Use Cases
- Threat Intelligence (monitor hacker forums, malware sales)
- Fraud Prevention (track stolen cards, credentials)
- Child Protection (monitor and disrupt CSAM networks)
- Digital Identity Protection (detect exposed credentials)
- Cyber Insurance (risk profiling)
- Infrastructure Protection (energy, water, transport)
- National Security (terrorism financing, arms sales)

## 5) Techniques
1. **Data Scraping** – Crawl and extract content from darknet marketplaces/forums (use lawful tooling).
2. **Deanonymization** – Cross-reference usernames, emails, crypto wallets with OSINT data.
3. **Content & Sentiment Analysis** – Identify threat actors, emerging attacks.
4. **Cryptocurrency Tracking** – Blockchain analytics to follow illicit payments.
5. **Leak Monitoring** – Watch for breaches/exfiltrations relevant to your org/sector.

## 6) Tools & Platforms
**Access & Browsing**  
- [Tor Browser](https://www.torproject.org/) — Core access  
- [I2P](https://geti2p.net/) — Alternate darknet  
- [Tails OS](https://tails.boum.org/) — Amnesic OS  
- [Whonix](https://www.whonix.org/) — VM-based isolation

**Search & Index** *(dark web only)*  
- [Ahmia](https://ahmia.fi/)  
- [DarkSearch](https://darksearch.io/)  
- [Haystak](https://haystakvxad7wbk5.onion/) *(premium for advanced queries)*  

**Data Monitoring & Analysis**  
- [Maltego](https://www.maltego.com/) + dark web transforms  
- [SpiderFoot HX](https://www.spiderfoot.net/)  
- [Recorded Future](https://www.recordedfuture.com/) DARKInt module  
- [DarkOwl Vision](https://www.darkowl.com/)  
- [OnChain Industries](https://www.onchainindustries.com/) for blockchain tracing  
- [Have I Been Pwned](https://haveibeenpwned.com/) for breach correlation

## 7) Discovery Patterns (Dorking & Pivoting)
*(lawful, open-source indexing only — do not hack or force entry)*

### Clear Web Dorks to Find Dark Web References:
- `"onion link"` filetype:txt OR filetype:pdf  
- `"Tor mirror"` AND `site:pastebin.com`  
- `"dark web market"` OR `"hidden service"`  
- `site:github.com "onion" "marketplace"`  
- `"http://*.onion"` -site:onion.cab  

### Username & Handle Pivoting:
- Search known handles in OSINT sources to link to dark web activity.
- `"@handle" site:reddit.com`  
- `"@handle" site:twitter.com`  
- `"@handle" "bitcoin address"`

### Crypto Pivot:
- Paste BTC/ETH/XMR address into blockchain explorers (e.g., Blockchair, OXT, Etherscan) to trace transactions.

## 8) How-To Workflow
1. **Scope & Authorize** — Define targets, confirm legal/ethical clearance.
2. **Access Environment** — Use isolated VM + VPN + Tor for opsec.
3. **Seed Collection** — Gather onion links, forum names, marketplace URLs from open intel.
4. **Infiltration** — Create personas, join forums (only if lawful).
5. **Automate Monitoring** — Use scraping/indexing tools for keyword alerts.
6. **Pivot** — From content → usernames → crypto → clear web identities.
7. **Correlate with OSINT** — Validate dark web findings against open data.
8. **Document** — Timestamp, hash, screenshot, export logs for chain-of-custody.

## 9) OpSec Tips
- Never use personal accounts or devices.
- Isolate dark web activity in disposable/segregated environments.
- Avoid downloading files unless sandboxed and scanned.
- Change identities regularly to avoid doxxing by hostile actors.

## 10) Ethical & Legal Considerations
- Do not access illegal content (especially CSAM).
- Follow your jurisdiction’s cybercrime & privacy laws.
- Use only in authorized investigative contexts.
- Ensure compliance with internal policies & court evidentiary standards.

## 11) Sample Dark Web Monitoring Queries
*(via lawful indexing services like Ahmia/Haystak)*  
- `"companyname" OR "productname"`  
- `"employeeemail@company.com"`  
- `"confidential" OR "internal use only"`  
- `"database dump"`  
- `"RDP access"` + `"country"`  
- `"fullz"` + `"SSN"`

## 12) Documentation Hygiene
- Log date/time (UTC), source URL, capture method.
- Screenshot + export text data; hash files for integrity.
- Keep an audit trail for legal admissibility.
- Label sources as **verified** or **unverified**.

## 13) Quick DARKInt Tool Recipe
**Goal:** Detect stolen corporate credentials  
**Steps:**  
1. In Ahmia, search `"@company.com"`  
2. Extract onion links → access via Tor  
3. Scrape forum threads for email/password combos  
4. Verify breach source in HaveIBeenPwned  
5. Notify security team + recommend resets

## 14) Key Risks
- Malware in downloads  
- Honeypot sites run by LE or criminals  
- Misinformation planted to mislead  
- Jurisdictional violations when crossing borders digitally

## 15) Further Learning
- Europol IOCTA Reports  
- Tor Project Resources  
- OSINT & Dark Web modules in [SANS SEC497](https://www.sans.org/cyber-security-courses/practical-open-source-intelligence/)  
- [Bellingcat’s Dark Web Guide](https://www.bellingcat.com/resources/2021/05/10/a-beginners-guide-to-the-dark-web/)

### Changelog (2025-08-11)
- Added ethical usage guidelines
- Updated tools list with blockchain tracing resources
- Expanded discovery & pivoting patterns
