# Port Scan Detection

## Objective

Identify a TCP port scan using Wireshark.

---

## Background

Attackers commonly perform port scans to identify open services before attempting exploitation. Detecting port scanning activity is a fundamental SOC monitoring task.

---

## Data Source

Sample PCAP containing an Nmap TCP SYN scan.

File:

```
port-scan.pcapng
```

---

## Investigation Procedure

1. Open the PCAP.
2. Apply TCP SYN filter.
3. Review destination ports.
4. Identify repeated SYN packets.

---

## Display Filters

TCP SYN packets

```
tcp.flags.syn == 1 && tcp.flags.ack == 0
```

Source IP

```
ip.src == <Scanner_IP>
```

---

## Analysis

Observed:

- Multiple SYN packets.
- Sequential destination ports.
- No application data.
- Large number of connection attempts.

---

## Indicators of Compromise (IOCs)

- High number of SYN packets.
- Connections to many destination ports.
- Short time interval.
- Single source IP.

---

## Findings

Traffic pattern matched a TCP SYN Port Scan.

---

## Conclusion

The observed communication demonstrated reconnaissance activity commonly associated with network scanning.

---

## Screenshots

- SYN Filter
- Port Scan Activity
- Destination Ports
- Expert Information
