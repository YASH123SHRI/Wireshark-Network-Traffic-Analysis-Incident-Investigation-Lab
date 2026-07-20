# Capture Configuration

## Objective

The objective of this section is to configure Wireshark for capturing live network traffic on a Windows 11 workstation. Proper capture configuration ensures that relevant packets are collected for protocol analysis and network investigation.

---

## Lab Environment

| Component | Details |
|-----------|----------|
| Operating System | Windows 11 |
| Packet Analyzer | Wireshark |
| Capture Interface | Wi-Fi / Ethernet (Active Interface) |
| Capture Format | PCAPNG |

---

## Selecting the Capture Interface

After launching Wireshark, all available network interfaces were displayed. The active interface showing continuous network activity was selected for packet capture.

> **Selected Interface:** Wi-Fi

Screenshot:

<img width="1536" height="326" alt="image" src="https://github.com/user-attachments/assets/3086a633-6ea0-47fd-8344-f8bcbf7d79e4" />

---

## Capture Options

The default capture settings were used.

| Setting | Value |
|----------|-------|
| Promiscuous Mode | Enabled |
| Monitor Mode | Not Applicable |
| Name Resolution | Default |
| Capture Filter | None |

No capture filters were applied so that all packets generated during the lab could be captured.

---

## Starting Packet Capture

Packet capture was started by selecting the active network interface and clicking the **Start Capturing Packets** button.

Screenshot:

`screenshots/capture-started.png`

---

## Generating Test Traffic

To verify that packet capture was working correctly, basic network traffic was generated using the Windows Command Prompt.

Command used:

```cmd
ping google.com -n 5
```

This generated ICMP Echo Request and Echo Reply packets.

---

## Saving the Capture

After the traffic was generated, packet capture was stopped and saved in PCAPNG format.

Filename:

```
lab-setup-test.pcapng
```

Location:

```
pcap-files/
```

---

## Verification

The captured packets included:

- ARP
- DNS
- ICMP
- TCP
- HTTPS

This confirmed that Wireshark was successfully capturing live network traffic.

Screenshot:

`screenshots/capture-completed.png`

---

## Learning Outcome

After completing this configuration, the packet capture environment was successfully prepared for protocol analysis and network investigation in the subsequent sections of this project.
