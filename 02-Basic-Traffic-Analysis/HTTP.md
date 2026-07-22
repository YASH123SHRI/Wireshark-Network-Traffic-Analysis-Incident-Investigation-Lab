# HTTP Traffic Analysis

## Objective

Capture and analyze unencrypted HTTP traffic using Wireshark.

---

## Background

HTTP is an application-layer protocol used to transfer web content. Unlike HTTPS, HTTP transmits data in plaintext.

---

## Traffic Generation

Visited the following website:

```
http://neverssl.com
```

---

## Packet Capture

1. Start Wireshark.
2. Open browser.
3. Visit the URL above.
4. Stop capture.
5. Save as:

```
http.pcapng
```

---

## Display Filter

```
http
```

---

## Packet Analysis

Observed:

- HTTP GET Request
- HTTP 200 OK Response
- Host Header
- User-Agent

---

## Important Fields

| Field | Description |
|-------|-------------|
| Method | GET |
| Host | Requested server |
| URI | Requested page |
| Status Code | 200 OK |

---

## Findings

HTTP traffic was visible in plaintext.

---

## Conclusion

HTTP allows packet-level inspection of application-layer data because encryption is not used.

---

## Screenshots

- HTTP GET

<img width="1919" height="1018" alt="image" src="https://github.com/user-attachments/assets/623b0cd7-79cb-4bb1-85ea-037ad5371abb" />

- HTTP Response

<img width="1919" height="994" alt="image" src="https://github.com/user-attachments/assets/bf9f2062-298b-4168-9416-d6245c1e8442" />
