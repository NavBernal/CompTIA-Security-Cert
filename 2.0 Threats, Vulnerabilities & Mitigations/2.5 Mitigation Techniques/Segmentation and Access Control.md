# Segmenting the Network
### Physical, logical, or virtual segmentation
- Devices, VLANS, Virtual Networks
### Performance
- High-bandwidth applications
### Security
- Users shouldn't talk directly to DB servers
- The only applications in the core are SQL and SSH
### Compliance
- Mandated segmentation (PCI Compliance)
- Makes change control much easier
# Access Control Lists (ACLs)
### Allow or disallow traffic
- Groupings of categories
- Source IP, destination IP, port number, time of day, application, etc.
### Restrict access to network devices
- Limit by IP address or other identifier
- Prevent regular user/non-admin access
### Be careful when configuring these
- You can accidentally lock yourself out
# Access Control Lists
### List the permissions
- Bob can read files
- Fred can access the network
- James can access network 192.168.1.0/24 using TCP ports 80, 443, and 8088
### Many operating systems use ACLs to provide access to files
- A trustee and the access rights allowed
# Application Allow List/Deny List
### Any application can be dangerous
- Vulnerabilities, trojan horses, malware
### Security policy can control app execution
- Allow list, deny/block list
### Allow list
- Nothing runs unless it's approved
- Very restrictive
### Deny list
- Nothing on the "bad list" can be executed
- Anti-virus, anti-malware
# Examples of Allow and Deny List
### Decisions are made in the operating system
- Often built-in to the operating system management
### Application hash
- Only allows applications with this unique identifier
### Certificate
- Allow digitally signed apps from certain publishers
### Path
- Only run applications in these folders
###  Network zone
- The apps can only run from this network zone