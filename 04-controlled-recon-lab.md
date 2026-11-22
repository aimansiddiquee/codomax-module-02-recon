# 4. Controlled Reconnaissance Lab

A controlled lab lets me discover, analyze and document security findings **safely and legally**.

## 4.1 Rules of the lab

1. Define the **scope** (which targets are allowed) before starting.
2. Use only systems I own or that are meant for practice.
3. Keep scans gentle; avoid heavy or disruptive scans.
4. Record every command, time and result as evidence.
5. Report findings with impact and recommended fixes.

## 4.2 Lab design

- Practice targets: `scanme.nmap.org`, a local web application, or an isolated virtual machine.
- Tools: nslookup/dig/whois, Nmap, Wireshark, Burp Suite / OWASP ZAP.
- Network: isolated (host-only/NAT) when vulnerable machines are used.

## 4.3 Finding documentation template

| Field | Description |
|---|---|
| Title | Short name of the finding |
| Target | System or URL |
| Evidence | Command, output or screenshot |
| Severity | High / Medium / Low / Info |
| Impact | What an attacker could do |
| Recommendation | How to fix it |
