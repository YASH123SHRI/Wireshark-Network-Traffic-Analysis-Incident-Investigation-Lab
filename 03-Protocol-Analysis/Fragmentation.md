# IP Fragmentation Analysis

## Objective

Analyze fragmented IP packets using Wireshark and understand how large packets are divided during transmission.

---

## Background

IP fragmentation occurs when a packet exceeds the Maximum Transmission Unit (MTU) of a network. The packet is divided into smaller fragments, which are reassembled at the destination.

---

## Traffic Generation

Fragmented packets were analyzed using a sample PCAP containing IP fragmentation.

> Note: Fragmentation is uncommon on modern networks. A sample capture is recommended for consistent analysis.

---

## Packet Capture

1. Open Wireshark.
2. Load the fragmentation sample PCAP.
3. Apply the fragmentation filter.
4. Analyze fragmented packets.

---

## Display Filter

```
ip.flags.mf == 1 || ip.frag_offset > 0
```

---

## Packet Analysis

Observed:

- Fragment Offset
- More Fragments Flag
- Identification Field
- Reassembled Packet

---

## Important Packet Fields

| Field | Description |
|--------|-------------|
| Identification | Identifies fragments belonging to the same packet |
| Fragment Offset | Position of the fragment |
| More Fragments | Indicates additional fragments |
| Total Length | Fragment size |

---

## Findings

- One IP packet was divided into multiple fragments.
- All fragments shared the same Identification value.
- Wireshark successfully reassembled the original packet.

---

## Conclusion

IP fragmentation allows oversized packets to traverse networks with smaller MTU values. Excessive fragmentation can negatively impact network performance.

---

## Screenshots

- Fragmentation Filter
- Fragmented Packet
- Reassembled Packet
