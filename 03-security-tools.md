# 3. Essential Security Tools

| Tool | Type | Main use |
|---|---|---|
| **Nmap** | Network scanner | Discover hosts, open ports, services and versions |
| **Wireshark** | Packet analyzer | Capture and inspect network traffic |
| **Burp Suite** | Web proxy | Intercept and modify web requests, test web apps |
| **OWASP ZAP** | Web scanner | Free tool to find web application vulnerabilities |

## 3.1 Nmap

```
nmap -sn 192.168.1.0/24        # host discovery
nmap target                     # top 1000 ports
nmap -sV target                 # service versions
nmap -p 1-1000 target           # port range
nmap -sC -sV target             # default scripts + versions
nmap -O target                  # OS detection (admin rights)
nmap -oN result.txt target      # save output
```
Port states: **open** (service listening), **closed** (reachable, nothing listening), **filtered** (blocked by firewall).

## 3.2 Wireshark

- Capture on an interface, then use display filters: `icmp`, `dns`, `http`, `tcp.port == 443`, `ip.addr == x.x.x.x`.
- Shows protocol, source, destination and packet details; helps to see the TCP handshake and plain-text traffic.

## 3.3 Burp Suite

- Works as an **intercepting proxy** between browser and website (default `127.0.0.1:8080`).
- **Proxy:** intercept and edit requests. **Repeater:** resend requests manually. **Intruder:** automated payload testing. **Decoder / Comparer:** helper tools.
- Use only on applications you are authorized to test.

## 3.4 OWASP ZAP

- Free, open-source scanner from OWASP.
- **Spider** finds pages, **passive scan** checks traffic safely, **active scan** sends attack-like requests.
- Alerts are rated High, Medium, Low and Informational, with an explanation and recommended fix.

## 3.5 Legal practice targets

`scanme.nmap.org` (light Nmap scans allowed), OWASP Juice Shop, DVWA, `testphp.vulnweb.com`, and your own machines or virtual labs.
