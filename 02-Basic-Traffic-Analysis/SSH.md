# SSH Traffic Analysis

## Objective

Capture and analyze Secure Shell (SSH) traffic using Wireshark to understand how encrypted remote connections are established.

---

## Background

SSH (Secure Shell) is an application-layer protocol that provides secure remote access to systems through encrypted communication. Unlike FTP or HTTP, SSH encrypts authentication credentials and session data.

---

## Traffic Generation

An SSH connection was initiated from the Windows Command Prompt.

Example command:

```cmd
ssh username@<SSH_Server_IP>
```

Example:

```cmd
ssh analyst@192.168.1.20
```

> **Note:** A local SSH server or lab environment is recommended.

---

## Packet Capture

1. Open Wireshark.
2. Select the active network interface.
3. Start packet capture.
4. Initiate the SSH connection.
5. Authenticate successfully.
6. Close the SSH session.
7. Stop the capture.
8. Save the file as:

```
ssh.pcapng
```

---

## Display Filter

```
ssh
```

or

```
tcp.port == 22
```

---

## Packet Analysis

The capture contains:

- TCP Three-Way Handshake
- SSH Protocol Version Exchange
- Key Exchange Initialization
- Encrypted Application Data

---

## Important Packet Fields

| Field | Description |
|--------|-------------|
| Protocol Version | SSH client and server versions |
| TCP Port | Port 22 |
| Key Exchange | Encryption negotiation |
| Encrypted Packet | Protected application data |

---

## Findings

- SSH session established successfully.
- Authentication process remained encrypted.
- Application data was not visible due to encryption.

---

## Conclusion

SSH traffic analysis demonstrated the importance of encrypted communication. Unlike insecure protocols, SSH protects authentication credentials and session data from network interception.

---

## Screenshots

- SSH Display Filter
- Protocol Version Exchange
- Key Exchange
- Encrypted Traffic
