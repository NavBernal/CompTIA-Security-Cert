# Virtualization Security
### Quite different than non-virtual machines
- Can appear anywhere
### Quantity of resources vary between VMs
- CPU, memory, storage
### Many similarities to physical machines
- Complexity adds opportunity for the attackers
### Virtualization vulnerabilities
- Local privilege escalations
- Command injection
- Information disclosure
# VM Escape Protection
### The virtual machine is self-contained
- There's no way out
- Or is there?
### VM Escape
- Break out of the VM and interact with the host operating system or hardware
### Once you escape the VM, you have great control
- Control the host and control other guests VMs
### This would be a huge exploit
- Full control of the virtual world
# Escaping the VM
### March 2017 - Pwn2Own Competition
- Hacking contest
- You pwn it, you own it - along with some cash
### JavaScript engine bug in Microsoft Edge
- Code execution in the Edge sandbox
### Windows 10 Kernel Bug
- Compromise the guest OS
### Hardware simulation bug in VMware
- Escape to the host
### Patches were released soon afterwards
# Resource Reuse
### The hypervisor manages the relationship between physical and virtual resources
- Available RAM, storage space, CPU availability, etc.
### These resources can be reused between VMs
- Hypervisor host with 4GB of RAM
- Supports three VMs with 2GB of RAM each
- RAM is allocated and shared between VMs
### Data can be inadvertently shared between VMs
- Time to update the memory management features
- Security patches can mitigate the risk