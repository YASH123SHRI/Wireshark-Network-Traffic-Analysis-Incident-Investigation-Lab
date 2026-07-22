# DNS Traffic Analysis

## Objective

Analyze Domain Name System (DNS) packets to understand how domain names are resolved into IP addresses.

---

## Background

DNS translates human-readable domain names into IP addresses, allowing systems to communicate over the Internet.

---

## Traffic Generation

DNS queries were generated using the following command:

```cmd
nslookup google.com
```

---

## Packet Capture

1. Start Wireshark.
2. Begin packet capture.
3. Execute the command above.
4. Stop capture.
5. Save as:

```
dns.pcapng
```

---

## Display Filter

```
dns
```

---

## Packet Analysis

The capture contains:

- Standard DNS Query
- Standard DNS Response
- Requested Domain
- Returned IP Address

---

## Important Packet Fields

| Field | Description |
|-------|-------------|
| Transaction ID | Matches query and response |
| Query Name | Requested domain |
| Query Type | A Record |
| Response | Returned IP |

---

## Findings

- DNS query sent successfully.
- DNS server responded with valid IPv4 address.

---

## Conclusion

DNS successfully resolved the requested domain name into an IP address.

---

## Screenshots

- DNS Filter

<img width="1919" height="597" alt="image" src="https://github.com/user-attachments/assets/24aa1e3d-3b19-4b27-801a-ddfc16130a6a" />

- DNS Query

<img width="1919" height="442" alt="image" src="https://github.com/user-attachments/assets/556e5f84-c32e-47f0-a21f-ac4be6e261e8" />

  
- DNS Response

<img width="1919" height="434" alt="image" src="https://github.com/user-attachments/assets/60e6a1a2-614d-4a5d-8cd3-8785831ad0ff" />

