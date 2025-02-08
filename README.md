Penetration Testing and Web Security Research
This repository contains penetration testing research and security assessments, focusing on HTTP request smuggling, subdomain enumeration, and vulnerability testing. The research primarily targets Wells Fargo's web infrastructure for educational and responsible disclosure purposes.

Contents
1. HTTP Request Smuggling
File: httpsmuggling112224.docx
Tool Used: smuggler.py
Target: www.wellsfargo.com
Summary:
The testing involved various prefix manipulations (e.g., nameprefix1, tabprefix1, space1, midspace-01, postspace-01, etc.).
Results indicate possible request smuggling vulnerabilities via TECL (Transfer-Encoding Chunked-Length) and CLTE (Content-Length Transfer-Encoding) techniques.
2. Subdomain and Directory Enumeration
File: Hakrawler pull with all sub domains and sub directories.docx
Tool Used: Hakrawler
Summary:
Extracted numerous subdomains and directories related to Wells Fargo.
Identified several potentially sensitive endpoints, such as:
Login portals (connect.secure.wellsfargo.com)
Fraud report pages (/privacy-security/fraud/report)
Internal resources (/auth/login/static/js/general_alt.js?single)
This data could assist in further reconnaissance and security analysis.
3. Web Application Testing
Screenshots (png files) show:
Burp Suite Intruder attack setup.
Payloads used for URL redirection testing.
Potential open redirect vulnerabilities in the Wells Fargo web infrastructure.
Tools & Methodology
Burp Suite – Used for intercepting and testing HTTP request manipulations.
Smuggler.py – Conducted HTTP request smuggling tests.
Hakrawler – Automated subdomain and directory discovery.
