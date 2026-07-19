# Wireshark Network Traffic Analysis & Incident Investigation Lab

## Overview

This project is a hands-on network traffic analysis and incident investigation lab built using **Wireshark**. The objective is to understand how different network protocols operate, analyze captured packets, identify suspicious network activities, and perform basic incident investigation from packet capture (PCAP) files.

The project follows a structured learning approach beginning with packet capture fundamentals and progressing towards real-world security investigations such as port scanning, brute-force attacks, suspicious traffic analysis, malware communication, and network incident reporting.

This repository demonstrates practical skills expected from entry-level SOC (Security Operations Center) analysts.

---

## Objectives

- Learn packet capturing using Wireshark
- Understand common network protocols
- Analyze TCP/IP communications
- Identify abnormal network behaviour
- Investigate common cyber attack patterns
- Practice packet filtering techniques
- Build basic incident investigation skills
- Create professional investigation reports

---

# Project Structure

```
Wireshark-Network-Traffic-Analysis
│
├── README.md
│
├── 01-Lab-Setup
│   ├── Network-Topology.md
│   ├── Installing-Wireshark.md
│   └── Capture-Configuration.md
│
├── 02-Basic-Traffic-Analysis
│   ├── ICMP.md
│   ├── ARP.md
│   ├── DNS.md
│   ├── HTTP.md
│   ├── HTTPS.md
│   ├── FTP.md
│   ├── SSH.md
│   └── DHCP.md
│
├── 03-Protocol-Analysis
│   ├── TCP-Handshake.md
│   ├── UDP.md
│   ├── TCP-Retransmissions.md
│   ├── TCP-Flags.md
│   ├── Fragmentation.md
│   └── Conversations.md
│
├── 04-Network-Investigation
│   ├── Suspicious-IP.md
│   ├── Port-Scan-Detection.md
│   ├── Brute-Force-Attack.md
│   ├── DNS-Tunneling-Basics.md
│   ├── HTTP-Credential-Leak.md
│   └── Malware-Traffic-Basics.md
│
├── 05-Filtering-Techniques
│   ├── Display-Filters.md
│   ├── Capture-Filters.md
│   ├── Coloring-Rules.md
│   ├── Follow-TCP-Stream.md
│   └── Exporting-Objects.md
│
├── 06-Case-Studies
│   ├── Case-1-Employee-Web-Browsing.md
│   ├── Case-2-FTP-File-Transfer.md
│   ├── Case-3-Suspicious-Network-Traffic.md
│   └── Case-4-Network-Incident-Report.md
│
├── Findings.md
├── Recommendations.md
│
├── pcap-files
├── screenshots
└── reports
```

---

# Lab Environment

| Component | Details |
|-----------|---------|
| Operating System | Kali Linux |
| Packet Analyzer | Wireshark |
| Test Machine | Windows / Kali Linux |
| Network Type | NAT / Host-Only (Virtual Environment) |
| Packet Sources | Live Capture & PCAP Files |

---

# Topics Covered

### Lab Setup

- Installing Wireshark
- Network topology
- Capture configuration
- Selecting interfaces
- Packet capture basics

---

### Basic Traffic Analysis

- ICMP
- ARP
- DNS
- HTTP
- HTTPS
- FTP
- SSH
- DHCP

---

### Protocol Analysis

- TCP Three-Way Handshake
- UDP Communication
- TCP Flags
- TCP Retransmissions
- IP Fragmentation
- Endpoint Conversations

---

### Network Investigation

- Suspicious IP Analysis
- Port Scan Detection
- Brute Force Attack Detection
- DNS Tunneling Basics
- HTTP Credential Leakage
- Malware Traffic Identification

---

### Wireshark Features

- Display Filters
- Capture Filters
- Coloring Rules
- Follow TCP Stream
- Exporting Objects
- Packet Inspection

---

### Incident Case Studies

- Employee Web Browsing Investigation
- FTP File Transfer Investigation
- Suspicious Network Activity Investigation
- Network Incident Report

---

# Skills Demonstrated

- Network Traffic Analysis
- Packet Inspection
- TCP/IP Analysis
- Network Protocol Analysis
- Incident Investigation
- Threat Hunting Basics
- IOC Identification
- Packet Filtering
- Log Analysis
- Security Documentation
- Report Writing
- Wireshark

---

# Tools Used

- Wireshark
- Kali Linux
- Windows
- Command Prompt
- Linux Terminal
- Ping
- nslookup
- dig
- ftp
- ssh
- curl
- netcat

---

# Repository Workflow

```
Generate Network Traffic
        │
        ▼
Capture Packets
        │
        ▼
Analyze Protocols
        │
        ▼
Apply Filters
        │
        ▼
Investigate Suspicious Activity
        │
        ▼
Document Findings
        │
        ▼
Prepare Incident Report
```

---

# Key Learning Outcomes

By completing this project, I gained practical experience in:

- Capturing and analyzing live network traffic
- Understanding packet-level communication
- Investigating common network attacks
- Detecting suspicious behaviour using Wireshark
- Applying display and capture filters efficiently
- Interpreting protocol fields and packet headers
- Preparing technical findings and investigation reports

---

# Screenshots

Project screenshots are available inside the `screenshots/` directory.

---

# PCAP Files

Sample packet captures used during analysis are available inside the `pcap-files/` directory.

---

# Reports

Detailed investigation reports are available inside the `reports/` directory.

---

# Findings

Major observations and security findings are documented in:

- `Findings.md`

---

# Recommendations

Security recommendations and mitigation strategies are documented in:

- `Recommendations.md`

---

# Disclaimer

This project is created strictly for educational purposes and cybersecurity training. All traffic captures and investigations were performed in a controlled lab environment.

---

## Author

**YASH SHRIVASTAVA**
