# Attacks can happen anywhere
### Two categories for IT security
- Some might say on-prem data is more secure, while others might say cloud-based is more secure
- There are pros and cons to both in regards to security
### Cloud-based security is centralized and costs less
- No dedicated hardware, no data center to secure
- A third-party handles everything
### On-premises puts the security burden on the client
- This means there are extra costs related to data center security and infrastructure
### Attackers want your data
- They don't care where it is
# On-Premises Security
## Pros:
### Customize your security posture
- Full control when everything is in-house
### On-site IT team can manage security better
- The local team can ensure everything is secure as they are likely better trained to deal with the company's specific needs compared to a third-party cloud provider
- This does, however, mean a local team can be more expensive and difficult to staff compared to a cloud provider
### Local team maintains uptime and availability
- You have complete control of all of the data and systems
- System checks can occur any time
- Any changes or modifications can be done yourself
- No need to rely on third party phone support
## Cons:
### Security changes can take time
- New equipment, configurations, and additional costs whereas a cloud provider already has all of that stuff readily available
# Centralized vs Decentralized
### Most organizations are physically decentralized
- Many locations, cloud providers, operating systems, etc.
### Difficult to manage and protect so many diverse systems
- It would instead be better to centralize the security management
### A centralized approach might look like:
- Correlated alerts
- Consolidated log file analysis
- Comprehensive system status and maintenance/patching
### It's not perfect
- This would mean there is a single point of failure that would cause your organization to lose all visibility to what's going on with your security
- As your organization grows larger, that system begins working more
- May need additional storage space to handle the increasing number of logs, as well as additional CPU power to manage the different alerts that you might receive
# Virtualization
### Virtualization
- Runs many different operating systems on the same hardware
### Each application instance has its own operating system
- This adds potential overhead and complexity
- Virtualization is also relatively expensive in order to have hardware powerful enough to run all these different operating systems at the same time without issue
### Virtualization Example Diagram
![](attachments/3cb2e51f59973034ce5a31ba5e804788.png)
- One challenge that comes with a virtualized environment is that each individual virtual machine needs to have its own operating system
- The architecture starts with the infrastructure, or the physical device that everything will run on, and then there's software that runs on top of that called the hypervisor
- The hypervisor's job is to manage all of the resources between the separate virtual machines running on that system
- Each virtual machine requires its own guest operating system
- On top of that guest operating system will be the application that you need to run in your environment
- This diagram showcases where some inefficiencies might be
- For instance, let's say that every guest operating system on the hypervisor is all running the exact same OS
- Even though it's all the same OS, you still need to run three separate instances of that OS even though they're all identical to each other
- This is where containerization comes into play
# Application Containerization
### Addresses inefficiencies of virtualization
- Containerization is a way to have multiple applications running simultaneously on a single piece of hardware
### Container
- Contains everything you need to run an application, **except for the OS**
- Code and dependencies
- A standardized unit of software
- This can be visualized in the following diagram:
![](attachments/3640cf880c0ba55d2516069d1a9a99f6.png)
### An isolated process in a sandbox
- Similar to virtualization, all of these applications are isolated from one another
- Apps are self contained and can't interact with each other
- This makes it very efficient to either remove or turn off a container and replace and add other
### Container image
- Each of these containers is referencing a single host OS that's running on this infrastructure
- Generally these apps have already been designed to run on that single host OS
- This is a standard for portability
- It's lightweight, uses the host kernel, and allows for secure separation between applications
# Virtualized vs Containerized
![](attachments/b45302191b6fe692a0cdbf6e164c2e3f.png)
- As seen in the diagram, both options start at the bottom with hardware that everything is running on AKA the infrastructure
- This changes a bit as we move up through the stack
- While a hypervisor is used on top of the infrastructure in a virtualized environment, an actual OS is used in a containerized environment
- On top of the host OS is the containerization software
- A popular option for this is Docker which is software that can then manage all of these different apps in their own separate containers
- This differs from a virtualized environment as our guest OS are running separate entities on each virtual machine
- There are of course pros and cons to both options, and it's up to the organization to find the solution that works best for their business model
# IoT (Internet of Things)
### What is it?
- Devices designed to be integrated into your network and support some of the features and services that you use on a day to day basis
### Sensors
- Heating, cooling, lighting
### Smart devices
- Home automation, video doorbells
### Wearable technology
- Watches, health monitors
### Facility automation
- Temperature, air quality, lighting
### Convenient, but usually contain weak default settings
- IoT manufacturers are not security professionals
- They may be very good at designing a thermostat or doorbell, but may not be good at implementing good security practices
- We do have to think about how we would implement IoT devices in an environment that is highly secure
- **It only takes a single IoT device to be exploited for an attacker to have full access inside of your network**
# SCADA / ICS
### Supervisory Control and Data Acquisition System
- Large-scale, multi-site **Industrial Control Systems (ICS)**
### PC manages equipment
- Power generation, refining, manufacturing equipment
- Facilities, industrial, energy, logistics
### Distributed Control systems
- Real-time information
- System control
- Everything can be handled in the control room, eliminating the need for physical access to all equipment
### Requires extensive segmentation
- No access from the outside
- Serious security issues can arise if someone was to gain access to power generation systems or oil refineries
- This could have a dramatic impact not just on immediate power needs, but could affect it for a long period of time
- This is why many SCADA systems are some of the most secure that you'll find in the world
# RTOS (Real-Time Operating System)
### An OS with a deterministic processing schedule
- No time to wait for other processes
- Industrial equipment, automobiles, military environments
- One example in vehicles is when needing to come to a complete stop, your entire system will suddenly focus on that breaking system and make sure that you're not able to skid out of control
### Extremely sensitive to security issues
- Non-trivial systems
- Need to always be available
- These systems tend to be very self-contained, and it can be difficult to know what type of security is in place
# Embedded Systems
### Hardware and software designed for a specific function
- Or to operate as part of a larger system
### Is built with only this task in mind
- Can be optimized for size and/or cost
### Common examples
- Traffic light controllers
- Digital watches
- Medical imaging systems
# High Availability
### Redundancy doesn't mean always available
- May need to be powered on and configured manually in order to become readily available
### HA (High Availability)
- Always on, always available
- There may be an HA configuration for a pair of firewalls that you've installed
- If one of those firewalls was to stop working, it would fail over to the other highly available firewall
### May include many different components working together
- Active/Active can provide scalability advantages
- In the last example with the firewalls, we had a primary firewall and we failed over to a backup that was simply waiting for that primary to fail
- Some firewalls can be configured so that both of those systems are active all the time
- If one of those firewalls was to fail, the other would continue to work normally, and all of the traffic would continue to flow without anyone knowing there was a failure
### Higher availability almost always means higher costs
- There's always another contingency you could add
- Upgraded power, high-quality server components, etc.
- Continuing with the firewall example, we needed two separate firewalls to provide that HA capability
- But if we have two separate firewalls, maybe we would also need two separate network infrastructures
- If we have that, we might also need two separate power systems
- You can continue to add on these systems and plan out for additional HA, but doing so will result in more associated costs