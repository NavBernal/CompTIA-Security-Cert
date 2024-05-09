y## Exam Objective 1.2
## Zero Trust
### Planes of Operation
- Many networks are open on the inside
	- Once you're through the firewall, there are few security controls
- Zero trust is a holistic approach to network security
	- Covers every device
- Everything must be verified
### Controlling Trust
### Policy Enforcement Point
### Security Zones
- Where are you coming from and where are you going?
	- Trusted/untrusted
	- Internal/external network
![](attachments/Pasted%20image%2020240416193058.png)
### Deception & Disruption
![](attachments/Pasted%20image%2020240416193347.png)
#### Honeypots
- Attract the bad guys and trap them there
- The attacker is probably a machine
- Honeypots create a virtual world to explore
- Many different options
	- Most are open source and available to download
- Constant battle to discern the real from the fake
#### Honeynets
- A real network includes more than a single device
	- Servers, workstations, routers, switches, firewalls
- Built a larger deception network with one or more honeypots
- More than one source of information
#### Honeyfiles
- Attract the attackers with more honey
	- Creates files with fake info
	- Something bright and shiny
- Bait for the honeynet (passwords.txt)
- Add many honeyfiles to file shares
- An alert is sent if the file is accessed
	- A virtual bear trap
#### Honeytokens
- Track the malicious actors
	- Add some traceable data to the honeynet
	- If the data is stolen, you'll know where it came from
- API creds
	- Doesn't actually provide access
	- Notifications are sent when used
- Fake email addresses
	- Add it to a contact list
	- Monitor the internet to see who posts it
- Many other examples
	- Database records
### Gap Analysis
- Refers to the process of identifying discrepancies or "gaps" between an org's current security posture and its desired or required posture
- Where you are compared with where you want to be
	- The "gap" between the two
- This may require extensive research
	- There's a lot to consider
- This can take weeks or months
	- An extensive study with numerous participants
	- Get ready for emails, data gathering, and technical research
#### Choosing the Framework
- Work
## 1.3 - The importance of change management processes and the impact to security
- Business processes impacting security operation
- Technical implications
- Documentation
- Version control
- Example:
	- Target Data Breach
		- In 2013, Target experiences a massive data breach that exposed the personal and financial information of over 110 million customers
		- The breach occurred due to a failure in the company's change management process
#### Change Management
- How to make a change
	- Upgrade software, patch an application, change firewall configuration, modify switch ports
- One of the most common risks in the enterprise
	- Occurs very frequently
- Often overlooked or ignored
- Have clear policies
	- Frequency, duration, installation process, rollback procedures
- Sometimes extremely difficult to implement
	- It's hard to change corporate culture
#### Change Approval Process
- A formal process for managing change
	- Avoid downtime, confusion, and mistakes
- A typical approval process
	- Complete the requests forms
	- Determine the purpose of the change
	- Identify the scope of the change
	- Schedule a data and time of the change
	- Determine affected systems and the impact
#### Impact Analysis
- Determine a risk value
	- i.e. high, medium, low
	- 