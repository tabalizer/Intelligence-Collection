# 📖 Epic Google Dork Cheat Sheet for Advanced OSINT 🔍

Google dorks use advanced search operators to uncover hidden information. Below is a comprehensive cheat sheet organized by category, with one-liner dorks and explanations. Copy, paste, and tweak these for your investigation needs. *(Pro tip: Use quotes `"` for exact phrases and `OR`/`-` to refine searches.)*

## 📄 File Type Discovery  
Find specific file types (PDFs, docs, etc.) that might contain valuable info. Use `filetype:` (or `ext:`) to restrict by extension. Great for locating reports, resumes, or data dumps.  

- 📄 **Sensitive Docs:** `filetype:pdf "confidential"` – Finds PDF documents labeled *“confidential”*, often internal reports or l191】.  
- 📄 **Multi-Format Search:** `"John J. Doe" (filetype:pdf OR filetype:docx OR filetype:xlsx)` – Searches for an exact name across PDF, Word, or Excel files (useful for finding resumes, contracts,L812】).  

## 📂 Directory Listings  
Discover open directory indexes on web servers. These pages (often titled “Index of”) list files on a server when directory listing is enabled – a goldmine for finding unprotected files and folders.  

- 📂 **Open Indexes:** `intitle:"index of /" "Parent Directory"` – Finds publicly accessible *directory index* pages (look for “Index of /” and “Parent Directory” in results). Often indicates a browsable file repository.  
- 📂 **Backup Folders:** `intitle:"index of" backup` – Reveals open directories named “backup” that might contain old databases, configs, or ZIP 01-L107】. These often hold sensitive data from previous versions.  

## 🎯 Site-Specific Search  
Focus your OSINT on a particular site or domain. The `site:` operator restricts results to a given website or TLD. Great for searching a target organization’s domain or finding content in a specific sector (.edu, .gov, etc.).  

