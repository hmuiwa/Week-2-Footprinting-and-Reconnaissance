# WEEK 2 | PROJECT MODULE 1
# Footprinting & Reconnaissance Attacks Using Multiple Kali Linux Tools

## 📌 Project Overview

This project focuses on Footprinting and Reconnaissance, the initial phase of a cybersecurity assessment. The objective is to gather publicly available information about a target domain using multiple Kali Linux tools.

Reconnaissance helps security professionals understand a target's domain registration details, DNS infrastructure, web technologies, HTTP response headers, and Web Application Firewall (WAF) protection.

In this practical lab, six Kali Linux tools are used to perform passive and non-intrusive information gathering against the assigned target.

## 🎯 Objectives

- Identify domain registration information using WHOIS.
- Fingerprint web technologies using WhatWeb.
- Resolve domain names to IP addresses using NSLookup.
- Analyze HTTP response headers using cURL.
- Detect Web Application Firewall technologies using WAFW00F.
- Enumerate DNS records using DNSRecon.
- Document findings, command outputs, and screenshots.

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| WHOIS | Domain registration information |
| WhatWeb | Web technology fingerprinting |
| NSLookup | DNS resolution |
| cURL | HTTP response header analysis |
| WAFW00F | WAF detection |
| DNSRecon | DNS enumeration |

## 🎯 Target Information

- **Target Domain:** networkwalks.com
- **Target URL:** https://networkwalks.com
- **Operating System:** Kali Linux
- **Project:** Week 2 – Project Module 1

## 🧪 Tasks Performed

### Task 1: WHOIS Enumeration

**Objective:** Retrieve public domain registration details, registrar information, registration dates, and name servers.

```bash
whois networkwalks.com
```

**Evidence:**  
- Screenshot: `screenshots/task-1-whois.png`
- Output: `outputs/whois.txt`

### Task 2: Web Technology Fingerprinting

**Objective:** Identify the web server, CMS, frameworks, plugins, and other technologies used by the target website.

```bash
whatweb networkwalks.com
```

**Evidence:**  
- Screenshot: `screenshots/task-2-whatweb.png`
- Output: `outputs/whatweb.txt`

### Task 3: DNS Resolution

**Objective:** Resolve the domain name into its associated IP address.

```bash
nslookup networkwalks.com
```

**Evidence:**  
- Screenshot: `screenshots/task-3-nslookup.png`
- Output: `outputs/nslookup.txt`

### Task 4: HTTP Response Header Analysis

**Objective:** Retrieve and analyze the HTTP response headers returned by the target website.

```bash
curl -I https://networkwalks.com
```

**Evidence:**  
- Screenshot: `screenshots/task-4-curl-headers.png`
- Output: `outputs/curl-headers.txt`

### Task 5: Web Application Firewall Detection

**Objective:** Identify whether a Web Application Firewall is protecting the target website.

```bash
wafw00f networkwalks.com
```

**Evidence:**  
- Screenshot: `screenshots/task-5-wafw00f.png`
- Output: `outputs/wafw00f.txt`

### Task 6: DNS Enumeration

**Objective:** Enumerate publicly available DNS records, including NS, MX, TXT, and other discovered records.

```bash
dnsrecon -d networkwalks.com
```

**Evidence:**  
- Screenshot: `screenshots/task-6-dnsrecon.png`
- Output: `outputs/dnsrecon.txt`

## 📊 Findings

The reconnaissance process helps identify:

- Domain registration and registrar information.
- Public IP address and DNS infrastructure.
- Web technologies and server configurations.
- HTTP response headers and server information.
- Possible Web Application Firewall protection.
- Mail servers and other DNS records.

Actual findings will be documented based on the collected command outputs.

## 📸 Screenshots

Screenshots of each task are stored in the `screenshots/` directory to provide evidence of the practical work performed.

## 🧠 Skills Acquired

- Linux command-line operations
- Domain footprinting
- DNS enumeration
- Web technology fingerprinting
- HTTP header analysis
- WAF detection
- Cybersecurity documentation
- Information gathering and reconnaissance

## 📝 Conclusion

This project provided practical experience in performing footprinting and reconnaissance using multiple Kali Linux tools. Each tool revealed different aspects of the target's publicly accessible infrastructure.

The exercise strengthened my understanding of information gathering, DNS analysis, web technology identification, and the importance of reconnaissance during a security assessment.

## ⚠️ Disclaimer

This project is intended for educational purposes and authorized cybersecurity training only. Reconnaissance activities were conducted within the scope of the assigned lab. Always obtain proper authorization before testing any domain or system.
