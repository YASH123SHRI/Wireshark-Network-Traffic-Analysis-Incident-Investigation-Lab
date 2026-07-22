# ICMP Traffic Analysis

## Objective

Analyze Internet Control Message Protocol (ICMP) packets captured using Wireshark and understand how ICMP is used to verify network connectivity.

---

## Background

ICMP (Internet Control Message Protocol) is a network layer protocol used for diagnostic and error-reporting purposes. The most common use of ICMP is the **ping** command, which sends Echo Request packets and receives Echo Reply packets.

---

## Traffic Generation

ICMP traffic was generated using the Windows Command Prompt.

Command:

```cmd
ping google.com -n 5
```

---

## Packet Capture

1. Open Wireshark.
2. Select the active network interface.
3. Start packet capture.
4. Execute the ping command.
5. Stop packet capture.
6. Save the capture as:

```
icmp.pcapng
```

---

## Display Filter

```
icmpv6
```

---

## Packet Analysis

The capture shows:

- ICMP Echo Request packets sent from the local machine.
- ICMP Echo Reply packets received from the destination.
- Matching Identifier and Sequence Number values.
- Successful communication with no packet loss.

---

## Important Packet Fields

| Field | Description |
|--------|-------------|
| Type | Echo Request (8) / Echo Reply (0) |
| Code | 0 |
| Identifier | Matches request and reply |
| Sequence Number | Tracks packet order |
| Checksum | Validates packet integrity |

---

## Findings

- Five Echo Request packets were transmitted.
- Five Echo Reply packets were received.
- Network connectivity was successfully verified.

---

## Conclusion

ICMP packet analysis demonstrated successful communication between the local workstation and the destination host. Wireshark accurately captured and decoded all ICMP packets.

---

## Screenshots

- Packet Capture
- ICMP Display Filter
- Packet Details Pane

## FILTER
<img width="1919" height="1014" alt="image" src="https://github.com/user-attachments/assets/36cffe96-7454-46d3-a94a-85ccfe1e33d4" />
## REQUEST
<img width="1919" height="443" alt="image" src="https://github.com/user-attachments/assets/45353d7d-a8ba-410d-a584-bff9d9eb2357" />
## REPLY
<img width="1919" height="762" alt="image" src="https://github.com/user-attachments/assets/8bb6fd92-9036-47cc-a739-7b45ed59ab08" />