- 🎯 **Internal Site Search:** `site:example.com "internal memo"` – Searches *only* on **example.com** for pages containing “internal memo”. Use this to find company-specific info (e.g. policies, staff pages) on a t ([What are Google dorks? Google dorks cheat sheet and guide | NordVPN](https://nordvpn.com/blog/google-hacks/#:~:text=Another%20Google%20dork%20example%20is,Fi)).  
- 🎯 **Sector Search:** `site:.edu filetype:pdf "resume"` – Finds PDF files containing “resume” on **.edu** domains. 🎓 Use this to collect CVs or personal info from university websites (names, emails, etc., in student or faculty resumes).  

## 🕵️ Index of Sensitive Data  
Dig up exposed sensitive data by targeting known filenames or keywords in open indexes. Combines the directory listing approach with specific terms for juicy info. Perfect for finding leaked credentials, database dumps, or keys.  

- 🕵️ **Password Repositories:** `intitle:"index of" "passwords.txt"` – Locates open directories holding files like *passwords.txt*, which often contain lists ls. (Remove quotes or use wildcards to catch variations like `passwords.csv` or `.bak` files.)  
- 🕵️ **Database Dumps:** `intitle:"index of" "backup.sql"` – Finds SQL database backups exposeds. These may contain schemas or even data dumps. Also try variations like `.sql.zip` or keywords like “dump” to catch compressed backups.  
- 🕵️ **SSH Keys:** `intitle:"index of" "id_rsa.pub"` – Searches for public SSH key es. Public keys alone aren’t secrets, but finding them on an open server might indicate a misconfigured `.ssh/` directory (and the private key could be nearby!).  

## 🔐 Login Portals  
Identify pages that look like login forms or portals. Useful for mapping an organization’s login interfaces (webmail, VPN, admin logins) during recon. Common indicators are “login” in the URL or title and fields like username/password on the page.  

- 🔐 **Generic Login Pages:** `intitle:"Login" "Username" "Password"` – Finds pages with “Login” in the title and the words “Username” and “Password” in the text. These are likely login pages with input fields for credentials.  
- 🔐 **Specific Login URL:** `inurl:login intext:"password"` – Targets pages with “login” in the URL that also mentionin text. This can reveal login endpoints (e.g. `login.php`, `login.aspx`) including those that might not be obvious via the website’s navigation.  

## ⚠️ Error Messages  
Hunt for sites leaking error logs or debug messages. Developers sometimes leave verbose errors that reveal server paths, SQL queries, or stack traces. Dorks targeting these messages can uncover software versions or vulnerabilities.  

- ⚠️ **SQL Errors:** `intext:"You have an error in your SQL syntax"` – Finds pages showing MySQL error 1064 messages. These occur when a query fails, possibly hinting at SQL injection points or poorly sanitized inputs (the error often includes the faulty SQL snippet and server version).  
- ⚠️ **Server Stack Traces:** `intext:"Fatal error" "on line" "Warning:"` – Searches for PHP runtime errors that include *“Fatal error”* or *“Warning”* and a line number. Such results can expose file paths on the server (e.g., `/var/www/...`) or code specifics, useful for identifying tech stack and misconfigurations.  
- ⚠️ **Log Files:** `filetype:log "Exception"` – Looks for log files (`*.log`) containing the term “Exception”. This can surface Java, .NET, or application logs that were accidentally left accessible, potentially revealing debug info, API keys, or user data.  

## 📷 Insecure Devices (Webcams & Printers)  
Uncover live feeds from unsecured webcams and status pages for network printers or IoT devices. Many are indexed by Google due to default pages or unprotected interfaces. These dorks target known titles/URLs used by such devices. *(Remember: just because you **can** view it doesn’t mean you **should** – **no snooping** beyond your legal authority!)*

- 📷 **Public Webcams:** `intitle:"webcamXP 5"` – Finds pages with “WebcamXP 5” in the title (a pop ([How to Use Google Dorks to Access Online Cameras | by Meerabell | OSINT Team](https://osintteam.blog/how-to-use-google-dorks-to-access-online-cameras-251e83106f6b#:~:text=intitle%3A%E2%80%9CwebcamXP))ftware). Users often forget to password-protect these, resulting in live camera feeds accessible to anyone (🎥 think parking lots, lobbies, etc.).  
- 🖨️ **Open Printers:** `intitle:"Printer Status" inurl:"PrinterStatus.html"` – Exposes netwoatus pages. Many office printers have a web interface; this dork finds ones where the status page is publicly reachable (showing printer model, status, possibly company info).  
- 📷 **IP Camera Feeds:** `inurl:"/view/view.shtml"` – Searches for URLs containing the common camera feed pa ([How to Use Google Dorks to Access Online Cameras | by Meerabell | OSINT Team](https://osintteam.blog/how-to-use-google-dorks-to-access-online-cameras-251e83106f6b#:~:text=inurl%3Aview%2Fview))iew.shtml`**. This often leads to live streams from IP cameras (Axis, Panasonic, etc.) that use a generic web interface.  

## 🔧 Configuration Files  
Locate configuration files or backup configs that have been indexed. These often contain credentials, API keys, or other secrets. Look for specific file extensions and keywords that denote config data. Combining `filetype:` with sensitive terms can yield gold.  

- 🔧 **Env Files with Secrets:** `filetype:env "DB_PASSWORD"` – Searches for **environment config** files (often named `.env`) that se passwords. This dork can reveal DB connection details, API keys, or other app secrets if the .env file was accidentally left in the webroot.  
- 🔧 **Exposed Backups:** `ext:bak "wp-config.php"` – Looks for backup copie config files. For example, a developer might save `wp-config.php.bak` which, if accessible, will display the database name, user, and password in plain text. (Try other extensions like `.old`, `.orig` or common names like *config.php.save*).  
- 🔧 **API Keys in Code:** `site:github.com "SECRET_KEY"` – Dork through public GitHub repositories forf “SECRET_KEY”. Often finds API keys, tokens, or credentials hard-coded in public code. You can swap in other terms like **"API_KEY"**, **"AWS_SECRET"**, or **"password"** and target other code hosting domains if needed.  

## 🛡️ Admin Panels  
Find administrative interfaces and control panels that might be exposed. These could be login pages for site admins, database control panels, or IoT device dashboards. Identifying them is useful for understanding an organization’s attack surface (or for testing your own).  

- 🛡️ **Admin Login Pages:** `inurl:admin intitle:"Login"` – Identifies admin login portals by looking for “admin” in the URLin the page title. Common results include URLs like ***/admin/login***, ***/admin.php***, or CMS backends.  
- 🛡️ **Admin Dashboard Access:** `intitle:"Admin Panel" "Dashboard"` – Searches for pages with titles indicating an admin panel or dashboard. For example, many admin interfaces have a title like “Admin Panel”, “Admin Dashboard”, or include the word “Administrator”. This dork can reveal pages that might not be obviously named “admin”. (E.g. an Elasticsearch or Kibana console might show “Dashboard”).  

----

**🔚 Note:** Google dorking is a powerful OSINT technique to find information that’s not immediately visible. Use these queries to augment your investigations, but **with great power comes great responsibility**. Always ensure you have permission to access any discovered system or data, and keep your searches ethical. Happy dorking! 🕵️🔎

