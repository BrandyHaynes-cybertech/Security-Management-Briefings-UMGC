# Security Briefing — VPN Protocols for Remote Work Security
**Course:** CMIT 425 — Cybersecurity Management | UMGC  
**Author:** Brandy Haynes  

---

## Overview

VPNs (Virtual Private Networks) became critical infrastructure during the COVID-19 pandemic as companies transitioned to remote work. This briefing covers four major VPN protocols — IKEv2, SSTP, L2TP/IPSec, and OpenVPN — and their strengths and weaknesses for securing remote corporate access.

---

## VPN Protocol Comparison

### IKEv2 — Internet Key Exchange Version 2
- Developed jointly by **Microsoft and Cisco**
- Establishes a secure connection between a VPN device and VPN server
- Tunneling protocol based on the **IPSec protocol suite**
- Offers a secure tunnel for communication between two peer devices over the internet
- **Best for:** Stable, fast connections — particularly mobile devices that switch between networks

### SSTP — Secure Socket Tunneling Protocol
- Acts as an invisible tunnel connecting server and client, encrypting all data passing through
- Uses **fixed ports** — no issues traveling through firewalls
- **Limitation:** Only works within **Microsoft operating system** environments
- **Best for:** Windows-only environments requiring strong encryption and firewall traversal

### L2TP/IPSec — Layer 2 Tunneling Protocol / Internet Protocol Security
- Can be used together or separately
- When combined, creates a significantly more secure VPN connection
- More secure than older protocols like **PPTP (Point-to-Point Tunneling)**
- **Limitation:** Results in slower speeds and can be blocked by firewalls — must pass through **UDP port 500**
- **Best for:** Anonymization rather than primary security features in high-speed environments

### OpenVPN
- One of the strongest **open-source** VPN protocols available
- Works across most major operating systems — **Windows, iOS, Linux, and Android**
- Allows employees to use a wide range of devices securely
- Uses extremely secure encryption methods
- Easily passes through firewalls
- Typically used alongside a VPN service provider
- **Best for:** Organizations with diverse device environments requiring maximum security

---

## Protocol Comparison Summary

| Protocol | OS Support | Firewall Traversal | Security Level | Best Use Case |
|----------|-----------|-------------------|----------------|---------------|
| IKEv2 | Windows, iOS, Android | Yes | High | Mobile users |
| SSTP | Windows only | Yes | High | Windows environments |
| L2TP/IPSec | Most OS | Sometimes blocked | Medium-High | Anonymization |
| OpenVPN | All major OS | Yes | Highest | Diverse device environments |

---

## Conclusion

Each VPN protocol offers different mechanisms for secure remote network access. The right choice depends on the organization's specific needs — operating system environment, device diversity, firewall configuration, and required security level. OpenVPN provides the broadest compatibility and highest security, while SSTP offers excellent security in Windows-only environments. IKEv2 is optimal for mobile users, and L2TP/IPSec serves better as an anonymization tool than a primary security feature.

---

## References

1. ExpressVPN. IKEv2 Protocol for VPN: What is IKEv2? https://www.expressvpn.com/what-is-vpn/protocols/ikev2
2. Nemchick, E. VPN Protocols Explained and Compared. Avast. https://www.avast.com/c-vpn-protocols
3. CactusVPN. What Is SSTP? Your Guide to the SSTP VPN Protocol. https://www.cactusvpn.com/beginners-guide-to-vpn/what-is-sstp/
4. Parkin, T. What Can L2TP Do for Your Network? Network World. https://www.networkworld.com/article/2163334/what-can-l2tp-do-for-your-network-.html
5. Summers, J. What is OpenVPN? How it Works & When to Use It. https://www.allthingssecured.com/vpn/faq/what-is-openvpn/
