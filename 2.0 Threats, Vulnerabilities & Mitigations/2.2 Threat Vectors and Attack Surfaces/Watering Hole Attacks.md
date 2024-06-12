# Watering Hole Attack
### What if your network was really secure?
- You didn't even plug in that USB key from the parking lot
### The attackers can't get in
- Not responding to phishing emails
- Not opening any email attachments
### Have the mountain come to you
- Go where the mountain hangs out
- The watering hole
- This requires a bit of research
# Executing the watering hole attack
### Determine which website the victim group uses
- Educated guess - local restaurant site that employees use often
- Industry-related sites
### Infect one of these third-party sites
- Site vulnerability
- Email attachments
### Infect all visitors
- They're only looking for specific victims
- Now you're in their network
# Example Watering Hole Attack
### Occured in January 2017
### Attackers poisoned the sites of the Polish Financial Supervision Authority, National Banking and Stock Commission of Mexico, State-owned bank in Uruguay
- The watering hole was sufficiently poisoned
### Visiting the site would download malicious JavaScript files
- But only to IP addresses matching banks and other financial institutions
### Did the attack work?
- We still don't know
# Watching the Watering Hole
### Defense-in-depth
- Layered defense
- Antivirus, Firewall, IDS, etc.
### Firewalls and IPS (Intrusion Prevention Service)
- Stop ethe network traffic before things get bad
### Anti-Virus/Anti-Malware Signature Updates
- The Polish Financial Supervision Authority attack code was recognized and stopped by generic signatures in Symantec's anti-virus software