# Availability
### System Uptime
- Access data, complete transactions
- A foundation of IT security
### A balancing act with security
- Available, but only to the right people
### We spend a lot of time and money on availability
- Monitoring, redundant systems
### An important metric
- We are often evaluated on total available time
- Companies' will have bragging rights for having "99.9% uptime in the past 6 months" as that showcases they've been doing a good job (so far) at ensuring their services are always available
# Resilience
### Eventually, something will happen
- Can you maintain availibility?
- Can you recover?
- How quickly?
### Based on many different variables
- The root cause of the issue
- Replacement hardware installation
- Software patch availability
- Redundant systems
### Commonly referenced as MTTR (Mean Time to Repair)
- This describes the length of time it takes to replace something that is no longer available with components that are
# Cost
###  How much money is required?
- Everything ultimately comes down to cost
### Initial installation
- Very different across platforms
### Ongoing maintenance
- Annual ongoing cost
- This may either fall on the manufacturer or be an internal cost
### Replacement or repair costs
- You might need more than one
### Tax implications
- Operating or capital expense
# Responsiveness
### Request information
- Get a response
- How quickly did we receive that response?
### This is especially important for interactive applications
- Humans are very sensitive delays and a sluggish program/service could cause them to never use it again
### Speed is an important metric
- Challenging to quantify due to multiple steps being required
- Responsiveness may vary widely depending on what's happening with that application
- We tend to look at the overall functions of an app
- Some of those may occur very quickly and seem snappy, whereas others require additional steps and come across as slow
- All parts of the application contribute to this metric
# Scalability
### How quickly and easily can we increase or decrease capacity?
- This might happen many times a day
- We refer to this process as **elasticity**
### What's preventing an org's scalability?
- There's always a resource challenge associated with this
- It costs money to have large scalability
- One way that org's deal with that is to build out an app instance that matches the current load for that app
- As more people need to use it, we might extend or scale this app to be much larger
- This can sometimes be done automatically behind the scenes and the end user has no idea that you're increasing scalability as the load increases
### Needs to include security monitoring
- From a security perspective, we need to ensure that we're monitoring the entire application regardless of how it might scale
- We might have security tools that are able to monitor the base configuration, but this needs to be extended as we increase scalability
# Ease of Deployment
### An application has many moving parts
- Web server, database, catching server, firewalls, etc.
### This might be an involved process
- Hardware resources, cloud budgets, change control
### This might be very simple
- **Orchestration/automation**: A description of building out a  cloud based infrastructure automatically on demand
- This is one of the significant advantages of a cloud based infrastructure, you can very easily and programmatically build out an entire application instance in a moment's notice
### Important to consider during the project management phase
- One missed detail can cause deployment issues
# Risk transference
### Many methods to minimize risk
- Transfer the risk to a third-party
### Cybersecurity insurance
- Attacks and downtime can be recovered
- Popular with the rise in ransomware as it becomes possible to recoup at least some internal costs from the attack
### Recover Internal Losses
- Outages and business downtime
### Protect against legal issues from customers
- The insurance may be able to limit the costs associated with legal proceedings
# Ease of Recovery
### Something will eventually go wrong
- Time is money
- How easily can you recover?
### Malware Infection
- Reload operating system from original media - 1 hour
- Reload from corporate image - 10 minutes
- Both options result in a similar solution, but one takes much less time and thus will cost the organization less money from downtime
### This is another important design criteria
- If you're planning on implementing a new application or a new service in your organization, you might also think about what it will take to get this system back up and running if it runs into a problem
- This may be critical to the final product
# Patch Availability
### Software isn't usually static
- Bug fixes, security updates, etc.
### This is often the first task after installation
- Make sure you're running the latest version
### Most companies have regular updates
- Microsoft's monthly patch schedule
### Some companies rarely patch
- This might be a significant concern
# Inability to Patch
### What if patching wasn't an option?
- This happens more often than you might think
### Embedded systems
- HVAC controls
- Time clocks
- Hotel key fob handles
### These are not designed for end-user updates
- This is a bit short sighted these days as there is a much larger threat landscape in the modern tech world
### These devices may need additional security controls
- A firewall for your HVAC systems may sound crazy, but it's better to be safe than sorry
# Power
### A foundational element
- Must have electricity to be able to run all of these systems, whether it's something on premises or in the cloud
- This can require extensive engineering
- Sometimes overlooked, but it is one of the most important components of everything we do in tech
# Overall power requirements can differ
- A data center would have much different power needs vs an office building
- Always a good idea to bring in a licensed electrician who would know just how much power is needed to keep everything running
### Primary Power
- Most orgs have a single provider
- If living in a largely populated area, there may be many
### Backup services
- UPS (Uninterruptible Power Supply)
- Generators
# Compute
### An application's heavy lifting
- More than just a single CPU
### In the cloud, this is referred to as the Compute Engine
- Does the actual thinking and processing of the data
### May be limited to a single processor
- Easier to develop
### Use multiple CPUs across multiple clouds
- Additional complexity
- Enhanced scalability