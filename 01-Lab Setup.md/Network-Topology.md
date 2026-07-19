# Network Topology

## Objective

The objective of this lab setup is to create a simple and controlled environment for capturing and analyzing network traffic using Wireshark. The Windows 11 system functions as both the traffic generator and the packet analysis workstation.

---

## Lab Environment

| Component | Details |
|-----------|----------|
| Host Operating System | Windows 11 |
| Packet Analyzer | Wireshark |
| Network Interface | Wi-Fi / Ethernet |
| Internet Connection | Home Router |
| Traffic Sources | Web Browser, Command Prompt, PowerShell |
| Capture Format | PCAPNG |

---

## Network Topology

![Network Topology](../screenshots/network-topology.png)

---

## Topology Description

The lab consists of a single Windows 11 system connected to the Internet through a home router. Wireshark captures network traffic directly from the active network interface while various applications generate network packets.

Traffic is generated using common Windows utilities and applications, including:

- Web Browser (HTTP/HTTPS)
- Command Prompt (ICMP using `ping`)
- PowerShell
- SSH Client
- FTP Client
- Windows Networking Services

This setup provides a realistic environment for analyzing network protocols and investigating packet-level communication without requiring additional virtual machines.

---

## Traffic Captured During the Project

The following protocols are analyzed throughout this project:

| Protocol | Purpose |
|----------|---------|
| ARP | Address Resolution |
| ICMP | Network Connectivity |
| DNS | Name Resolution |
| HTTP | Web Traffic |
| HTTPS | Secure Web Traffic |
| FTP | File Transfer |
| SSH | Secure Remote Login |
| DHCP | IP Address Assignment |
| TCP | Reliable Communication |
| UDP | Connectionless Communication |

---

## Why This Topology?

This topology was selected because it reflects a typical endpoint environment found in enterprise networks. It allows packet capture from real user activity while keeping the lab simple, reproducible, and focused on network traffic analysis.

---

## Learning Outcomes

After completing this lab setup, the following objectives were achieved:

- Configured a Windows-based packet analysis environment.
- Prepared the system for live network packet capture.
- Identified the active network interface.
- Established a foundation for protocol analysis and incident investigation in subsequent sections.
