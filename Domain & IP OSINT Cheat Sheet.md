# Domain & IP OSINT Cheat Sheet
_Last verified: 2025-08-10 • Scope: open-source collection only (no credentialed access). All methods must comply with local law and data privacy regulations._

---

## 🎯 1) Purpose
To investigate domain names, IP addresses, and related infrastructure using open-source intelligence — uncovering ownership, hosting, history, and technical relationships.

---

## 🛠 2) Core Tool Arsenal

### WHOIS & Registration Data
- **Whois.domaintools.com** — Domain WHOIS, history (paid for advanced features).  
- **Whoisxmlapi.com** — API and web WHOIS lookups.  
- **ViewDNS.info** — Multi-tool including WHOIS, reverse WHOIS, and DNS history.  
- **ICANN WHOIS Lookup** — Official WHOIS registry query.

### DNS & Infrastructure
- **DNSDumpster.com** — DNS record enumeration, subdomain mapping.  
- **SecurityTrails.com** — DNS history, IP blocks, associated domains.  
- **Spyse.com** — Infrastructure and SSL certificate intelligence.  
- **crt.sh** — Certificate Transparency logs for domains/subdomains.  
- **Shodan.io** — Search engine for internet-connected devices by IP/domain.  
- **Censys.io** — SSL/TLS and host scan data.

### IP Address Intelligence
- **ipinfo.io** — IP geolocation, ASN, hosting provider.  
- **MaxMind GeoLite2** — Free geolocation database.  
- **AbuseIPDB.com** — IP abuse reports and history.  
- **BGPlay / RIPEstat** — BGP routing and ASN data.

### Historical & Archival
- **Wayback Machine** — Archived versions of websites.  
- **ViewDNS Reverse IP Lookup** — Domains hosted on the same IP.  
- **SecurityTrails Historical DNS** — Past DNS and hosting changes.

---

## 🔍 3) Investigation Workflow
1. **Identify**  
   - Start with domain or IP from a known source.  
2. **Resolve**  
   - Use DNS lookups to find associated IP(s), MX records, TXT/SPF/DKIM records.  
3. **Correlate**  
   - Map hosting provider, ASN, and co-hosted domains.  
4. **Corroborate**  
   - Cross-check WHOIS, certificate logs, and passive DNS records.  
5. **Capture**  
   - Archive findings with timestamps, screenshots, and exportable data.

---

## 🧩 4) Pivoting Opportunities
- Reverse WHOIS: find all domains registered with same email/organization.  
- Reverse IP: discover all domains sharing the same IP address.  
- SSL/TLS certificate search: find other domains using same certificate.  
- Subdomain discovery: identify development, staging, or hidden endpoints.

---

## 📌 5) Key Clues in Domain & IP Data
- Registrant name, email, organization.  
- Creation and expiry dates (can suggest longevity or throwaway nature).  
- Name server provider (can reveal registrar or hosting habits).  
- ASN and hosting provider patterns.  
- Co-located services (mail servers, FTP hosts, VPN gateways).

---

## 🌐 6) Cross-Platform Verification
- Search registrant email across breach databases (e.g., HaveIBeenPwned).  
- Check IP in OSINT tools like Shodan and Censys for exposed services.  
- Look up associated domains in search engines for linked activity.

---

## ⚠️ 7) 2025 Environment & Cautions
- GDPR and privacy proxy services hide most WHOIS details — use historical data for older records.  
- Cloud hosting (AWS, Azure, GCP) often obfuscates physical hosting clues — focus on service metadata.  
- Some services block repeated lookups — rotate queries.

---

## 🛡 8) Investigator Tips
- Always cross-check domain/IP findings against at least two independent sources.  
- When possible, enrich with certificate transparency and passive DNS to spot hidden links.  
- Maintain a visual map of infrastructure for complex investigations.

---

## 🗂 9) Documentation Hygiene
- Record: domain/IP, query date (UTC), sources used, findings, and confidence rating.  
- Archive raw WHOIS/DNS outputs alongside your analysis.

---

### 📜 Changelog (2025-08-10)
- Expanded DNS tool list with historical and passive DNS options.  
- Added ASN/BGP investigation resources.  
- Updated privacy & GDPR considerations for WHOIS in 2025.
