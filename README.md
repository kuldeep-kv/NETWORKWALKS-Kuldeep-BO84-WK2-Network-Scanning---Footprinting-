# 🚀 Week 2 Submission | Cybersecurity Internship – Footprinting & Network Scanning

![Kali Linux](https://img.shields.io/badge/OS-Kali%20Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)
![OSINT](https://img.shields.io/badge/Focus-OSINT%20%26%20Reconnaissance-2ea44f?style=for-the-badge)
![Nmap](https://img.shields.io/badge/Tool-Nmap%20%2F%20Zenmap-00599C?style=for-the-badge)

Continuing my cybersecurity learning journey with another week of hands-on practical tasks focused on **Information Gathering, Footprinting, and Network Scanning** using Kali Linux.

---

## 📋 Overview

This week's submission involved working with two important reconnaissance and network discovery tools:

* **theHarvester** for passive OSINT and public footprinting.
* **Zenmap / Nmap** for active host discovery and subnet mapping.

---

## 🔹 Task 1: theHarvester – OSINT & Footprinting

Used **theHarvester** in Kali Linux to gather publicly available information related to the target organization `microsoft.com`.

### Practical Activities
- Collected email IDs and subdomains using **Baidu** as the data source with a search limit of **1,000 results**.
- Performed a broader information-gathering exercise across **all available sources** with a result limit of **50**.
- Explored how OSINT tools help identify publicly exposed organizational infrastructure and contact data.

### Commands Executed

Search using Baidu with a limit of 1,000 results
theHarvester -d microsoft.com -l 1000 -b baidu

Search across all available sources with a limit of 50 results
theHarvester -d microsoft.com -l 50 -b all

🔹 Task 2: Zenmap – Network Scanning & Host Discovery
Worked with Zenmap and Nmap to understand network discovery and identify active hosts within a local subnet.

Practical Activities
Checked local network interfaces and IP configuration using ifconfig.

Verified network reachability and connectivity using ping.

Conducted a host discovery (ping sweep) scan across my local /24 subnet.

Explored how Zenmap provides a graphical interface for network topology visualization and scan profile management.

Commands Executed

# 1. Identify local network interface and IP address
ifconfig

# 2. Verify host connectivity
ping -c 4 <target-or-gateway-IP>

# 3. Discover active hosts on the local /24 subnet
nmap -sn <your-IP>/24

💡 Key LearningsPassive Reconnaissance & OSINT: Gathering intelligence from public search engines without directly interacting with target servers.Attack Surface Mapping: Identifying exposed email addresses and subdomains associated with an organization.Network Addressing: Understanding IP ranges and /24 CIDR subnet notation.Host Discovery: Utilizing Nmap ping scans (-sn) and Zenmap's GUI to enumerate live devices on a local network.Linux Tooling: Building hands-on fluency with Kali Linux terminal workflows.🛡️ Tools & TechnologiesCategoryTools / ConceptsOperating SystemKali LinuxOSINT & FootprintingtheHarvester, BaiduNetwork ScanningNmap, ZenmapCore Utilitiesifconfig, ping, CIDR Notation⚠️ DisclaimerAll reconnaissance and network scanning activities documented in this repository were performed strictly for educational purposes as part of a cybersecurity internship. Always ensure you have explicit authorization before scanning any network or domain.
