# Email Security Challenges
### The protocols used to transfer emails include relatively few security checks
- It's very easy to spoof an email
### Spoofing happens all the time
- Check your spam folder
### The email looks as if it originated from james@professormesser.com
- But did it? How can you tell?
### A reputable sender will configure email validation
- Publicly available on the sender's DNS server
# Mail Gateway
### The gatekeeper
- Evaluates the source of inbound email messages
- Blocks it at the gateway before it reaches the user
- On-site or cloud-based
![](attachments/cbc8521987af1289514de42c873de8d0.png)
# Sender Policy Framework (SPF)
### SPF Protocol
- Sender configures a list of all servers authorized to send emails for a domain
### List of authorized mail servers are added to a DNS TXT record
- Receiving mail servers perform a check to see if incoming mail really did come from an authorized host
![](attachments/6f11e58a74a5e6eeacd9bf64bbf086db.png)
# Adding an SPF TXT Record
![](attachments/e68c5336f5fd53e7ddb73085903d9334.png)
# Domain Key Identified Mail (DKIM)
### A mail server digitally signs all outgoing mail
- The public key is in the DKIM TXT record
### The signatures is validated by the receiving mail servers
- Not usually seen by the end user
![](attachments/26b0e7b127836d7ed736922fb45fc083.png)
# Adding a DKIM TXT Record
![](attachments/6655be541c80368f61434e41772c74d2.png)
# DMARC
### Domain-Based Message Authentication, Reporting, and Conformance
- An extension of SPF and DKIM
### The domain owner decided what receiving email servers should do with emails not validating using SPF and DKIM
- That policy is written into a DNS TXT record
- Accept all, send to spam, or reject the email
### Compliance reports are sent to the email admin
- The domain owner can see how many emails are received
# Adding a DMARC TXT Record
![](attachments/48f02463607ec8bf720a3cf4e66ad2e3.png)
# DMARC Reports
![](attachments/e9e3ab361d758a8c141fcf3d23daa3f6.png)