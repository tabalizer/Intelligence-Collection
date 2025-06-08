# 🕵️‍♂️ OSINT Cheat Sheet: Wayback Machine & Internet Archive

---

## 🌐 Overview
- 🗂️ **What?** A free digital archive for websites, books, media, and more  
- 📅 **Founded:** 1996  
- 📈 **Coverage:** Over 800 billion webpages archived  

---

## 🎯 OSINT Use Cases
- 🔄 **Recover deleted content** (pages, social posts, files)  
- 🧠 **Track content changes** (policy updates, edits, removals)  
- 🔍 **Investigate infrastructure** (old portals, subdomains, endpoints)  
- 📑 **Audit corporate history** (claims, PR, sustainability, product timelines)  
- 🔐 **Preserve digital evidence** (legal, journalistic, intelligence purposes)  

---

## 🚀 Archive Query Formats
```text
# Full archive history
https://web.archive.org/web/*/example.com

# Specific date snapshots (Jan 1, 2022)
https://web.archive.org/web/20220101*/example.com

# All subdomains
https://web.archive.org/web/*/sub.example.com/*

# Specific page path
https://web.archive.org/web/*/example.com/login
```

---

## 🛠️ Tools & Tactics
- 🧩 **Compare Snapshots**  
  Use Wayback UI “Compare” to highlight differences between two dates.

- 📂 **Download Archived Files**  
  Right-click → Save As on snapshots to preserve HTML, PDFs, images.

- 🕵️ **Extract Metadata**  
  Use `exiftool` or `strings` on archived files to pull embedded timestamps and authorship.

- 🔎 **Google Cache Backup**  
  Search: `cache:example.com` in Google to cross-reference with live/archived version.

- 📜 **List Archive Captures (Wayback CDX API)**  
  Example:  
  `http://web.archive.org/cdx/search/cdx?url=example.com&output=json&fl=timestamp,original`

---

## ⚠️ Known Limitations
| Limitation                | Description                                          |
|---------------------------|------------------------------------------------------|
| 🔍 Partial snapshots       | JavaScript-heavy or robots.txt-blocked sites may be missing |
| ⏱️ Time delay              | Some captures are delayed weeks or months            |
| 🌍 Regional restrictions   | Some content may be geo-blocked or legally removed   |

---

## ✅ Best Practices
- Always verify snapshot **timestamp** in the top banner  
- Use multiple snapshot **dates** to confirm changes  
- Archive content **yourself** at [archive.org/save](https://archive.org/save) to preserve evidence  
- Document **URL, access time, and snapshot URL** in notes or reports  
- Cross-reference with **Google Cache**, **DNS records**, and **WHOIS history**

---

## 💡 Snapshot Preservation Workflow
1. Search the URL using wildcard format  
2. Select and open relevant snapshot  
3. Use “View Source” or download files  
4. Run tools like `exiftool`, `strings`, or `hashdeep`  
5. Save snapshot URL and archive a local copy  
