# The Endpoint
### The user's access
- Applications and data
- Devices: computers, laptops, etc.
### Stop the attackers
- Inbound attacks
- Outbound attacks
### Many different platforms
- Mobile, desktop
### Protection is multi-faceted
- Defense in depth: many different security solutions for all these different platforms
# Edge vs. Access Control
### Control at the edge
- Your internet link: where the inside of the network meets the outside/internet
- Managed primarily through firewall rules
- Firewall rules rarely change
### Access Control
- Control from wherever you are
	- Inside our outside
- Access can be based on many rules
	- By user, group, location, application, etc.
- Access can be easily revoked or changed
	- Change your security posture at any time
# Posture Assessment
### You can't trust everyone's computer
- BYOD
- Malware infections/missing antivirus
- Unauthorized applications
### Before connecting to the network, perform a health check
- Is it a trusted device?
- Is it running antivirus? Which one? Is it updated?
- Are the corporate applications installed?
- Is it a mobile device? Is the disk encrypted?
- The type of device doesn't matter - Windows, macOS, Linux, iOS, Android
# Health Checks/Posture Assessment
### Persistent agents
- Permanently installed onto a system
- Periodic updates may be required
### Dissolvable agents
- No installation is required
- Runs during the posture assessment
- Terminates when no longer required
### Agentless NAC (Network Access Control)
- Integrated with AD
- Checks are made during login and logoff
- Can't be scheduled
# Failing Your Assessment
### What happens when a posture assessment fails?
- Too dangerous to allow access
### Quarantine network, notify administrators
- Just enough network access to fix the issue
### Once resolved, try again
- May require additional fixes
# Endpoint Detection and Response (EDR)
### A different method of threat protection
- Scale to meet the increasing number of threats
### Detect a threat 
- Signatures aren't the only detection tool
- Behavioral analysis, machine learning, process monitoring
- Lightweight agent on the endpoint
### Investigate the threat
- Root cause analysis
	- Able to determine why that virus got onto the system, and work backwards to find a way to remove it and prevent it from infecting any other systems
### Respond to the Threat
- Isolate the system, quarantine the threat, rollback to a previous config
- API driven, no user or technician intervention required
# Extended Detection and Response (XDR)
### An evolution of EDR
- Provides additional intelligence and a larger scope of data input to discover any malicious software
- Improve missed detections, false positives, and long investigation times
- Attacks involve more than just the endpoint
- Instead of having a single agent that only knows what's happening on a single device, XDR can interpret data from many different systems simultaneously
### Add network-based detection
- Investigate and respond to network anomalies
### Correlate endpoint, network, and cloud data
- Improve detection rates
- Simplify security event investigations
# User Behavior Analytics
### XDR commonly includes user behavior analytics
- Extend the scope of anomaly detection
### Watch users, hosts, network traffic, data repositories, etc.
- Create a baseline or normal activity
- Requires data analysis over an extended period
### Watch for anything unusual
- Use a set of rules, pattern matching, statistical analysis
### Real-time detection of unusual activity
- Catch the threat early