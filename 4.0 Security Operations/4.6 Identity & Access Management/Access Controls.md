# Access Control
### Authorization
- The process of ensuring only authorized rights are exercised
- Policy enforcement
- The process of determining rights
- Policy definition
### Users receive rights based on Access Control modules
- Different business needs or mission requirements
# Least Privilege
### Rights and permissions should set to the bare minimum
- You only get exactly what's needed to complete your objective
### All user accounts must be limited
- Applications should run with minimal privileges
### Don't allow users to run with admin privileges
- Limits the scope of malicious behaviors
# Mandatory Access Control (MAC)
### The operating system limits the operation on an object
- Based on security clearance levels
### Every object gets a label
- Confidential, secret, top secret, etc.
### Labeling of objects uses predefined rules
- The administrator decides who gets access to what security level
- Users cannot change these settings
# Discretionary Access Control (DAC)
### Used in most operating systems
- A familiar access control model
### You create a spreadsheet
- As the owner, you control who has access
- You can modify access at any time
### Very flexible access control
- And very weak security
# Role-Based Access Control (RBAC)
### You have a role in your organization
- Manager, directory, team lead, project manager
### Administrators provide access based on the role of the user
- Rights are gained implicitly instead of explicitly
### In Windows, use Groups to provide role-based access control
- You are in shipping and receiving, so you can use the shipping software
- You are the manager, so you can review shipping logs
# Rule-Based Access Control
### Generic term for following rules
- Conditions other than who you are
### Access is determined through system-enforced rules
- System admins, not users
### The rule is associated with the object
- System checks the ACLs for that object
### Rule examples
- Lab network access is only available between 9AM and 5PM
- Only Chrome browsers may complete this web form
# Attribute-Based Access Control (ABAC)
### Users can have complex relationships to apps and data
- Access may be based on many different criteria
### ABAC can consider many parameters
- A "next gen" authorization model
- Aware of context
### Combine and evaluate multiple parameters
- Resource information, IP address, time of day, desired action, relationship to data, etc.
# Time-of-day Restrictions
### Almost all security devices include a time-of-day option
- Restrict access during certain times or days of the week
- Usually not the only access control
### Can be difficult to implement
- Especially in a 24-hour environment
### Time-of-day restrictions
- Training room network is inaccessible between midnight and 6AM
- Conference room access is limited after 8PM
- R&D databases are only available between 8AM and 6PM