### Surfing along your wireless network
- And then you're not
### And then it happens again
- And again
### You may not be able to stop it
- There's (almost) nothing you can do
### Wireless deauthentication
- A significant wireless DoS attack
# 802.11 Management Frames
### 802.11 wireless includes a number of management features
- These are frames that make everything work that aren't meant to be seen by regular users
### Important for the operation of 802.11 wireless
- How to find access points, manage QoS, associate/disassociate with an access point, etc.
### Original wireless standards didn't add protection for management frames
- They were sent in clear text with no authentication or validation
# Example Wireless Management Frame
![](attachments/Pasted%20image%2020240626155051.png)
# Protecting Against Deauth Attacks
### IEEE has already addressed this problem
- Updates included with 802.11ac
### Some of the important management frames are encrypted
- Disassociate, deauthenticate, channel switch announcements, etc.
### Not everything is encrypted
- Beacons, probes, authentication, association
# RF (Radio Frequency) Jamming
### Denial of Service
- Prevents wireless communication
### Transmit interfering wireless signals
- Decrease the signal-to-noise ratio at the receiving device
- The receiving device can't hear the good signal
### Sometimes it's not intentional
- Interference, not jamming
- Microwave oven, fluorescent lights
### Jamming is intentional
- Someone wants your network to not work
# Wireless Jamming
### Many different types
- Constant, random bits/constant, legitimate frames
- Data sent at random times - random data and legitimate frames
- Reactive jamming - only when someone else tries to communicate
### Needs to be somewhere close
- Difficult to be effective from a distance
### Time to go fox hunting
- You'll need the right equipment to hunt down the jam
- Directional antenna, attenuator