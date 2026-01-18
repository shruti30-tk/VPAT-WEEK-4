# API Security Testing – Vulnerability Log

## Overview
This document records the vulnerabilities identified during API security testing conducted as part of LAB-2. The assessment aligns with OWASP API Top 10 risks.


## Vulnerability Testing Log

| Test ID | Vulnerability                  | Severity  | Target Endpoint |
|-------|--------------------------------|-----------|-----------------|
| 008   | Broken Object Level Authorization (BOLA) | Critical  | /api/users/{id} |
| 009   | GraphQL Injection               | High      | /graphql        |


## Test Case Details

### Test ID 008 – Broken Object Level Authorization (BOLA)

**Description:**  
The API failed to verify whether the authenticated user was authorized to access specific object IDs.

**Testing Method:**
- Intercepted API request using Burp Suite
- Modified user ID parameter in the endpoint
- Replayed the request using Burp Repeater

**Result:**  
The server returned data belonging to another user.

**Impact:**  
Attackers can access sensitive user data without authorization.


### Test ID 009 – GraphQL Injection

**Description:**  
The GraphQL API allowed unauthorized access to restricted fields due to insufficient validation.

**Testing Method:**
- Crafted GraphQL queries using Postman
- Modified query structure to request excessive fields
- Observed API responses

**Result:**  
The API exposed sensitive data beyond intended access.

**Impact:**  
Data leakage and backend schema exposure.


## Manual API Token Manipulation
- Authorization tokens were intercepted using Burp Suite
- Tokens were modified or removed
- API requests were replayed
- Unauthorized access was granted in multiple cases


## API Testing Summary (50 Words)
The API security assessment identified critical vulnerabilities such as Broken Object Level Authorization and GraphQL Injection. Inadequate authorization checks allowed unauthorized access to sensitive data. These findings highlight the importance of enforcing strict access control, validating GraphQL queries, and following OWASP API security best practices.


## Recommendations
- Implement object-level authorization checks
- Validate authentication tokens on every request
- Restrict GraphQL query depth and accessible fields
- Apply rate limiting and logging
- Follow OWASP API Security Top 10 guidelines
