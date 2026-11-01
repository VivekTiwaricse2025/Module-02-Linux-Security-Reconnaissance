# Day 8 — Nmap and Wireshark Basics

## Aim
Learn what network scanning and packet analysis do, then practise only against the local computer or an explicitly authorised lab.

## Nmap
Nmap is a network discovery and security auditing tool. It can identify hosts, open ports and service information. A port is a numbered communication endpoint used by network services.

### Safe local exercise
On your own computer:
```bash
nmap 127.0.0.1
```
Optional service identification on the same local machine:
```bash
nmap -sV 127.0.0.1
```
`127.0.0.1` is the IPv4 loopback address, which refers to your own computer. Do not replace it with a public or third-party address unless you have explicit authorisation.

## Wireshark
Wireshark is a packet analyser. It captures and displays network packets to help users understand protocols and troubleshoot networks.

### Safe practice
1. Open Wireshark.
2. Select an interface belonging to your own computer.
3. Start a short capture while generating ordinary traffic, such as opening a local page or performing a permitted DNS lookup.
4. Stop the capture.
5. Inspect packet details and identify protocol names.
6. Save a small sample only if it contains no credentials or personal information; otherwise use a screenshot with sensitive data hidden.

Useful display filters:
- `dns` — DNS packets
- `tcp` — TCP packets
- `udp` — UDP packets
- `http` — HTTP packets, where present

## Observation record
- Device / lab used: __________________
- Nmap command: __________________
- Ports reported on localhost: __________________
- Wireshark interface: __________________
- Protocols observed: __________________
- What did you learn from the capture? __________________

## Review questions
1. What is Nmap used for?
2. What is a port?
3. What does `127.0.0.1` represent?
4. What is packet analysis?
5. Differentiate TCP and UDP at a basic level.
6. Why should captures be checked for sensitive information before sharing?
