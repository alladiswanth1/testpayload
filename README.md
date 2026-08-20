# Test Payloads

Live site: https://testpayloads.linkpc.net/

The repository now also contains a structured, file-based payload reference under [`payloads/`](payloads/).

Major collections include:

- XSS: reflected, DOM, context breakout, encoded variants
- SQL injection: generic, MySQL, PostgreSQL, MSSQL
- SSRF: localhost/internal, cloud metadata, parser bypasses
- SSTI detection
- Path traversal
- Command injection detection
- XXE detection
- Open redirect
- CORS origin test cases

Use only for authorized security testing, bug bounty scope, labs, and CTFs. Prefer low-impact confirmation payloads before moving to anything more invasive.
