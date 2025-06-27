# 🗂️ Collection Data Categories **v.2 – FULL** 🚀  
*Practical cheat-sheet — now with added entities and attributes + NATO-aligned ratings*

---

## 🛡️ NATO Reliability & Credibility Matrix

| 🔠 | **Source Reliability** | 🔢 | **Information Credibility / Accuracy** |
|---|------------------------|---|----------------------------------------|
| **A** | Completely reliable | **1** | Confirmed by independent sources |
| **B** | Usually reliable | **2** | Probably true - logical & consistent |
| **C** | Fairly reliable | **3** | Possibly true - partially corroborated |
| **D** | Not usually reliable | **4** | Doubtful – no corroboration |
| **E** | Unreliable | **5** | Improbable – contradicted elsewhere |
| **F** | Cannot be judged | **6** | Truth cannot be judged |

*Tag every datapoint “`<Reliability><Credibility>`” (e.g. **B2**).*

---

## 🎯 Priority Flags
| Flag | Meaning | Trigger |
|------|---------|---------|
| 🔥 **HOT** | Immediate operational impact | Active threat, surveillance target |
| ⏳ **TIM** | Time-sensitive (≤ 72 h) | Perishable opportunity |
| 🧊 **COLD** | Background / strategic | No urgency |

---

## 📌 Entity Attribute Catalogue

### 1. 👤 Individuals
| **Attribute Group** | **Fields** |
|---------------------|------------|
| 🆔 **Identity** | Full Name, Aliases, Identity No./SSN, Nationality (primary/secondary), Passport No., Biometrics (DNA, fingerprints, face, iris) |
| 📍 **Address & Presence** | Residential Address, Workplace, Current Location (live), Historical Movements (GPS, travel records) |
| 🧑 **Characteristics** | Physical Description, Health Status, Behaviour traits (trust / risk), Psychological profile |
| 💼 **Professional / Personal** | Roles & Responsibilities, Employer, Daily Routine, Education, Skills, Hobbies |
| 💰 **Financial / Assets** | Bank accts, Crypto wallets, Investments, High-value items, Real estate |
| 📞 **Communications** | Phone numbers (current/historic), Email, Social media, Secure apps (Signal, Telegram, WhatsApp, Matrix) |
| 🎖 **Titles & Ranks** | Official rank, Honorifics, Community roles |
| 🔗 **Relations / Networks** | Family, Associates, Org affiliations, Event involvement, Ownership links |

---

### 2. 🏢 Organizations
| **Attribute Group** | **Fields** |
|---------------------|------------|
| 🏷 **Identity** | Legal name, Acronyms, Brands, Registration No., Logos |
| 🏗 **Ownership & Structure** | Shareholders, Parent / Subsidiaries, Org chart, Board, Key leaders |
| 📍 **Footprint** | HQ, Branches, Warehouses, Data centres, Geocoords |
| 👥 **Personnel** | Management, Employees, Contractors, Advisors |
| 💰 **Finance** | Accounts, Revenue, Funding sources, Credit rating, Sanctions status |
| 🛍 **Products / Services** | Lines of business, Trade names, NAICS / HS codes |
| 🤝 **External Links** | Partners, Suppliers, Competitors, NGOs, OCG ties |
| 🏗 **Infrastructure & Assets** | Facilities (buildings, plants), Vehicles, Machinery, IT systems |
| 🎭 **Roles & Activities** | Mandate, Campaign schedules, Key events |
| ⚖ **Legal** | Licences, Court cases, Compliance status |

---

### 3. 🏠 Properties & Sites
| **Attribute Group** | **Fields** |
|---------------------|------------|
| 📍 **Location** | Address, Geo coords, Admin area (city, district, country) |
| 👥 **Ownership** | Owner type (individual / entity), Current owner, Previous owners |
| 📝 **Property Details** | Area (m²), Zoning, Construction date, Usage (description), Property ID, Utilities |
| 🔒 **Security** | Access points, CCTV, Barriers, Alarm systems |
| ⛩ **Cover Indicators** | Front company, Dual-use, False signage |

