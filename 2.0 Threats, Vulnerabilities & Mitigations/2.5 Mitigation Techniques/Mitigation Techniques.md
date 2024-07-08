# Patching
### Incredibly important
- System stability, security fixes
### Monthly updates
- Incremental (and important)
### Third-party updates
- Application developers, device drivers
### Auto-update
- Not always the best option for large organizations as it is better for the IT team to test the patches to ensure their stability before rolling them out to everyone else
### Emergency out-of-band updates
# Encryption
### Prevent access to application data files
- File system encryption
### File level encryption
- Windows EFS (Encrypted File System)
### Full disk encryption (FDE)
- Encrypt everything on the drive
- BitLocker, FileVault, etc.
### Application data encryption
- Managed by the app
- Stored data is protected
# Monitoring
###  Aggregate information from devices
- Built-in sensors, separate devices
- Integrated into servers, switches, routers, firewalls, etc.
### Sensors
- Intrusion prevention systems, firewall logs, authentication logs, web server access logs, database transaction logs, email logs
### Collectors
- Proprietary consoles (IPS, firewall), SIEM (Security Information Event Monitoring) consoles, syslog servers
- Many SIEMs include a correlation engine to compare diverse sensor data
# Least Privelege
### Rights and permissions should be set to the bare minimum
- You only get exactly what's needed to complete your objective
### All user accounts must be limited
- Applications should run with minimal privileges
### Don't allow users to run with administrative privileges
- Limits the scope of malicious behavior
# Configuration Enforcement
### Perform a posture assessment
- Each time a device connects
### Extensive check
- OS patch version
- EDR (Endpoint Detection and Response) version
- Status of firewall and EDR
- Certificate status
### Systems out of compliance are quarantined
- Private VLAN with limited access
- Recheck after making corrections
# Decommissioning
### Should be a formal policy
- Don't throw your data into the trash
- Someone will find this later
### Mostly associated with storage devices
- Hard drive
- SSD
- USB drives
### Many options for physical devices
- Recycle the drive or repurpose for another system
- Destroy the device if it contains sensitive data