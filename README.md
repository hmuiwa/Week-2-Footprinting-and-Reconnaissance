# WEEK 2 
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

### Task 2: Web Technology Fingerprinting

**Objective:** Identify the web server, CMS, frameworks, plugins, and other technologies used by the target website.

```bash
whatweb networkwalks.com
```

**Evidence:**  
- Screenshot: `screenshots/task-2-whatweb.png`

### Task 3: DNS Resolution

**Objective:** Resolve the domain name into its associated IP address.

```bash
nslookup networkwalks.com
```

**Evidence:**  
- Screenshot: `screenshots/task-3-nslookup.png`

### Task 4: HTTP Response Header Analysis

**Objective:** Retrieve and analyze the HTTP response headers returned by the target website.

```bash
curl -I https://networkwalks.com
```

**Evidence:**  
- Screenshot: `screenshots/task-4-curl-headers.png`

### Task 5: Web Application Firewall Detection

**Objective:** Identify whether a Web Application Firewall is protecting the target website.

```bash
wafw00f networkwalks.com
```

**Evidence:**  
- Screenshot: `screenshots/task-5-wafw00f.png`

### Task 6: DNS Enumeration

**Objective:** Enumerate publicly available DNS records, including NS, MX, TXT, and other discovered records.

```bash
dnsrecon -d networkwalks.com
```

**Evidence:**  
- Screenshot: `screenshots/task-6-dnsrecon.png`

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


# Network Scanning with Zenmap

## 📌 Project Overview

This project focuses on network scanning and host discovery using Zenmap, the graphical user interface (GUI) for Nmap.

The objective is to identify live hosts within a local area network (LAN), discover their IP and MAC addresses, determine the number of active devices, and visualize the network topology.

This practical exercise was conducted using Zenmap on a Windows PC.

## 🎯 Objectives

- Download and install Zenmap on Windows.
- Identify the local IP address and LAN subnet.
- Perform a ping scan to discover live hosts.
- Determine the number of active hosts.
- Identify the IP addresses of discovered hosts.
- Identify the MAC addresses of discovered hosts.
- Generate and export a network topology diagram as a PDF.

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Zenmap | GUI-based network scanning |
| Nmap | Network discovery and scanning engine |
| Windows CMD | IP configuration and MAC address identification |
| ipconfig | Retrieve local network configuration |

## 🎯 Lab Environment

- **Operating System:** Windows
- **Scanning Tool:** Zenmap
- **Network Type:** Local Area Network (LAN)
- **Scan Type:** Ping Scan
- **Subnet:** 10.0.0.0/24 (instructor's example; actual subnet may differ)

## 🧪 Tasks Performed

### Task 1: Download and Install Zenmap

Zenmap was downloaded from the official Nmap website and installed on the Windows PC.

Official download page: https://nmap.org/download.html

### Task 2: Identify Local IP Address and LAN Subnet

The Windows Command Prompt was used to identify the local IP address and network configuration.

```cmd
ipconfig
```

### Task 3: Discover Live Hosts

A Ping Scan was performed in Zenmap to identify active hosts within the local subnet.

Example target subnet:

```text
192.168.0.0/24
```

### Task 4: Determine the Number of Live Hosts

The scan identified four live hosts, including the scanning PC, according to the provided lab results.

### Task 5: Identify IP Addresses of Live Hosts

The discovered IP addresses were:

```text
192.168.0.100
192.168.0.101
```

### Task 6: Identify MAC Addresses of Live Hosts

The MAC addresses identified during the lab were:

```text
B4:0F:3B:5B:0C:90
04:95:E6:CF:39:18
```

The local PC's MAC address can be obtained using:

```cmd
ipconfig /all
```

### Task 7: Generate Network Topology

Zenmap's Topology tab was used to visualize the discovered hosts and their network relationships.

The topology was exported as a PDF file and saved for documentation.

## 📊 Results

- **Total Live Hosts:** 4
- **Scan Type:** Ping Scan
- **IP Addresses Identified:** 4
- **MAC Addresses Identified:** 4
- **Network Topology:** Exported as PDF

## 🧠 Skills Acquired

- Network scanning
- Host discovery
- LAN subnet identification
- IP address enumeration
- MAC address identification
- Nmap and Zenmap usage
- Network topology visualization
- Windows network troubleshooting

## 📸 Evidence

Screenshots of the tasks performed are available in the `screenshots/` directory.

The exported network topology PDF is stored in the `reports/` directory.

## 📝 Conclusion

This project provided practical experience in network scanning and host discovery using Zenmap. I learned how to identify live devices within a local network, retrieve their IP and MAC addresses, and visualize the network topology.

The exercise strengthened my understanding of network reconnaissance and the importance of identifying active hosts during a cybersecurity assessment.

## ⚠️ Disclaimer

This project was conducted for educational purposes. Network scanning should only be performed on networks and devices for which you have explicit authorization.


## ⚠️ Disclaimer

This project is intended for educational purposes and authorized cybersecurity training only. Reconnaissance activities were conducted within the scope of the assigned lab. Always obtain proper authorization before testing any domain or system.
