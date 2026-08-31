# Wireshark Capture Filters

## Objective

Demonstrate the use of Wireshark capture filters to limit which packets are captured during a live network capture.

---

## Background

Capture filters are applied before or during packet capture. They determine which packets Wireshark records.

Unlike display filters, packets that do not match a capture filter are not captured.

Capture filters use the Berkeley Packet Filter (BPF) syntax.

---

## Display Filter vs Capture Filter

| Feature | Display Filter | Capture Filter |
|---|---|---|
| Applied | After capture | Before/during capture |
| Purpose | Analyze captured packets | Limit captured packets |
| Syntax | Wireshark display filter syntax | BPF syntax |
| Example | `tcp.port == 443` | `port 443` |

---

## Capture Filters Tested

Capture DNS traffic:
port 53

Capture HTTP traffic:
tcp port 80

Capture HTTPS traffic:
tcp port 443
