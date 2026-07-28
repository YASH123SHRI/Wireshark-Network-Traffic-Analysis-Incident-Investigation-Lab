# Brute Force Attack Investigation

## Objective

Investigate repeated authentication attempts indicating a possible brute-force attack.

---

## Background

A brute-force attack attempts multiple username and password combinations until successful authentication occurs. Repeated failed login attempts within a short period are a common indicator.

---

## Data Source

Sample PCAP containing multiple login attempts.

File:

```
brute-force.pcapng
```

---

## Investigation Procedure

1. Open the PCAP.
2. Identify authentication protocol.
3. Review repeated login attempts.
4. Count failed attempts.
5. Identify source IP.

---

## Display Filters

FTP

```
ftp
```

SSH

```
ssh
```

TCP Port

```
tcp.port == 21
```

or

```
tcp.port == 22
```

---

## Analysis

Review:

- Source IP
- Destination IP
- Authentication attempts
- Server responses
- Connection frequency

---

## Indicators of Compromise (IOCs)

- Numerous login attempts.
- Short time interval.
- Same source IP.
- Repeated authentication failures.

---

## Findings

Traffic demonstrated characteristics of a brute-force login attack.

---

## Conclusion

Repeated authentication failures indicate malicious login attempts requiring defensive action.

---

## Screenshots

- Login Attempts
- Authentication Packets
- Source IP
- Packet Timeline
