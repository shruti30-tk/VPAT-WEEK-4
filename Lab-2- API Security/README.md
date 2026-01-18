# LAB-2: API Security Testing Lab

## Objective
The objective of this lab is to perform API security testing aligned with the OWASP API Top 10 vulnerabilities. The lab focuses on identifying authorization flaws, injection issues, and authentication weaknesses using manual and automated tools.


## Tools Used
- Burp Suite (Community Edition)
- Postman
- sqlmap (theoretical usage)
- PortSwigger Web Security Academy (Online Lab Environment)


## Test Environment
- Platform: PortSwigger Web Security Academy
- API Type: REST & GraphQL APIs
- Authentication Mechanism: Token-based authentication
- Testing Method: Manual API testing and request manipulation


## Tasks Performed
- Enumerated exposed API endpoints
- Tested APIs for Broken Object Level Authorization (BOLA)
- Performed GraphQL injection testing
- Manipulated API authorization tokens using Burp Suite
- Documented vulnerabilities and impact


## Vulnerabilities Identified
- Broken Object Level Authorization (BOLA)
- GraphQL Injection
- Improper Authorization Handling


## Key Findings
The APIs lacked sufficient authorization checks, allowing attackers to access unauthorized resources. GraphQL endpoints exposed excessive data due to improper query validation.


## Summary
This lab demonstrated how insecure API design and missing access controls can lead to critical vulnerabilities. Proper authorization, input validation, and adherence to OWASP API security guidelines are essential to protect backend services.

