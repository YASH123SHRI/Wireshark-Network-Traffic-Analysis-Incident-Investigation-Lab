# HTTP Credential Leak Investigation

## Objective

Analyze HTTP traffic to identify credentials transmitted in plaintext.

---

## Background

Unlike HTTPS, HTTP does not encrypt application-layer data. Usernames, passwords, cookies, and other sensitive information may be visible directly within captured packets.

This investigation demonstrates why unencrypted protocols should not be used for authentication.

---

## Data Source

Sample PCAP containing an HTTP login request.

File:

```
http-credential-leak.pcapng
```

---

## Investigation Procedure

1. Open the PCAP.
2. Apply the HTTP filter.
3. Identify HTTP POST requests.
4. Inspect packet contents.
5. Follow the TCP Stream.

---

## Display Filters

HTTP Traffic

```
http
```

HTTP POST Requests

```
http.request.method == "POST"
```

---

## Analysis

Review the following:

- Request Method
- Host
- URI
- Form Data
- Authorization Headers (if present)

---

## Indicators of Sensitive Information

- Username fields
- Password fields
- Cookies
- Session Tokens
- Authorization Headers

---

## Findings

Sensitive credentials were transmitted without encryption and were visible within the HTTP payload.

---

## Conclusion

HTTP allows sensitive information to be intercepted by anyone capable of capturing network traffic. Secure authentication should always use HTTPS.

---
