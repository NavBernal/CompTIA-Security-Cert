# Security in the Cloud
### Cloud adoption has been nearly universal
- It's difficult to find a company NOT using the cloud
### We've put sensitive data in the cloud
- The attackers would like this data
### We're not putting in the right protections
- 76% of organizations aren't using MFA for management console users
### Simple best-practices aren't being used
- 63% of code in production is unpatched
- Vulnerabilities rated high or critical (CVSS >= 7.0)
# Attack the Service
### Denial of Service (DoS)
- Can put a complete halt to business operations
- A fundamental attack type
### Authentication Bypass
- Take advantage of weak or faulty authentication (lack of MFA)
### Directory Traversal
- Fault configurations put data at risk
### Remote Code Execution
- Take advantage of unpatched systems
# Attack the Application
### Web application attacks have increased
- Log4j and Spring Cloud Function
- Easy to exploit, rewards are extensive
### Cross-Site Scripting (XSS)
- Take advantage of poor input validation
### Out of bounds write
- Write to unauthorized memory areas
- Data corruption, crashing, or code execution
### SQL Injection
- Get direct access to a database