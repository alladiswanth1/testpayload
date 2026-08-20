# Structured Payload Library

This directory splits payloads by vulnerability class and testing context so bug bounty / lab testing does not rely on one mixed list.

> Use only on systems you own or are explicitly authorized to test. Prefer the least-impacting probe that can confirm behavior.

## Categories

- `xss/` — reflected, DOM, attribute/context-breakout, encoding variants
- `sqli/` — generic probes plus DB-specific MySQL, PostgreSQL, MSSQL variants
- `ssrf/` — localhost/internal probes, cloud metadata references, parser/hostname bypasses, OOB detection patterns
- `ssti/` — engine-detection probes
- `path-traversal/` — traversal and encoding probes
- `command-injection/` — non-destructive timing / output probes
- `xxe/` — local-file and OOB detection patterns
- `open-redirect/` — URL parser / validation probes
- `cors/` — Origin-header test cases
- `csrf/` — request-shape / token-validation test cases

## Conventions

- One payload or test case per line where practical.
- `example.invalid` is used as a non-routable placeholder for tester-controlled hosts.
- Prefer `alert(1)`, arithmetic, short delays, and harmless local requests for detection.
- Replace placeholders only inside an authorized lab or program scope.
- Do not treat a payload firing as the full finding: verify source → sink / parser behavior, impact, and reproducibility.
