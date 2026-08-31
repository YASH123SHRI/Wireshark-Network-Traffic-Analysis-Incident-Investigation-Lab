# Wireshark Display Filters

## Objective

Demonstrate the use of Wireshark display filters to isolate and analyze specific network traffic from a packet capture.

---

## Background

Display filters are applied after packets have been captured. They allow an analyst to narrow down a large packet capture and focus on specific protocols, hosts, ports, or packet characteristics.

Unlike capture filters, display filters do not remove packets from the capture. They only control which packets are currently displayed.

---

## Lab Environment

| Component | Details |
|---|---|
| Operating System | Windows 11 |
| Packet Analyzer | Wireshark |
| Capture Format | PCAPNG |

---

## Test Capture

The filtering exercises were performed using a packet capture containing normal network traffic.

Example:

```text
conversations.pcapng
```

#screenshot

icmp
<img width="1919" height="369" alt="image" src="https://github.com/user-attachments/assets/7ee455ae-67d1-4fbb-9c51-d64a23957c24" />

dns
<img width="1919" height="609" alt="image" src="https://github.com/user-attachments/assets/0654c218-0b8f-406a-b482-b9d84e1a4603" />

tcp
<img width="1919" height="576" alt="image" src="https://github.com/user-attachments/assets/2b4715a9-5700-4d22-ae60-7a7cb9e3646c" />

udp
<img width="1919" height="610" alt="image" src="https://github.com/user-attachments/assets/1de9160a-2b04-4307-8981-3a50df1cbc38" />

combined filter
<img width="1919" height="601" alt="image" src="https://github.com/user-attachments/assets/a6a94ba5-b893-4f65-a419-a91c9e86ee55" />
