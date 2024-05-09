# AAA Framework
### Identification
- This is who you claim to be
- Usually your username
### Authentication
- Prove you are who you say you are
- Password and other authentication factors
### Authorization
- Based on your identification and authentication, what access do you have?
### Accounting
- Resources used: Login time, data sent and received, logout time
# Authenticating People
![](attachments/Pasted%20image%2020240508220241.png)
# Authenticating Systems
### You have to manage many devices
- Often devices that you'll never physically see
### A system can't type a password
 - And you may not want to store one
### How can you truly authenticate a device?
- Put a digitally signed certificate on the device
### Other business processes rely on the certificate
- Access to the VPN from authorized devices
- Management software can validate the end device
# Certificate Authentication
### An organization has a trusted Certificate Authority (CA)
- Most orgs maintain their own CAs
### The organization creates a certificate for a device
- And digitally signs the certificate with the org's CA
### The certificate can now be included on a device as an authentication factor
- The CA's digital signature is used to validate the certificate
