# TCP Retransmission Analysis

## Objective

Identify and analyze TCP retransmissions using Wireshark.

---

## Background

TCP retransmissions occur when a sender does not receive an acknowledgment for a transmitted packet within the expected time. Retransmissions help ensure reliable data delivery.

---

## Traffic Generation

Network traffic was captured while downloading a file or browsing websites. If retransmissions were not naturally present, a publicly available sample PCAP containing retransmissions can be analyzed.

---

## Packet Capture

1. Start Wireshark.
2. Capture traffic during web browsing or file download.
3. Stop capture.
4. Save as:

```
tcp-retransmission.pcapng
```

---

## Display Filter

```
tcp.analysis.retransmission
```

---

## Packet Analysis

Observed:

- Retransmitted TCP packets
- Original Sequence Number
- Duplicate Transmission
- Delayed Acknowledgment

---

## Important Packet Fields

| Field | Description |
|--------|-------------|
| Sequence Number | Retransmitted sequence |
| Acknowledgment Number | Receiver acknowledgment |
| Expert Information | Indicates retransmission |
| Time Delta | Delay before retransmission |

---

## Findings

- Retransmissions occurred due to delayed acknowledgments or packet loss.
- Wireshark identified retransmitted packets using Expert Information.

---

## Conclusion

TCP retransmissions improve communication reliability by resending lost or unacknowledged packets. Frequent retransmissions may indicate network congestion or connectivity issues.

---

## Screenshots

- Retransmission Filter
- Expert Information
- Retransmitted Packet
