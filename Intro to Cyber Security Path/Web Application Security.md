### Identification and Authentication Failure

**Identification** is the ability to identify a user uniquely
**Authentication** is the ability to prove that the ser is whom they claim to be

Examples of weaknesses:
- Allowing attacker to use brute force
- Allowing weak passwords
- Storing passwords in plain text

### Broken Access Control

**Access control** ensures each user can only access files related to their role.

Example vulnerabilities:
- Failing to apply principle of least privilege
- Being able to view/modify someone else's account by using their unique ID
- Being able to browse pages requiring authentication as an unauthenticated user

### Injection

Insert malicious code as part of input. 

Improper valadation and sanitation.

### Cryptographic Failures

Cryptography focuses on the processes of encryption and decryption of data.

Encryption scrambles cleartext into ciphertext
Decryption converts the ciphertext back into the original cleartext using the secret key. 

Examples of cryptographic failures:
- Sending sensitive data in clear text (using HTTP instead of HTTPS)
- Replying on weak cryptographic algortihms
- Using default or weak keys


