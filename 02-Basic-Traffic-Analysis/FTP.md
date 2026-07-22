# FTP Traffic Analysis

## Objective

Capture and analyze File Transfer Protocol (FTP) traffic using Wireshark to understand how FTP establishes connections and transfers data.

---

## Background

FTP (File Transfer Protocol) is an application-layer protocol used to transfer files between a client and a server. By default, FTP does not encrypt its communication, making usernames, passwords, and commands visible in network captures.

---

## Traffic Generation

An FTP session was initiated from the Windows Command Prompt to a test FTP server.

Example command:

```cmd
ftp <FTP_Server_IP_or_Hostname>
```

Example:

```cmd
ftp 192.168.1.10
```

> **Note:** A local FTP server or a lab FTP server is recommended to ensure consistent and reproducible results.

---

## Packet Capture

1. Open Wireshark.
2. Select the active network interface.
3. Start packet capture.
4. Connect to the FTP server.
5. Log in and execute basic FTP commands (e.g., `dir`, `get`, `put`, `bye`).
6. Stop the capture.
7. Save the capture as:

```
ftp.pcapng
```

---

## Display Filter

```
ftp
```

---

## Packet Analysis

The capture contains:

- FTP Control Connection
- USER Command
- PASS Command
- Server Response Codes
- Directory Listing
- File Transfer Commands

---

## Important Packet Fields

| Field | Description |
|--------|-------------|
| USER | Username sent by the client |
| PASS | Password sent by the client (plaintext) |
| Command | FTP commands issued by the client |
| Response Code | Server status response (e.g., 220, 230, 221) |

---

## Findings

- FTP commands were transmitted in plaintext.
- User authentication was visible.
- Server responses confirmed successful communication.

---

## Conclusion

FTP traffic analysis demonstrated that the protocol does not provide encryption by default. Sensitive information, including login credentials and commands, can be observed directly in captured packets.

---

## Screenshots

- FTP Display Filter
- USER/PASS Commands
- FTP Server Responses
- FTP Session Overview
