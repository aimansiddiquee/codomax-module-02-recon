# Lab Guide: Controlled Reconnaissance

Scope: `scanme.nmap.org` and my own computer only.

## Task 1: Passive reconnaissance (no contact with target)
```
nslookup scanme.nmap.org
nslookup -type=NS nmap.org
nslookup -type=MX nmap.org
nslookup -type=TXT nmap.org
```
Also use an online WHOIS lookup (for example whois.domaintools.com) for `nmap.org`.

## Task 2: Active reconnaissance with Nmap (gentle scans only)
```
nmap -sn scanme.nmap.org
nmap scanme.nmap.org
nmap -sV scanme.nmap.org
nmap -p 22,80,443 scanme.nmap.org
```

## Task 3: Local enumeration of my own computer
```
nmap -sV 127.0.0.1
netstat -an
```

## Task 4: Traffic analysis with Wireshark
Capture while running Task 1 and 2, then filter with `dns`, `icmp` and `tcp.flags.syn == 1`.

## Task 5: Web tool basics (OWASP ZAP or Burp Suite)
Run a **passive/automated scan only** against `testphp.vulnweb.com` (a site made for testing) and review the alerts.

## Task 6: Document
Fill `lab-record.md` with commands, results, screenshots (upload the images to this repository) and findings.
