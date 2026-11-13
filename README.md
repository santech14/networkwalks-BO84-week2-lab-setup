WEEK 2 – PROJECT MODULE 1
FOOTPRINTING & RECONNAISSANCE ATTACKS WITH MULTIPLE KALI TOOLS

Student Name: [Your Name]
Course: Cybersecurity / Ethical Hacking
Week: 2
Project: Module 1 – Footprinting & Reconnaissance
Target Domain: networkwalks.com
Operating System: Kali Linux
Date: [Submission Date]

1. INTRODUCTION

Footprinting and reconnaissance are the initial stages of cybersecurity testing and ethical hacking. The purpose is to collect publicly available information about a target domain and understand its internet-facing infrastructure.

In this project, I used six Kali Linux tools to investigate the publicly available information associated with networkwalks.com.

The tools used were:

WHOIS
WhatWeb
NSLookup
cURL
WAFW00F
DNSRecon

The information collected helps identify domain registration details, website technologies, IP addresses, HTTP headers, Web Application Firewall (WAF) information, and DNS records.

Objective: To understand how reconnaissance tools work and how they help cybersecurity professionals identify publicly exposed information.

2. TASK 1 – WHOIS DOMAIN REGISTRATION LOOKUP
Objective

To identify the domain registration information, including the registrar, domain creation date, expiration date, and name servers.

Tool Used

WHOIS

Command Executed
bash
whois networkwalks.com

Procedure
Open Kali Linux.
Open the terminal.
Enter the WHOIS command.
Press Enter.
Review the domain registration information.
Save the output in a text file.
Screenshot – Task 1

[INSERT YOUR TASK 1 WHOIS TERMINAL SCREENSHOT HERE]

Output / Findings

Paste the actual command output or summarize the following information:

Registrar:
Domain Registration Date:
Domain Expiration Date:
Domain Name Servers:
Domain Status:
Registrant Information (if publicly available):
Observation

The WHOIS tool provides publicly available domain registration information. It helps identify the registrar, registration dates, and name servers associated with a domain.

3. TASK 2 – WEBSITE TECHNOLOGY FINGERPRINTING
Objective

To identify the technologies used by the website, including its web server, Content Management System (CMS), plugins, frameworks, and other detectable technologies.

Tool Used

WhatWeb

Command Executed
bash
whatweb networkwalks.com

Procedure
Open the Kali Linux terminal.
Enter the WhatWeb command.
Press Enter.
Examine the detected website technologies.
Save the output in a text file.
Screenshot – Task 2

[INSERT YOUR TASK 2 WHATWEB TERMINAL SCREENSHOT HERE]

Output / Findings

Record the actual results:

Website IP Address:
Web Server:
CMS:
Detected Plugins:
Programming Technologies:
Other Information:
Observation

WhatWeb helps identify technologies used by a website. This information allows cybersecurity professionals to understand the website's technology stack and assess whether software components require security updates.

4. TASK 3 – DNS LOOKUP
Objective

To resolve the domain name into its corresponding IP address using DNS lookup.

Tool Used

NSLookup

Command Executed
bash
nslookup networkwalks.com

Procedure
Open the Kali Linux terminal.
Enter the NSLookup command.
Press Enter.
Observe the DNS server and resolved IP address.
Save the output in a text file.
Screenshot – Task 3

[INSERT YOUR TASK 3 NSLOOKUP TERMINAL SCREENSHOT HERE]

Output / Findings
DNS Server:
Domain Name:
Resolved IP Address:
Additional IP Addresses (if available):
Observation

NSLookup is used to query DNS servers and find the IP address associated with a domain name. This helps understand how domain names are translated into network addresses.

5. TASK 4 – HTTP RESPONSE HEADER ANALYSIS
Objective

To retrieve and examine the HTTP response headers returned by the website.

Tool Used

cURL

Command Executed
bash
curl -I https://networkwalks.com

Procedure
Open the Kali Linux terminal.
Enter the cURL command.
Press Enter.
Review the HTTP response status and headers.
Save the output in a text file.
Screenshot – Task 4

[INSERT YOUR TASK 4 CURL TERMINAL SCREENSHOT HERE]

Output / Findings

Record the actual results:

HTTP Status Code:
Server:
Content-Type:
Date:
Cache Information:
Redirect Information:
Other Security Headers:
Observation

The cURL command retrieves HTTP response headers without downloading the complete webpage. These headers provide information about the web server, response status, content type, caching, and other server configurations.

6. TASK 5 – WEB APPLICATION FIREWALL DETECTION
Objective

To identify whether a Web Application Firewall (WAF) is detected on the target website.

Tool Used

WAFW00F

Command Executed
bash
wafw00f networkwalks.com

Procedure
Open the Kali Linux terminal.
Enter the WAFW00F command.
Press Enter.
Review the detection results.
Save the output in a text file.
Screenshot – Task 5

[INSERT YOUR TASK 5 WAFW00F TERMINAL SCREENSHOT HERE]

Output / Findings
WAF Detected: Yes / No
WAF Name:
Additional Information:
Observation

WAFW00F helps identify whether a website is protected by a Web Application Firewall. A WAF monitors and filters incoming web traffic to help protect applications from malicious requests.

7. TASK 6 – DNS RECORD ENUMERATION
Objective

To enumerate publicly available DNS records associated with the target domain.

Tool Used

DNSRecon

Command Executed
bash
dnsrecon -d networkwalks.com

Procedure
Open the Kali Linux terminal.
Enter the DNSRecon command.
Press Enter.
Examine the DNS records returned by the tool.
Save the output in a text file.
Screenshot – Task 6

[INSERT YOUR TASK 6 DNSRECON TERMINAL SCREENSHOT HERE]

Output / Findings

Record the actual results:

A Records:
AAAA Records:
NS Records:
MX Records:
TXT Records:
SPF Records:
SRV Records:
Other DNS Information:
Observation

DNSRecon helps identify publicly available DNS records associated with a domain. These records provide information about domain resolution, mail servers, name servers, and other internet services.

8. SUMMARY OF RESULTS

The following table summarizes the six reconnaissance tasks performed during this project.

Task	Tool	Purpose	Status
1	WHOIS	Domain registration lookup	Completed / Pending
2	WhatWeb	Website technology fingerprinting	Completed / Pending
3	NSLookup	DNS and IP resolution	Completed / Pending
4	cURL	HTTP header analysis	Completed / Pending
5	WAFW00F	WAF detection	Completed / Pending
6	DNSRecon	DNS record enumeration	Completed / Pending
9. CONCLUSION

In this project, I learned how to perform basic footprinting and reconnaissance using six different Kali Linux tools.

I used WHOIS to examine domain registration details, WhatWeb to identify website technologies, and NSLookup to resolve domain names into IP addresses.

I also used cURL to examine HTTP response headers, WAFW00F to check for Web Application Firewall detection, and DNSRecon to enumerate publicly available DNS records.

This practical exercise improved my understanding of reconnaissance techniques and the importance of gathering information during the initial stages of cybersecurity assessments.

These tools can also help website administrators and security professionals understand what information their websites expose publicly and identify opportunities to improve security.

10. REFERENCES
Kali Linux Official Documentation – https://www.kali.org/
WHOIS – https://www.icann.org/
WhatWeb – https://github.com/urbanadventurer/WhatWeb
cURL – https://curl.se/
WAFW00F – https://github.com/EnableSecurity/wafw00f
DNSRecon – https://github.com/darkoperator/dnsrecon

End of Report
