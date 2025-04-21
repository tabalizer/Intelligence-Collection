# 🗺️ Geolocation Techniques for OSINT

Geolocation in OSINT involves identifying physical locations of people, objects, or events by analyzing open data sources. It's essential in verification, intelligence, investigations, and situational awareness.

---

## 📍 Geotagging Information

**🎯 Purpose:** Extract embedded location data from digital files.

🔧 Techniques:
- EXIF data extraction from images  
- Analyzing geotagged social posts  
- Reverse image search with location filters  
- Photo cluster mapping (e.g., Flickr Maps)

🛠️ Tools: ExifTool, Google Images, Yandex, Flickr Maps

---

## 🛰️ Usage of Satellite Imagery

**🎯 Purpose:** Match imagery content to physical terrain.

🔧 Techniques:
- Visual terrain & structure comparison  
- Using various map services (Google, Bing, HERE)  
- Street View and crowd-sourced street imagery  
- Overhead satellite views for verification

🛠️ Tools: Google Earth, Sentinel Hub, Mapillary, Yandex Maps

---

## 📱 Location-Based Services

**🎯 Purpose:** Leverage GPS, Wi-Fi, or cellular data via user activity.

🔧 Techniques:
- Mobile app data leakage  
- Analyzing check-in or visit history  
- Bluetooth and proximity data  
- Geolocation API usage (e.g., cell tower triangulation)

🛠️ Tools: OpenCelliD, Google Maps Timeline, API sniffers, app telemetry tools

---

## 📡 Sensor & Network-Based Clues

**🎯 Purpose:** Analyze device signal interactions.

🔧 Techniques:
- Wi-Fi and Bluetooth signal mapping  
- Cellular network triangulation  
- Matching SSID/BSSID via open databases

🛠️ Tools: WiGLE.net, Kismet, Airodump-ng

---

## 🖼️ Image & Video Analysis

**🎯 Purpose:** Use visual elements to determine physical location.

🔧 Techniques:
- Landmark and terrain matching  
- Language/signage interpretation  
- Sun/shadow-based orientation  
- Weather condition correlation  
- EXIF metadata when available

🛠️ Tools: Google Street View, SunCalc, Forensically, InVID

---

## 🌐 IP Geolocation

**🎯 Purpose:** Approximate physical location via IP addresses.

🔧 Techniques:
- Public IP lookups  
- Cross-referencing time zones and post times  
- Historical IP resolution  
- VPN/Tor detection

🛠️ Tools: IPinfo.io, MaxMind, ViewDNS, SecurityTrails

---

## 🧲 Geofencing

**🎯 Purpose:** Detect entry/exit from defined virtual zones.

🔧 Techniques:
- Monitoring geofenced content/posts  
- SDK/ad behavior leakage  
- Social media filters by location  
- App event-based triggers

🛠️ Tools: App telemetry analysis, social media search tools, reverse engineering frameworks

---

## 🗺️ Historical Map Overlays

**🎯 Purpose:** Compare past and present terrain.

🔧 Techniques:
- Georeferencing vintage maps  
- Using historical satellite/time-lapse tools  
- Archival map overlays

🛠️ Tools: Map Warper, QGIS, Google Earth Pro, David Rumsey Map Collection

---

## 📄 Document & Source Cross-Referencing

**🎯 Purpose:** Validate location via open-source content correlation.

🔧 Techniques:
- Verifying claims via news/event reports  
- Matching visuals to reported incidents  
- Community-sourced location identification  
- Multisource triangulation

🛠️ Tools: Google Search, Local media, Reddit/OSINT subforums, news APIs

---

## 🧰 Stack Summary

| Category                     | Tools                                                             |
|------------------------------|-------------------------------------------------------------------|
| Metadata & EXIF              | ExifTool, Forensically, InVID                                     |
| Satellite & Map Imagery      | Google Earth, Sentinel Hub, Mapillary, Yandex                     |
| Signal/SSID Mapping          | WiGLE.net, Kismet, OpenCelliD                                     |
| App & LBS Data               | n8n + API sniffers, App telemetry platforms, SDK trackers         |
| IP Geolocation               | IPinfo.io, MaxMind, ViewDNS, SecurityTrails                       |
| Historical Overlays          | QGIS, Google Earth Pro, Map Warper, David Rumsey Map Collection   |
| Crowdsource & Validation     | Reddit, Twitter, Local forums, News APIs                          |

---

> 🧠 Combine visual forensics, metadata extraction, map overlays, and open-source triangulation for reliable location verification.
```

---
