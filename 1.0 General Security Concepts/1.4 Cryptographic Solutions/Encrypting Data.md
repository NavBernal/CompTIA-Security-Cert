# Encrypting Stored Data
### Protect data on storage devices
- SSD, HDD, USB drive, cloud storage, etc.
- This is data at rest
### Full-disk and Partition/Volume Encryption
- BitLocker, FileVault, etc.
### File Encryption
- EFS (Encrypting File System), third-party utilities
# Database Encryption
### Protecting Stored Data
- And the transmission of that data
### Transparent Encryption
- Encrypt all database information with a symmetric key
### Record-level Encryption
- Encrypt individual columns
- Use separate symmetric keys for each column
# Employee Table Example
### Before Encryption:
![](Pasted%20image%2020240521120814.png)
### Transparent Encryption:
![](Pasted%20image%2020240521120910.png)
### Column-Level Encryption
![](Pasted%20image%2020240521120957.png)
# Transport Encryption
### Protect data traversing the network
- You're probably doing this now
### Encrypting in the application
- Browsers can communicate using HTTPS
### VPN (Virtual Private Network)
- Encrypts all data transmitted over the network, regardless of the application
- Client-based VPN using SSL/TLS
- Site-to-site VPN using IPSec
# Encryption Algorithms
### There are many, many different ways to encrypt data
- The proper "formula" must be used during encryption and decryption
### Both sides decide on the algorithm before encrypting the data
- The details are often hidden from the end user
### There are advantages and disadvantages between algorithms
- Security level, speed, complexity of implementation, etc.
# Encryption Algorithm Comparison
![](Pasted%20image%2020240521121401.png)
# Cryptographic Keys
### There's very little that isn't known about the cryptographic process
- The algorithm is usually a known entity
- The only thing you don't know is the key
### The key determines the output
- Encrypted data
- Hash value
- Digital signature
### Keep your key private!
- It's the only thing protecting your data
# Key Lengths
### Larger keys tend to be more secure
- Prevent brute-force attacks
- Attackers can try every possible key combination
### Symmetric Encryption
- 128-bit or larger symmetric keys are common
- These numbers get larger and larger as time goes on
### Asymmetric Encryption
- Complex calculations of prime numbers
- Larger keys than symmetric encryption
- common to see key lengths of 3,072 bits or larger
# Key Stretching
### A weak key is a weak key
- By itself, it's not very secure
### Make a weak key stronger by performing multiple processes
- Hash a password, hash the hash, and continue...
- Key stretching, key strengthening
### Brute force attacks would require reversing each of those hashes
- The attacker has to spend much more time, even though the key is small