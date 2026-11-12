# wk2-Network-Scanning---Footprinting-
Hands-on Cybersecurity Internship lab repository covering OSINT, footprinting, and network discovery workflows in Kali Linux using theHarvester, Nmap, and Zenmap.
🛡️ Cybersecurity Internship – Week 2: Footprinting & Network Scanning

📌 Overview

This repository documents my Week 2 hands-on practical tasks for my Cybersecurity Internship. The primary focus of this module was Information Gathering, Passive Reconnaissance (OSINT), Footprinting, and Active Network Scanning within a Kali Linux environment.

🛠️ Tools & Technologies Used

Operating System: Kali Linux

OSINT & Footprinting: theHarvester

Network Scanning & Visualization: Nmap, Zenmap

Networking Utilities: ifconfig, ping

📋 Practical Tasks Breakdown

🔹 Task 1: theHarvester – OSINT & Footprinting

Used theHarvester in Kali Linux to gather publicly available intelligence (emails, subdomains, and hosts) related to the target organization microsoft.com.

Activities & Commands Executed:

Targeted Data Source Collection (Baidu):

Gathered email IDs and subdomains using Baidu as the search engine source with a result limit of 1,000.

theHarvester -d microsoft.com -l 1000 -b baidu


Multi-Source OSINT Aggregation:

Conducted a broader reconnaissance scan querying all available public data sources with a result limit of 50.

theHarvester -d microsoft.com -l 50 -b all


Analysis:

Evaluated how Open-Source Intelligence (OSINT) tools uncover publicly exposed organizational assets and digital footprints without directly interacting with target infrastructure.

🔹 Task 2: Zenmap & Nmap – Network Scanning & Host Discovery

Utilized Nmap and its graphical user interface, Zenmap, to perform active network discovery and map live hosts within a local subnet.

Activities & Commands Executed:

Network Interface & IP Identification:

Inspected local network interfaces, IP addresses, and subnet masks.

ifconfig


Connectivity Verification:

Verified network reachability and latency using ICMP echo requests.

ping -c 4 <target-IP>


Subnet Host Discovery (Ping Scan):

Executed a host discovery scan across the local /24 CIDR subnet to identify active devices without performing a full port scan.

nmap -sn <your-IP>/24


GUI Visualization:

Explored Zenmap to visualize network topology, compare scan profiles, and analyze host details in a structured interface.

💡 Key Learnings

Passive vs. Active Reconnaissance: Understanding the distinction between gathering public OSINT data (theHarvester) and actively probing network ranges (Nmap).

Attack Surface Awareness: Identifying how publicly indexed emails and subdomains can expand an organization's external footprint.

Subnetting & CIDR Notation: Applying /24 subnet masks to define scanning scopes accurately.

Host Discovery: Using ICMP/ARP ping sweeps (-sn) to efficiently enumerate live hosts on a local network.

⚠️ Disclaimer

All activities and scans documented in this repository were performed strictly for educational purposes as part of a structured cybersecurity internship. Passive OSINT queries targeted publicly accessible search engines, and active network scans were confined exclusively to an authorized local lab environment.
