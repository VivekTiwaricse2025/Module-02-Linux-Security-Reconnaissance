# Day 7 — Reconnaissance Fundamentals

## Aim
Understand information gathering and distinguish passive reconnaissance from active reconnaissance.

## Key concepts
**Reconnaissance** is the information-gathering phase of a security assessment.

- **Passive reconnaissance:** Collects information from publicly available sources without directly interacting with the target's systems. Examples include reviewing an organisation's public website, public documentation and public DNS records.
- **Active reconnaissance:** Sends requests or probes to a target system, such as checking a service on an authorised host. It is more likely to be logged and requires permission.

## DNS basics
DNS (Domain Name System) translates domain names into IP addresses. Common record types:
- `A`: IPv4 address
- `AAAA`: IPv6 address
- `MX`: mail server
- `NS`: authoritative name server
- `TXT`: text data, often used for domain verification and email-security policies
- `CNAME`: alias to another domain name

## Safe practice
For a simple DNS lookup of a public example domain:
```bash
nslookup example.com
```
You may also use:
```bash
dig example.com
```
These commands request DNS information; do not use them to enumerate private or sensitive domains without permission.

## Practical worksheet
1. Write the domain used for the lookup: __________________
2. Record the DNS tool used: __________________
3. Record the returned address/record type, if shown: __________________
4. Explain in your own words what DNS does: __________________
5. Was the activity passive or active? Explain: __________________

## Compare
| Passive reconnaissance | Active reconnaissance |
|---|---|
| Uses public/third-party information sources | Directly interacts with target systems |
| Usually lower visibility to the target | May be logged or trigger alerts |
| Still must respect privacy and laws | Requires explicit authorisation |

## Review questions
1. Define reconnaissance.
2. Differentiate passive and active reconnaissance.
3. What is DNS?
4. Explain A, AAAA, MX and NS records.
5. Why is written permission important before active reconnaissance?
