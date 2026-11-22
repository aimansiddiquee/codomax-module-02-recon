# Lab Record: Module 02

**Name:** Aimen Shahzad
**Scope:** scanme.nmap.org, testphp.vulnweb.com, my own computer

> Fill each section with my own real command output and screenshots.

## 1. Passive reconnaissance
| Command | Result summary | Screenshot |
|---|---|---|
| `nslookup scanme.nmap.org` | _(IP address found)_ | `01-nslookup.png` |
| `nslookup -type=NS nmap.org` | _(name servers)_ | `02-ns.png` |
| WHOIS lookup | _(registrar, dates)_ | `03-whois.png` |

## 2. Active reconnaissance (Nmap)
| Command | Open ports / services found | Screenshot |
|---|---|---|
| `nmap scanme.nmap.org` | _(ports)_ | `04-nmap.png` |
| `nmap -sV scanme.nmap.org` | _(versions)_ | `05-nmap-sv.png` |

## 3. Wireshark observations
_(DNS queries, ICMP, TCP SYN packets seen during the scans)_

## 4. Web tool findings (ZAP / Burp)
| Finding | Severity | Recommendation |
|---|---|---|
| _(alert name)_ | _(High/Medium/Low)_ | _(fix)_ |

## 5. Conclusion
_(What I learned, what the scans showed, how a defender would reduce the attack surface)_
