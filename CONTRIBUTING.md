
```markdown
# CONTRIBUTING


Thanks for contributing. Keep this repo professional, reproducible, and safe.


## Branch & commit conventions
- Use feature branches: `lab/01-web-app-pentest`.
- Commit messages should follow a clear convention. Example:
- `lab(01-web-app-pentest): add poc for sqli and initial writeup`
- `docs(readme): update lab checklist`


## Pull Requests
- Open a PR when a lab is complete or when you want peer feedback.
- PR description must include: summary, steps to reproduce, and checklist:
- [ ] Environment files included (`docker-compose.yml`, `Vagrantfile`, `repro.sh`)
- [ ] Writeup complete using template
- [ ] Sensitive data sanitized
- [ ] Tests or verification steps


## Security & sanitization
- **NEVER** commit private keys, credentials, or unapproved malware. Use placeholders like `<REDACTED_KEY>`.
- PCAPs may contain sensitive data; sanitize or only include short, safe excerpts.
- If a lab requires a malware sample, provide a script to fetch a benign sample for analysis rather than storing it in the repo.


## Lab quality requirements
Each lab must include:
- Objective, environment, threat model
- Step-by-step procedures with commands and reasoning
- Proof of exploit/analysis (sanitized) and mitigations
- Detection guidance (SIEM queries / rules)


## Style
- Markdown format, use fenced code blocks for commands
- Keep TL;DR at the top of each lab README (1–3 sentences)
---


## labs/01-web-app-pentest/README.md (detailed template)


```markdown
# Lab 01 — Web App Pentest (OWASP basics)


**TL;DR:** Exploit SQL Injection and stored XSS in OWASP Juice Shop (Docker). Demonstrate exploitation, parameterized fix, and create a WAF rule sample.


## Objective
- Practice OWASP Top 10 vulnerabilities (SQLi, XSS). Show exploit → patch → detection.


## Environment (Repro)
- Docker + Docker Compose
- juice-shop (latest via Docker)


**Files included:** `docker-compose.yml`, `repro.sh` (commands to start lab)


## Threat Model / Assumptions
- Attacker has network access to app only; no privileged access to host.


## Tools used
- nmap, sqlmap, Burp Suite (community), curl, sqlite3


## Step-by-step Attack
1. Start environment:
```bash
cd labs/01-web-app-pentest
./repro.sh
# opens: http://localhost:3000
Recon (nmap/curl)

Identify injectable parameter (demo payload)

Use sqlmap to extract user table (commands, options)

Demonstrate stored XSS using the product review form

(........)

Proof of Exploit

Show sanitized DB dump of non-sensitive columns

Show screenshot of XSS pop-up (sanitized)

Mitigation & Hardening

Parameterized queries example (Node/Express) and patched code snippet

Input validation examples and CSP header sample

Example ModSecurity rule to detect SQLi patterns

Detection

Example ELK query to detect unusual DB dump patterns / large response sizes

Sample SIEM rule for repeated suspicious POST requests

IOCs

Example payload strings, dummy IPs, and logged events (sanitized)

Lessons Learned & Next Steps

Test additional auth bypasses and session fixation vulnerabilities

References

OWASP Juice Shop

PortSwigger labs


