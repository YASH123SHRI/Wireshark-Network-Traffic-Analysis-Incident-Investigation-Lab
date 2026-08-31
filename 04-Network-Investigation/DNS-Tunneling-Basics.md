# DNS Tunneling Analysis (Basic)

## Objective

Analyze DNS traffic to identify characteristics commonly associated with DNS tunneling.

---

## Background

DNS tunneling is a technique where DNS queries and responses are used to carry data instead of normal domain name lookups. Since DNS traffic is usually allowed through firewalls, attackers may abuse it for data exfiltration or command-and-control (C2) communication.

This exercise focuses on identifying suspicious DNS behavior rather than confirming malicious activity.

---

## Data Source

Sample PCAP containing DNS tunneling traffic.

## Investigation Procedure

1. Open the PCAP in Wireshark.
2. Apply the DNS display filter.
3. Review DNS query names.
4. Identify unusually long or random-looking domain names.
5. Review query frequency and destination IP addresses.

---

## Display Filters

Show all DNS packets:

```
dns
```

DNS Queries Only:

```
dns.flags.response == 0
```

---

## Analysis

Review the following:

- Query Name
- Query Type
- Destination IP
- Query Frequency
- Length of Requested Domain

---

## Indicators of Suspicious Activity

- Long random-looking subdomains
- High volume of DNS requests
- Repeated queries to one domain
- Encoded strings within subdomains
- Unusual DNS traffic frequency

---

## Findings

- Multiple DNS queries contained unusually long subdomains.
- High query frequency was observed.
- Traffic pattern differed from normal DNS activity.

---

## Conclusion

The analyzed traffic demonstrated characteristics commonly associated with DNS tunneling. Additional investigation would be required to confirm malicious activity.

---

## Screenshot

- DNS Display Filter

<img width="1919" height="1024" alt="image" src="https://github.com/user-attachments/assets/b73d63ca-1295-4f88-a825-2908ab5183d5" />

- Suspicious DNS Queries

<img width="1919" height="1022" alt="image" src="https://github.com/user-attachments/assets/c253bcd6-419f-4849-b570-e49865536b5e" />

- Packet Details

<img width="936" height="503" alt="image" src="https://github.com/user-attachments/assets/8df06cd0-3d50-4a36-bc18-a2c27412f075" />

- Conversation Statistics

<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/5d5cb76e-cf95-49e5-9954-a3b0414bba8c" />
