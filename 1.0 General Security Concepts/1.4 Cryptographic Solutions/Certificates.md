# Digital Certificates
### A public key certificate
- Binds a public key with a digital signature
- And other details about the key holder
### A digital signature adds trust
- PKI uses Certificate Authorities for additional trust
- Web of Trust adds other users for additional trust
### Certificate creation can be build into the OS
- Part of Windows Domain services
- Many 3rd-party options
# What's in a Digital Certificate
### X.509
- Standard format
### Certificate Details
- Serial number
- Version
- Signature Algorithm
- Issuer
- Name of the cert holder
- Public key
- Extensions
- And more...
![](attachments/Pasted%20image%2020240521160226.png)
# Root of Trust
### Everything associated with IT security requires trust
- A foundational characteristic
### How to build trust from something unknown?
- Someone/something trustworthy provides their approval
### Refer to the root of trust
- An inherently trusted component
- Hardware, software, firmware, or other component
- Hardware security module (HSM), Secure Enclave, Certificate Authority, etc.
# Certificate Authorities
### You connect to a random website
- Do you trust it?
### Need a good way to trust an unknown entity
- Use a trusted third-party
- An authority
### Certificate Authority (CA) has digitally signed the website certificate
- You trust the CA, therefore you trust the website
- Real-time verification
# Third-party certificate authorities
### Built-in to your browser
- Any browser
### Purchase your web site certificate
- It will be trusted by everyone's browser
### CA is responsible for vetting the request
- They will confirm the certificate owner
- Additional verification information may be required by the CA
# Certificate Signing Requests
### Create a key pair, then send the public key to the CA to be signed
- A certificate signing request (CSR)
### The CA validates the request
- Confirms DNS emails and website ownership
### CA digitally signs the cert
- Returns to the applicant
![](attachments/Pasted%20image%2020240521165317.png)
# Private Certificate Authorities
### You are your own CA
- Build it in-house
- Your devices must trust the internal CA
### Needed for medium-to-large organizations
- Many web servers and privacy requirements
### Implement as part of your overall computing strategy
- Windows Certificate Services, OpenCA
# Self-Signed Certificates
### Internal certificates don't need to be signed by a public CA
- Your company is the only one going to use it
- No need to purchase trust for devices that already trust you
### Build your own CA
- Issue your own certificates signed by your own CA
### Install the CA certificate/trusted chain on all devices
- They'll now trust any certificates signed by your internal CA
- Works exactly like a certificate you purchased