---

### 4. 🏎️ Physical Assets
| **Attribute Group** | **Fields** |
|---------------------|------------|
| 🆔 **Identification** | Asset ID, Name, Make/Model, Serial/VIN, Category (vehicle, weapon, art) |
| 🔄 **Ownership** | Current owner, Previous owners, Lease/loan status |
| 📍 **Location** | Storage site, Transit route, Last seen (time-stamp) |
| ⚙ **Specs** | Configuration, Condition, Capability |
| 📂 **Docs** | Title, Registration, Maintenance logs |

---

### 5. 💾 Digital Assets
| **Attribute Group** | **Fields** |
|---------------------|------------|
| 🌐 **Hosting** | Domain, IP, Cloud tenant, Geo-routing |
| 🔗 **Virtual ID** | UUID, Object ID, Blockchain token |
| 🔄 **Ownership** | Admin account, Custodian, Previous holders |
| 🔐 **Access & Permissions** | Credential list, Privileged roles, MFA |
| 📝 **Metadata** | Creation date, Hash, File type, Size, Tagging, DLP marks |
| 📈 **Audit Trail** | Last login, Modification history, Exfil events |

---

### 6. 💬 Communications
- **Voice:** CDRs, IMSI/IMEI, Push-to-talk IDs  
- **Messaging:** App ID, Handle, Group membership, Key-exchange logs  
- **Email:** Header paths, PGP fingerprints, MX records  
- **RF/SAT:** Frequency, Modulation, Burst timings, TDoA fixes  

---

### 7. 🛰️ Geospatial & Movement
- **Imagery:** Sensor type, Pass-time, Resolution, Target bounding-box  
- **Mobility:** Cell-tower pings, ADS-B, AIS, ALPR hits, Toll-road data  
- **Routes & Patterns:** Waypoints, Duration, Anomalies, Choke-points  

---

### 8. 💳 Financial & Economic
- **Accounts:** IBAN, Bank, Balance snapshots, Beneficial owner  
- **Transactions:** Date, Amount, Counterparty, Channel, Typology  
- **Crypto:** Address, Tx hash, Mixer use, NFT holdings  
- **Trade:** Invoices, Bills of lading, Customs declarations  

---

### 9. 📅 Events & Incidents
| Field | Examples |
|-------|----------|
| 🕒 **Time** | Start, End, Duration, Time-zone |
| 🌍 **Location** | Geo-point, Venue, Digital domain |
| ❓ **Motivation** | Ideology, Profit, Retaliation |
| ⚙ **Method** | TTPs, Weapon system, Malware family |
| 👥 **Actors** | Individuals, Orgs, Assets involved |
| 📊 **Impact** | Casualties, Cost, Service disruption |
| 📂 **Classification** | Security incident, Safety breach, Notable occurrence |

---

### 10. 📢 Influence & Media
- **Media coverage:** Outlet, Headline, Tone/Sentiment  
- **Social engagement:** Bots, Amplification rate, Hashtags  
- **Narratives:** Key talking-points, Target audience, Language  

---

## 🧩 Cross-Cutting Metadata
- **🗂 Case/Op ID** • **🔐 Classification & Caveats** • **🔄 Chain of custody (hash, collector, timestamp)** • **✍️ Analyst notes / Gaps**

---

## ⚠️ Pitfalls & Counter-Measures
- **Over-collection** → use priority flags  
- **Circular reporting** → tag sources uniquely  
- **Metadata leaks** → strip EXIF / secure share-links  
- **Legal overstep** → validate against privacy & SIGINT law  

---

## 📖 ReadMe
| | |
|---|---|
| **Author** | [@tabalizer]([https://twitter.com/tabalizer](https://github.com/tabalizer) |
| **Version** | **v.2** (24 Apr 2025) |
| **Change-log** | Major update
| **License** | Creative Commons BY 4.0 |

---
