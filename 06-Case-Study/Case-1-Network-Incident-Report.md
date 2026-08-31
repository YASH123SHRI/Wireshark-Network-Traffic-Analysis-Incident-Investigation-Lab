# Case Study 1 – Network Incident Investigation Report

## 1. Incident Overview

### Case ID
CASE - 001


### Investigation Type
Network Traffic Analysis

### Analyst
Yash Shrivastava

### Date
31-08-2026

### Severity
Low

---

## 2. Executive Summary

A network traffic capture was investigated using Wireshark to identify potentially suspicious communication between internal and external hosts.

The investigation focused on identifying unusual network behavior, suspicious endpoints, communication patterns, protocols, and potential indicators of compromise.

The analysis identified:

- [Finding 1]
- [Finding 2]
- [Finding 3]

Based on the available network evidence, the activity was assessed as:
Benign

---

## 3. Investigation Objective

The objectives of this investigation were to:

1. Identify the hosts involved in the incident.
2. Identify suspicious IP addresses.
3. Analyze network conversations.
4. Identify unusual ports or protocols.
5. Examine suspicious communication patterns.
6. Extract relevant Indicators of Compromise (IOCs).
7. Determine whether the observed activity requires further investigation.

---

## 4. Evidence

### PCAP File

```text
pcap-files/case-1-network-incident.pcapng
```

Analysis Tool -
Wireshark

Operating System -
Windows 11

The following Wireshark features were used:
- Statistics → Endpoints
- Statistics → Conversations
- Statistics → Protocol Hierarchy

<img width="1919" height="440" alt="image" src="https://github.com/user-attachments/assets/5fdf0f9d-e708-4a06-aa11-f10a3cf0ae17" />
<img width="1919" height="460" alt="image" src="https://github.com/user-attachments/assets/d0d2d603-ef31-469f-b2db-b9670dd46be1" />
<img width="1515" height="824" alt="image" src="https://github.com/user-attachments/assets/650b87d7-a178-4a08-82cc-f0156e976356" />

Internal Host
IP Address: 10.151.238.1

External Host
IP Address: 20.184.175.2

<img width="1919" height="1016" alt="image" src="https://github.com/user-attachments/assets/a1383a9a-eda2-4bc7-84c6-4723b77aa4bf" />
<img width="1919" height="986" alt="image" src="https://github.com/user-attachments/assets/594efee7-a63f-4637-98cf-2af954d7c30f" />


## Risk Assessment

Likelihood
Low

Overall Risk
Low

## Limitations

This investigation was performed using network traffic contained within the provided PCAP.
The PCAP alone may not provide sufficient evidence to determine whether the activity was definitively malicious.

Additional evidence such as:

Windows Event Logs
Endpoint Detection and Response (EDR) data
DNS logs
Firewall logs
Proxy logs
Threat intelligence

may be required for confirmation.
