# Hardening Targets
### Most systems aren't secure with the default configurations
- You need some guidelines to keep everything safe
### Hardening guides are specific to the software or platform
- Get feedback from the manufacturer or Internet interest group
- They'll have the best details
### Other general-purpose guides are available online
# Mobile Devices
### Always-connected mobile technologies
- Phones, tablets, etc.
- Hardening checklists are usually available from manufacturers
### Updates are critical
- Bug fixes and security patches
- Prevent any known vulnerabilities
### Segmentation can protect data
- Company and user data are separated
### Control with an MDM
- Mobile Device Manager
- Best option when many company mobile devices are in use
# Workstations
### User desktops and laptops
- Windows, macOS, Linux, etc.
### Constant monitoring and updates
- Operating systems, applications, firmware, etc.
### Automate the monthly patches
- There's likely an existing process
### Connect to a policy management system
- AD group policy
### Remove unnecessary software
- Limit the threats
# Network Infrastructure Devices
### Switches, routers, etc.
- You never see them, but they're always there
### Purpose-built devices
- Embedded OS, limited OS access
### Configure authentication
- Don't use the defaults
### Check with the manufacturer
- Security updates
- Not usually updated frequently
- Updates are usually important and should be applied immediately
# Cloud Infrastructure
### Secure the cloud management workstation
- The keys to the kingdom
### Least privilege
- All services, network settings, applications rights and permissions
### Configure EDR (Endpoint Detection and Response)
- All devices accessing the cloud should be secure
### Always have backups
- Cloud to Cloud (C2C)
# Servers
### Many and varied
- Windows, Linux, etc.
### Updates
- OS updates/service packs, security patches
### User accounts
- Minimum password lengths and complexity
- Account limitations
### Network access and security
- Limit network access
### Monitor and secure
- EDR, anti-virus, anti-malware
# SCADA/ICS
### Supervisory Control and Data Acquisition System
- Large-scale, multi-site **Industrial Control Systems (ICS)**
### PC manages equipment
- Power generations, refining, manufacturing equipment
- Facilities, industrial, energy, logistics
### Distributed control systems
- Real-time information
- System control
### Requires extensive segmentation
- No access from the outside
- We don't want anyone online having access to these systems
# Embedded Systems
### Hardware and software designed for a specific function
- Or to operate as part of a larger system
### Can be difficult to upgrade
- Watches and televisions are relatively easy
- Other devices may not be easily modified
### Correct vulnerabilities
- Security patches remove potential threats
### Segment and firewall
- Prevent access from unauthorized users
# RTOS (Real-Time Operating System)
### An operating system with a deterministic processing schedule
- No time to wait for other processes
- Industrial equipment, automobiles, military environments
### Isolate the system
- Prevent access from other areas
### Run with the minimum services
- Prevent the potential for exploit
### Use secure communications
- Protect with a host-based firewall
# IoT Devices
### Heating and cooling, lighting, home automation, wearable tech, etc.
### Weak defaults
- IoT manufacturers are not security professionals
- Change those passwords
### Deploy updates quickly
- Can be a significant security concern
### Segmentation
- Put IoT devices on their own VLAN (Virtual Local Area Network)