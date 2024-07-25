# Secure Baselines
### The security of an application environment should be well defined
- All application instances must follow this baseline
- Firewall settings, patch levels, OS file versions
- May require constant updates
### Integrity measurements check for the secure baseline
- These should be performed often
- Check against well-documented baselines
- Failure requires an immediate correction
# Establish Baselines
### Create a series of baselines
- Foundational security policies
### Security baselines are often available from the manufacturer
- Application developer
- Operating system manufacturer
- Appliance manufacturer
### Many OSes have extensive options
- There are over 3000 group policy settings in Windows 10
- Only some of those are associate with security
# Deploy Baselines
### We now have established detailed security baselines
- How do we put those baselines into action?
### Deploy the baselines
- Usually managed througha  centrally administered console
### May require multiple deployment mechanisms
- AD group policy, MDM, etc.
### Automation is the key
- Deploy to hundreds or thousands of devices
# Maintain Baselines
### Many of these are best practices
- They rarely change
### Other baselines may require ongoing updates
- A new vulnerability is discovered
- An updated application has been deployed
- A new operating system is installed
### Test and measure to avoid conflicts
- Some baselines may contradict others
- Enterprise environments are complex