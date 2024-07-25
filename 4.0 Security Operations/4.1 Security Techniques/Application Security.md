# Secure Coding Concepts
### A balance between time and quality
- Programming with security in mind is often secondary
### Testing, testing, testing
- The QA process
### Vulnerabilities will eventually be found
- And exploited
# Input Validation
### What is the expected input?
- Validate actual vs expected
### Document all input methods
- Forms, fields, type
### Check and correct all input (normalization)
- A zip code should only be X amount of characters with a letter in the X column
- Fix any data with improper input
### The fuzzers will find what you missed
- Fuzzing is an automated process for providing different types of input for these applications
- Fuzzers will put random types of data into the input fields to see what the application might do
- If the app performs unexpectedly, the dev may need to go back and change the way that they're handling input validation
# Secure Cookies
### Cookies
- Information stored on your computer by the browser
### Used for tracking, personalization, session management
- Not executable, not generally a security risk
	- Unless someone gets access to them
### Secure cookies have a Secure attribute set
- Browser will only send it over HTTPS
### Sensitive information should not be saved in a cookie
- This isn't designed to be secure storage
# Static Code Analyzers
### Static Application Security Testing (SAST)
- Help to identify security flaws
### Many security vulnerabilities found easily
- Buffer overflows, database injections, etc.
### Not everything can be identified through analysis
- Authentication security, insecure cryptography, etc.
- Don't rely on automation for everything
### Still have to verify each finding
- False positives can occur
# Code Signing
### An application is deployed
- Users run application executable or scripts
### So many security questions
- Has the application been modified in any way?
- Can you confirm that the application was written by a specific developer?
### The application code can be digitally signed by the developer
- Asymmetric encryption
- A trusted CA (certificate authority) signs the developer's public key
- Developer signs the code with their private key
- For internal apps, user your own CA
# Sandboxing
### Applications cannot access unrelated resources
- They play in their own sandbox
### Commonly used during development
- Can be a useful production technique
### Used in many different deployments
- Virtual machines
- Mobile devices
- Browser iframes (Inline Frames)
- Windows User Account Control (UAC)
# Application Security Monitoring
### Real-time information
- Application usage, access demographics
### View blocked attacks
- SQL Injection attempts, patched vulnerabilities
### Audit the logs
- Find the information gathering and hidden attacks
### Anomaly detection
- Unusual file transfers
- Increase in client access