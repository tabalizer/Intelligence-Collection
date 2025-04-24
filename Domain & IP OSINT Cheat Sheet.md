# 🧠 Domain & IP OSINT Cheat Sheet (Advanced) 🌐

**Objective:** Conduct deep reconnaissance on domains and IPs with an intelligence-focused approach — mapping infrastructure, attribution, and activity over time.

---

## 🛠️ Core Recon Tools

| Tool             | Functionality                                          | URL                               |
|------------------|--------------------------------------------------------|-----------------------------------|
| **SecurityTrails**  | WHOIS, subdomains, historical DNS, passive DNS      | https://securitytrails.com        |
| **Shodan**          | Port scanning, banner grabbing, device fingerprint  | https://shodan.io                 |
| **Censys**          | TLS certs, services over time, host search          | https://censys.io                 |
| **LeakIX**          | Exposed services, leaked files, dev portals         | https://leakix.net                |
| **GreyNoise**       | IP behavior classification (benign/malicious)       | https://viz.greynoise.io          |
| **VirusTotal**      | IP/domain malware reports, graph relationships      | https://www.virustotal.com        |
| **FOFA**            | Chinese Shodan alternative, powerful for Asia infra | https://fofa.info                 |

---

## 🧭 Tactical Techniques & Workflows

### 🔍 1. **Domain Attribution via WHOIS**
- Use historical WHOIS to uncover:
  - Owner patterns (reuse of email, phone)
  - Company registration, address reuse
  - Change of ownership timelines
- Tools: SecurityTrails, DomainTools (paid), ViewDNS WHOIS History

---

### 🧬 2. **Subdomain Mapping (Infrastructure Discovery)**
- Combine:
  - `Amass`, `Subfinder`, `crt.sh`, `dnsx`
  - Zone transfer attempts (`dig axfr`)
- Cross-reference discovered subdomains in:
  - Shodan (open ports), VirusTotal (malicious activity), LeakIX (leaked panels)

---

### 🧪 3. **IP Analysis & Pivoting**
- Use `Censys` or `Shodan` to:
  - Discover what else is hosted on same /24
  - Identify devices running on same ASN
- Use `SecurityTrails` for reverse IP — other domains hosted on that IP

---

### 🌍 4. **Geolocation & Hosting Insight**
- Combine:
  - IPinfo.io + MaxMind → Get ASN, ISP, geo
  - ARIN/RIPE WHOIS for BGP data
  - Greynoise → Determine if IP is scanning the web or linked to malware campaigns

---

### 🕵️ 5. **Passive DNS & Historic DNS Tracking**
- Identify:
  - Domain resolution history
  - Infrastructure changes (e.g., moved from OVH to Cloudflare)
- Tools: RiskIQ (Community), DNSDB (Farsight, paid), SecurityTrails

---

### 🧠 6. **Correlation & Timeline Building**
- Use VirusTotal Graph or Maltego:
  - Map domains ↔ IPs ↔ certificates ↔ WHOIS email addresses
  - Timeline server behavior (e.g., open RDP > then blocked > then malware)

---

## 🔐 Certificate-Based Discovery (TLS Pivots)
- Search `Censys` or `crt.sh`:
  - Common Name (CN) or SAN reuse across domains
  - Self-signed certs that indicate dev/test environments
  - Cert hash reuse = same server across IPs

---

## ⚙️ Bonus Tools & Scripts
- `ASNmap`: Map out IP space of an entire ASN
- `tlsx`: TLS scanner to identify endpoints, grab certs fast
- `massdns`: High-performance DNS resolver for subdomain bruteforce
- `dnstwist`: Find typo-squatting or phishing variants

---

## ⚠️ Ethics & Legal Compliance

- ✅ Stick to publicly available information
- ❌ Don’t scan systems without authorization
- ⚠️ Watch data residency and GDPR-sensitive queries

---

## 🧩 Suggested Workflow

1. **Initial Domain** ➝ WHOIS & Certs ➝ Discover Subdomains
2. **Subdomains** ➝ Resolve IPs ➝ Shodan/Censys Scan
3. **IP Blocks** ➝ ASN Mapping ➝ Related Infra Discovery
4. **Timeline** ➝ Historical DNS + Certs + VT Graph
5. **Attribution** ➝ WHOIS Email ➝ Other Domains

---

🚀 *Use the internet against itself. Map, track, attribute — legally and intelligently.*
