# Suspicious IP Investigation

## Objective

Identify suspicious IP addresses from captured network traffic using Wireshark and perform a basic network investigation.

---

## Background

During network monitoring, analysts often encounter unknown or suspicious IP addresses communicating with internal systems. The objective is to determine whether the communication appears legitimate or requires further investigation.

---

## Data Source

Sample PCAP containing multiple network conversations.

File:

```
suspicious-ip.pcapng
```

---

## Investigation Procedure

1. Open the PCAP in Wireshark.
2. Navigate to:

```
Statistics
    ↓
Endpoints
```

3. Review all IPv4 addresses.
4. Identify external IP addresses with unusual communication.
5. Review conversations involving the suspicious IP.

---

## Display Filters

Filter by IP

```
ip.addr == <Suspicious_IP>
```

Example

```
ip.addr == 203.0.113.25
```

---

## Analysis

Review the following:

- Source IP
- Destination IP
- Protocol
- Destination Port
- Packet Count
- Data Volume

---

## Findings

- Identified communication with an external IP address.
- Observed multiple TCP connections.
- Traffic volume was higher than normal.
- Further investigation was recommended.

---

## Conclusion

Endpoint and conversation analysis successfully identified potentially suspicious communication requiring additional investigation.

---

## Screenshots

- Endpoints Window
- Conversations Window
- Suspicious IP Filter
- Packet Details

<img width="1919" height="1020" alt="image" src="https://github.com/user-attachments/assets/9beb58d3-d9f0-4882-bd80-ad0ed098677b" />

<img width="1919" height="1021" alt="image" src="https://github.com/user-attachments/assets/dd8f114d-746f-4cba-b7da-53747c3a6756" />
