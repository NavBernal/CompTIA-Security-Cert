# Content Filtering
### Control traffic based on data within the content
- URL filtering, website category filtering
### Corporate control of outbound and inbound data
- Sensitive material
### Control of inappropriate content
- NSFW
- Parental controls
### Protection against viruses/malware
# URL Scanning
### Allow or restricted based on Uniform Resource Locator
- Also called a Uniform Resource Identifier (URI)
- Allow list/block list
### Managed by category
- Auction, hacking, malware, travel, recreation, etc.
### Can have limited control
- URLs aren't the only way to surf
### Often integrated into an NGFW
- Filters traffic based on category or specific URL
# Agent Based
### Install client software on the user's device
- Usually managed from a central console
### Users can be located anywhere
- The local agent makes the filtering decisions
- Always on, always filtering
### Updates must be distributed to all agents
- Cloud based updates
- Update status shown at the console
# Proxies
- Sits between the users and the external network
- Receives the user requests and sends the request on their behalf (the proxy)
- Useful for caching information, access control, URL filtering, content scanning
- Applications may need to know how to use the proxy (explicit)
- Some proxies are invisible (transparent)
# Forward Proxy
### A centralized "internal proxy"
- Commonly used to protect and control user access to the Internet
# Block Rules
### Based on a specific URL
- x.professormesser.com: Allow
### Category of site content
- Usually divided into over 50 different topics
- Adult, Educational, Gambling, Government, Home and Garden, Legal, Malware, News, etc.
### Different dispositions
- Educational: Allow
- Home and Garden: Allow and Alert
- Gambling: Block
# Reputation
### Filter URLs based on perceived risk
- A good reputation is allowed
- A bad rep is blocked
- Risk: Trustworthy, low risk, medium risk, suspicious, high risk
### Automated reputation
- Sites are scanned and assigned a reputation
### Manual reputation
- Managers can administratively assign a rep if they don't agree with the automated result
### Add these dispositions to the URL filter
- High Risk: Block
- Trustworthy: Allow
# DNS Filtering
### Before connecting to a website, get the IP address
- Perform a DNS lookup
### DNS is updated with real-time threat intelligence
- Both commercial and public lists
### Harmful sites are not resolved
- No IP address, no connection
### This works for any DNS lookup
- Not just web filtering