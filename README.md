
# 🛡️ CYBERSECURITY LAB | WEEK 02

<div align="center">

# W2-PM1: FOOTPRINTING & RECONNAISSANCE 
### Multi-Tool Security Assessment with Kali Linux

![Kali Linux](https://img.shields.io/badge/OS-Kali%20Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)
![Cybersecurity](https://img.shields.io/badge/Domain-Cybersecurity-0EA5E9?style=for-the-badge)
![Project](https://img.shields.io/badge/Week-02-7C3AED?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-In%20Progress-orange?style=for-the-badge)

**PROJECT MODULE 01**

*Footprinting • Information Gathering • DNS Analysis • Web Fingerprinting*

---

**Student Name:** SANJO

**Course:** Cybersecurity / Ethical Hacking

**Target Domain:** `networkwalks.com`

**Platform:** Kali Linux

**Date:** November 2026

</div>

---

## 📌 01. PROJECT OVERVIEW

Footprinting and reconnaissance are the initial stages of cybersecurity assessments and ethical hacking.

The objective of this project is to collect publicly available information about a domain and understand its internet-facing infrastructure using Kali Linux tools.

This practical project explores six reconnaissance tools to examine domain registration, website technologies, DNS information, HTTP headers, and Web Application Firewall detection.

### 🎯 Project Objectives

- Identify domain registration information.
- Discover website technologies and server details.
- Resolve domain names into IP addresses.
- Analyze HTTP response headers.
- Identify Web Application Firewall protection.
- Enumerate publicly available DNS records.

---

## 🧰 02. TOOLS & TECHNOLOGIES

| No. | Tool | Purpose |
|:---:|---|---|
| 01 | WHOIS | Domain registration lookup |
| 02 | WhatWeb | Website technology fingerprinting |
| 03 | NSLookup | DNS resolution |
| 04 | cURL | HTTP response header analysis |
| 05 | WAFW00F | WAF detection |
| 06 | DNSRecon | DNS record enumeration |

---

# 🔍 03. PRACTICAL TASKS

## TASK 01 — WHOIS DOMAIN LOOKUP

<details>
<summary><b>📖 Click to view task details</b></summary>

### Objective

Identify domain registration information, including registrar, creation date, expiration date, and name servers.

### Tool

`WHOIS`

### Command

```bash
whois networkwalks.com
```

### Procedure

1. Open Kali Linux.
2. Launch the terminal.
3. Execute the WHOIS command.
4. Review the registration details.
5. Save the terminal output in a text file.

### 📸 Screenshot Evidence

**Insert your Task 1 terminal screenshot below:**

<img width="846" height="373" alt="image" src="https://github.com/user-attachments/assets/93d0e87d-e867-40fc-9772-17c2d648c207" />




### Observation

WHOIS provides publicly available domain registration information. It helps identify the registrar, registration dates, and name servers associated with a domain.

</details>

---

## TASK 02 — WEBSITE TECHNOLOGY FINGERPRINTING

<details>
<summary><b>📖 Click to view task details</b></summary>

### Objective

Identify the technologies used by the website, including its web server, CMS, plugins, frameworks, and other detectable components.

### Tool

`WhatWeb`

### Command

```bash
whatweb networkwalks.com
```

### Procedure

1. Open the Kali Linux terminal.
2. Execute the WhatWeb command.
3. Examine the detected technologies.
4. Identify the website's technology stack.
5. Save the terminal output.

### 📸 Screenshot Evidence

<img width="1898" height="180" alt="image" src="https://github.com/user-attachments/assets/1ac537dd-753e-47de-b302-3f70418cb65b" />



### Observation

WhatWeb identifies technologies used by websites. This information helps cybersecurity professionals understand the technology stack and assess whether software components require security updates.

</details>

---

## TASK 03 — DNS LOOKUP

<details>
<summary><b>📖 Click to view task details</b></summary>

### Objective

Resolve the domain name into its corresponding IP address using DNS lookup.

### Tool

`NSLookup`

### Command

```bash
nslookup networkwalks.com
```

### Procedure

1. Open the Kali Linux terminal.
2. Execute the NSLookup command.
3. Observe the DNS server.
4. Identify the resolved IP address.
5. Save the terminal output.

### 📸 Screenshot Evidence

<img width="385" height="144" alt="image" src="https://github.com/user-attachments/assets/b84a6a33-d1dc-4ead-9f71-04907ed285da" />


### Observation

NSLookup queries DNS servers and identifies the IP address associated with a domain name. It helps explain how domain names are translated into network addresses.

</details>

---

## TASK 04 — HTTP RESPONSE HEADER ANALYSIS

<details>
<summary><b>📖 Click to view task details</b></summary>

### Objective

Retrieve and examine HTTP response headers returned by the website.

### Tool

`cURL`

### Command

```bash
curl -I https://networkwalks.com
```

### Procedure

1. Open the Kali Linux terminal.
2. Execute the cURL command.
3. Examine the HTTP response.
4. Identify relevant response headers.
5. Save the terminal output.

### 📸 Screenshot Evidence

<img width="1902" height="182" alt="image" src="https://github.com/user-attachments/assets/f3ed5ec5-fcd9-4faf-b741-ecde710bd8d2" />



### Observation

cURL retrieves HTTP response headers without downloading the complete webpage. These headers provide information about the server response, content type, caching, and server configuration.

</details>

---

## TASK 05 — WEB APPLICATION FIREWALL DETECTION

<details>
<summary><b>📖 Click to view task details</b></summary>

### Objective

Identify whether a Web Application Firewall (WAF) is detected on the target website.

### Tool

`WAFW00F`

### Command

```bash
wafw00f networkwalks.com
```

### Procedure

1. Open the Kali Linux terminal.
2. Execute the WAFW00F command.
3. Review the detection results.
4. Identify whether a WAF was detected.
5. Save the terminal output.

### 📸 Screenshot Evidence

<img width="677" height="337" alt="image" src="https://github.com/user-attachments/assets/eed0da25-57f4-4876-9dad-e061bddf1671" />

### Observation

WAFW00F helps identify whether a website is protected by a Web Application Firewall. A WAF monitors and filters incoming web traffic to help protect web applications from malicious requests.

</details>

---

## TASK 06 — DNS RECORD ENUMERATION

<details>
<summary><b>📖 Click to view task details</b></summary>

### Objective

Enumerate publicly available DNS records associated with the target domain.

### Tool

`DNSRecon`

### Command

```bash
dnsrecon -d networkwalks.com
```

### Procedure

1. Open the Kali Linux terminal.
2. Execute the DNSRecon command.
3. Examine the discovered DNS records.
4. Identify relevant DNS information.
5. Save the terminal output.

### 📸 Screenshot Evidence

<img width="1089" height="434" alt="image" src="https://github.com/user-attachments/assets/002f7afb-b5d6-4509-ba44-8b97343ab2e3" />


### Observation

DNSRecon helps identify publicly available DNS records associated with a domain. These records provide information about domain resolution, mail servers, name servers, and other internet services.

</details>

---


### Key Learning Points

- Understanding passive and active reconnaissance.
- Learning how DNS infrastructure works.
- Identifying publicly exposed website information.
- Understanding HTTP response headers.
- Recognizing the purpose of Web Application Firewalls.
- Developing practical familiarity with Kali Linux tools.

---

---

# W2-PM5: Zenmap based Network Scanning



### 🎯 Objective
Perform network discovery using Zenmap and identify live hosts, IP addresses, and network topology.

### 🛠️ Tools Used
- Zenmap
- Nmap
- Windows CMD

### Step 1 - Download and Install Zenmap

Download Zenmap from the official website:

https://nmap.org/download.html

### Step 2 - Find Local IP Address and LAN Subnet

Open CMD and execute:

```cmd
ipconfig
```

Identify your IPv4 address and subnet mask.

**Screenshot:**

![IP Configuration](Task2/screenshots/ipconfig.png)

### Step 3 - Discover Live Hosts

Open Zenmap, enter your LAN subnet, select Ping Scan, and click Scan.

**Command example:**

```bash
nmap -sn <IP>
```


**Screenshot:**

<img width="1241" height="532" alt="image" src="https://github.com/user-attachments/assets/ed737eea-56cd-4608-bd22-2dd11d78ba7f" />


### Step 4 - Number of Live Hosts

**Answer:** 4 hosts were discovered, including my PC.

### Step 5 - IP Addresses of Live Hosts

- 10.0.2.2
- 10.0.2.3
- 10.0.2.4
- 10.0.2.15

### Step 6 - MAC Addresses

MAC addresses can be checked using:

```cmd
ipconfig /all
```

Actual MAC addresses are omitted from this public report for privacy.

### Step 7 - Network Topology

Open the Topology tab in Zenmap, enable the legend, and save the network topology as a PDF.

**Topology Screenshot:**

<img width="1241" height="619" alt="image" src="https://github.com/user-attachments/assets/ae62b80e-32d4-438d-892e-a7b682966db3" />


### 📚 Key Learnings

- Installed and used Zenmap.
- Identified local IP and subnet.
- Performed Ping Scan.
- Discovered live network hosts.
- Learned about IP and MAC addresses.
- Exported network topology as PDF.


</details>



# ⚠️ 04. DISCLAIMER

This project is intended for educational purposes and authorized cybersecurity assessments only.

All reconnaissance activities should be conducted within an approved scope and with appropriate authorization.

The findings recorded in this repository should reflect actual tool outputs and observations.

---

<div align="center">

## 🛡️ END OF PROJECT

**WEEK 02 | PROJECT MODULE 01**

*Learn • Practice • Analyze • Secure*

![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Education-0EA5E9?style=flat-square)
![Kali Linux](https://img.shields.io/badge/Powered%20By-Kali%20Linux-557C94?style=flat-square)

</div>
