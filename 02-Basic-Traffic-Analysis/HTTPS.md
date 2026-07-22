# HTTPS Traffic Analysis

## Objective

Analyze encrypted HTTPS communication.

---

## Traffic Generation

Visited

```
https://www.wikipedia.org
```

---

## Display Filter

```
tls
```

or

```
tcp.port==443
```

---

## Packet Analysis

Observed

- TCP Handshake
- TLS Client Hello
- TLS Server Hello
- Encrypted Application Data

---

## Findings

Payload was encrypted.

---

## Conclusion

HTTPS protects data confidentiality through TLS encryption.

---

## Screenshots

- TLS Handshake

<img width="1919" height="1018" alt="image" src="https://github.com/user-attachments/assets/628fede6-d2ae-419b-8bbd-34d0fe1f1fe1" />

  
- Client Hello

<img width="1919" height="1014" alt="image" src="https://github.com/user-attachments/assets/61b6f6ed-528f-46b0-8c9b-fe3fe7495d4f" />

- Server Hello

<img width="1919" height="1017" alt="image" src="https://github.com/user-attachments/assets/3895e08e-9818-48fe-8d69-f42bacc91027" />
