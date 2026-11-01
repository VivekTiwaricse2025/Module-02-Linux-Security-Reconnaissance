# Day 9 — Burp Suite and OWASP ZAP

## Aim
Understand how web-security testing proxies work and practise safely with a local training application.

## Burp Suite
Burp Suite is a web application security testing platform. Its proxy can sit between a browser and a web application so a tester can inspect requests and responses. Other features support mapping and testing web application behaviour.

## OWASP ZAP
OWASP ZAP (Zed Attack Proxy) is an open-source web application security testing tool. It can help users inspect HTTP traffic and identify potential security issues.

## Important: use a local lab
Use a deliberately vulnerable training application installed on your own computer, such as OWASP Juice Shop, or another lab explicitly provided by your instructor. Keep it bound to localhost where possible. Do not proxy, scan or attack a real website without written permission.

## Safe beginner workflow
1. Start your local practice application using its official setup instructions.
2. Confirm that it is available only at the local address/port configured by your lab.
3. Open Burp Suite or ZAP.
4. Configure a separate test browser profile to use the proxy, following the tool's official documentation.
5. Visit only your local practice application.
6. Observe a basic request and response.
7. Record the HTTP method, local path, status code and content type. Do not record passwords, cookies, tokens or personal data.
8. Stop the proxy and local lab when finished.

## Observation record
- Local training application: __________________
- Tool used: Burp Suite / OWASP ZAP
- Request method observed: __________________
- Response status code: __________________
- What is the purpose of an intercepting proxy? __________________
- Screenshot filename (redacted): __________________

## Review questions
1. What is Burp Suite?
2. What is OWASP ZAP?
3. What is an HTTP request?
4. What is an HTTP response?
5. What is the purpose of a proxy?
6. Why must web testing be limited to authorised targets?
