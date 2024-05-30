# Key Exchange
### A logistical challenge
- How do you share an encryption key across an insecure medium without physically transferring the key?
### Out-of-band Key Exchange
- Don't send the symmetric key over the 'net
- Telephone, courier, in-person, etc.
### In-band key exchange
- It's on the network
- Protects the key with additional encryption
- Use asymmetric encryption to deliver a symmetric key
# Real-time Encryption/Decryption
### There's a need for fast security
- Without compromising the security part
### Share a symmetric session key using asymmetric encryption
- Client encrypts a random (symmetric) key with a server's public key
- The server decrypts this shared key and uses it to encrypt data
- This is the session key
### Implement session keys carefully
- Need to be changed often (ephemeral keys)
- Need to be unpredictable
# Symmetric Key from Asymmetric Keys
### Use public and private key cryptography to create a symmetric key
- Math is powerful
![](Pasted%20image%2020240521122642.png)
