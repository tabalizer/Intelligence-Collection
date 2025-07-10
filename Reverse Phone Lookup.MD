# 🛡️ Reverse Phone Lookup OSINT Cheat Sheet

> **Empower your defenses. Outsmart phone fraud. Use Open-Source Intelligence (OSINT) to unmask unknown callers and block scams before they begin.**

---

## 🔍 What is Reverse Phone Lookup?

**Reverse Phone Lookup** uses a phone number to uncover details about the caller, including:
- 👤 Name  
- 🏠 Address  
- 🏢 Company or workplace  
- 🌐 Social media accounts  
- 💬 Public mentions  

Unlike Caller ID (which can be spoofed), this technique **cross-references billions of data points** for high-confidence identification.

---

## 🧰 Core Data Sources

| 🔗 Source Type         | 📌 Example Content                                      |
|------------------------|--------------------------------------------------------|
| 🏛️ Public Records      | Voter rolls, property ownership, business licenses     |
| 🗂️ Business Directories | Company staff lists, contact info                     |
| 📱 Social Media         | Public profiles, comments, shared posts               |
| 📞 Telecom Databases    | Carrier info, VOIP flags                              |
| 🚨 Scam Reports         | FTC lists, community complaints, blacklists           |

---

## ⚙️ How to Perform a Reverse Phone Lookup

### 🥇 1. **Start with Google Dorking**

Use advanced search operators to scan for the number across public platforms:

```plaintext
"123-456-7890"
"123-456-7890" site:facebook.com
"123-456-7890" filetype:pdf OR filetype:xls
"123-456-7890" -spam -scam
```

🔎 Works with: Google, DuckDuckGo, Bing, Yandex, Baidu

---

### 🛠️ 2. **Use OSINT Tools**

| 🧪 Tool                | ✅ What It Does                                   |
|------------------------|--------------------------------------------------|
| 🔎 **Truecaller**       | Global ID + spam flagging                        |
| 🧠 **OSINT Industries** | 70+ lookup modules (emails, names, socials)      |
| 🕸️ **Maltego**          | Visualizes networks, links phones to entities    |
| 🔍 **Sync.me / Whitepages / NumLookup** | Free identity checks       |
| 🧪 **BeenVerified / Intelius** | Paid deep reports (U.S. focused)         |

---

### 💬 3. **SOCMINT – Social Media Intelligence**

Check social platforms directly:

- 🔍 Facebook / LinkedIn / X (Twitter) / Instagram  
- 📲 WhatsApp / Telegram: Save contact & check profile info

```plaintext
"123-456-7890" site:linkedin.com
```

---

### 📂 4. **Cross-reference Public Records**

Search free or subscription databases:
- 🏘️ Property ownership
- 🏢 Business filings
- ⚖️ Court documents

---

## 🚩 Red Flags to Watch For

| ⚠️ Suspicious Pattern         | 📉 Implication                                  |
|------------------------------|-------------------------------------------------|
| 🔁 Burner numbers / no history | Disposable scam lines                          |
| 🎭 Caller ID mismatch         | Spoofed identity                               |
| 🌍 Foreign call origin        | Impersonation of local institutions            |
| 💬 Overuse of urgency         | Social engineering attempt                     |

---

## 👤 Who Should Use This?

### 1. **📱 Individuals**

Protect from:

#### 🧑‍⚖️ IRS / Bank Phishing Scams
> **Important:** This refers to **fraudsters impersonating** the IRS or banks—**not** legitimate government officials or financial institutions.

Scammers may:
- Claim you're under legal threat
- Demand immediate payment via crypto or gift cards
- Use spoofed caller ID to fake legitimacy

🔐 **OSINT lookup helps verify before you respond.**

#### 💻 Tech Support Scams
- "Apple", "Microsoft", or "Amazon" call claiming your device has an issue
- Ask for remote access or payments for fake services

#### 💔 Romance Scams
- Impersonate doctors, military personnel, or expats
- Build trust, then request money for emergencies

#### 🐷 Pig Butchering (Crypto Scams)
- Long-term deception blending romance and fake investments
- Scammers guide victims to fake crypto platforms, drain funds

**Tips**:
- Cross-check unknown callers before replying  
- Save flagged numbers to blocklist apps  
- Report confirmed scams to the FTC or your cybercrime unit  

---

### 2. **🏢 Businesses**

Protect against:

#### 💰 Fake Invoice Scams
- Impersonate vendors requesting urgent payments to fake accounts

#### 👨‍💼 CEO Fraud (Whaling)
- Spoofed executive numbers with urgent money transfer requests

#### 🧠 Social Engineering
- Use public info (LinkedIn, press releases) to impersonate clients or execs

**Best Practices**:
- 📵 Always verify vendor contact before processing payments  
- 🧩 Integrate phone verification in CRM workflows  
- 🔔 Trigger alerts for unknown or mismatched numbers  

---

### 3. **👮 Law Enforcement**

Support investigations by:

- 📞 Mapping phone fraud infrastructure  
- 🌐 Tracing VOIP/SIP providers and call gateways  
- 🔁 Correlating recycled numbers across scam types  
- 🧬 Visualizing fraud networks with tools like Maltego

**Use for:**
- ⚖️ Chain-of-custody for reverse lookup evidence  
- 🔗 Linking scams using shared infrastructure  
- 🕵️ Pattern analysis on scam call timing & frequency  

---

## 🧠 Advanced Techniques

| 🧩 Technique               | 🛠️ Tool or Method                        |
|----------------------------|------------------------------------------|
| 📈 **Temporal Pattern Mapping** | Time-based call clustering to spot scams |
| 🌍 **GeoINT on Call Origin**    | Lookup # country vs claimed ID          |
| 🔐 **SIM Swap Check**          | Monitor breach forums & swap indicators |
| 🧬 **Graph Network Analysis**  | Maltego, OSINT Industries Palette       |
| 🧾 **Public Breach Databases** | Check leaked databases for connections  |

---

## 🔐 Safety Tips

- ✅ Save reverse lookup results for future reference  
- 🛡️ Never engage unless you've verified the number  
- 🔁 Share confirmed scam numbers with your community  
- 🚫 Register your number with **Do Not Call lists**:
  - [FTC DNC](https://www.donotcall.gov/)
  - [Spamhaus DBL](https://www.spamhaus.org/)

---

## 📦 Resources

- 🔗 [Shadowdragon](https://www.shadowdragon.io/)
- 🔗 [Truecaller](https://www.truecaller.com/)
- 🔗 [OSINT Industries](https://www.osint.industries/)
- 🔗 [Maltego](https://www.maltego.com/)
- 🔗 [BeenVerified](https://www.beenverified.com/)
- 📘 [FTC Scam Alerts](https://www.consumer.ftc.gov/features/scam-alerts)

---

## ✅ Summary

> Reverse phone lookup is **not just a tool** — it's a **first line of defense** in the fight against phone fraud.

- 🕵️ Investigate unknown numbers  
- 🚫 Stop phishing and impersonation  
- 🧠 Protect individuals, businesses & investigators  
- 🧰 Use OSINT methods & tools proactively

---

📌 **Stay smart. Stay safe. Verify before you reply.**
