# Security Briefing — Cryptography: Symmetric vs Asymmetric Encryption
**Course:** CMIT 425 — Cybersecurity Management | UMGC  
**Author:** Brandy Haynes  

---

## Overview

Cryptography is the science and art of creating and breaking codes, used to safeguard communications from adversaries and unauthorized users. This briefing highlights symmetric key cryptography, asymmetric cryptography, and how bad actors can exploit weaknesses in each method.

---

## Symmetric Key Cryptography

### How It Works
- Uses a **single key** to both encrypt and decrypt data
- To decrypt information, the recipient must have the same key used to encrypt the original data
- Works **faster** than asymmetric cryptography

### Common Algorithm
- **AES (Advanced Encryption Standard)** — one of the most widely used symmetric encryption systems with 256-bit key length security

### Disadvantages
- Both parties must have access to the same secret key — a logistical challenge
- More useful for protecting personal information rather than shared corporate data
- With only one key, it is easier for an attacker to gain access
- If the private key is compromised, there is no failsafe

---

## Asymmetric Key Cryptography

### How It Works
- Also known as **public key encryption**
- Uses **two keys** — a public key and a private key
  - The private key stays hidden
  - The public key is available to authorized parties
- Allows message authentication with **non-repudiation** via digital signatures — the sender cannot deny sending a message
- Notifies the recipient when a message has been received or tampered with

### Common Algorithm
- **RSA (Rivest-Shamir-Adleman)** — one of the most common asymmetric encryption algorithms
  - Uses a mathematical key pair to encrypt or decrypt data
  - Can encrypt or decrypt with either the public or private key, making it harder for attackers to determine which key to target

### Disadvantages
- Slower than symmetric key encryption
- Not appropriate for bulk messages
- Public keys are generally not authenticated, making them less secure
- If the private key is compromised, the public key is already publicly accessible

---

## How Attackers Exploit Cryptography

### Key Compromise
- Gaining access to any private key results in a major data breach
- Leads to loss of customer and employee trust
- Compromised keys expose PII (Personally Identifiable Information), enabling identity theft and dark web data sales

### Key Exhaustion Attack
- Attackers use bits of data from each key generation to recreate encryption keys
- **Prevention:** Implement a Key Hierarchy to limit key reuse and exposure

---

## Comparison Summary

| Feature | Symmetric | Asymmetric |
|---------|-----------|------------|
| Number of Keys | 1 | 2 (public + private) |
| Speed | Faster | Slower |
| Best Use Case | Personal encryption | Corporate/shared encryption |
| Security Level | High if key is protected | More convenient but less secure |
| Failsafe if Key Compromised | None | None (public key is already accessible) |

---

## Conclusion

Both encryption methods provide varying levels of security. Organizations must choose based on their specific strengths, weaknesses, company preferences, and required security level. The better the security measures implemented, the less likely data breaches will occur.

---

## References

1. What is Asymmetric Key Cryptography? Thales Group. https://cpl.thalesgroup.com/faq/key-secrets-management/what-asymmetric-key-or-asymmetric-key-cryptography
2. What is a Symmetric Key? Thales Group. https://cpl.thalesgroup.com/faq/key-secrets-management/what-symmetric-key
3. What is RSA? How Does RSA Work? Encryption Consulting. https://www.encryptionconsulting.com/education-center/what-is-rsa/
4. Smirnoff, P. & Turner. Symmetric Key Encryption — Why, Where, and How It's Used in Banking. https://www.cryptomathic.com/news-events/blog/symmetric-key-encryption-why-where-and-how-its-used-in-banking
