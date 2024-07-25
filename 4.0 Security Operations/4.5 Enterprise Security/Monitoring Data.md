# FIM (File Integrity Monitoring)
### Some files change all the time
- Some files should NEVER change
### Monitor important OS and application files
- Identify when changes occur
### Windows - SFC (System File Checker)
### Linux - Tripwire
### Many host-based IPS options
# Data Loss Prevention (DLP)
### Where's your data?
- SSN, Credit Card Numbers, Medical Records
### Stop the data before the attackers get it
- Data "leakage"
### So many sources and destinations
- Often requires multiple solutions in different places
# DLP Systems
### On your computer
- Data in use
- Endpoint DLP
### On your network
- Data in motion
### On your server
- Data at rest
# USB Blocking
### DLP on a workstation
- Allow or deny certain tasks
### November 2008 - U.S. Department of Defense
- Worm virus "agent.btz" replicates using USB storage
- Bans removable flash media and storage devices
### All devices had to be updated
- Local DLP agent handled USB blocking
### Ban was lifted in February 2010
- Replaced with strict guidelines
# Cloud-Based DLP
### Located between users and the Internet
- Watch every byte of network traffic
- No hardware or software
### Block custom defined data strings
- Unique data for your organization
### Manage access to URLs
- Prevent file transfers to cloud storage
### Block viruses and malware
- Anything traversing the network
# DLP and Email
### Email continues to be the most critical risk vector
- Inbound threats, outbound data loss
### Check every email inbound and outbound
- Internal system or cloud-based
### Inbound
- Block keywords, identify imposters, quarantine email messages
### Outbound
- Fake wire transfers, W2 transmissions, employee information
# Emailing a Spreadsheet Template
### November 2016, Boeing
- Boeing employee emails spouse a spreadsheet to use as a template
### Contained the PII of 36,000 Boeing employees
- In hidden columns
- SSN, DoB, etc.
### Boeing sells its own DLP software
- But only uses it for classified work on customer networks