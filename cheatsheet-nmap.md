# Nmap Cheat Sheet

| Goal | Command |
|---|---|
| Host discovery | `nmap -sn 192.168.1.0/24` |
| Default scan | `nmap target` |
| Service versions | `nmap -sV target` |
| All ports | `nmap -p- target` |
| Specific ports | `nmap -p 22,80,443 target` |
| OS detection | `sudo nmap -O target` |
| Default scripts | `nmap -sC target` |
| SYN scan (admin) | `sudo nmap -sS target` |
| UDP scan | `sudo nmap -sU target` |
| Save output | `nmap -oN result.txt target` |

**Port states:** open, closed, filtered. Scan only authorized targets.
