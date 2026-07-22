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
icmp
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
