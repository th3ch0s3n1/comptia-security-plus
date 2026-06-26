# 🌐 Section 11: Secure Protocols


> Cornell Notes — CompTIA Security+ (SY0-701) | Maps to Domain 3.0 (Security Architecture)


## ❓ Cue / Key Questions & Notes


| Question / Keyword | Answer |
| --- | --- |
| **🟢 Web & Remote Access** | TLS |
| 🔴 What is HTTPS? | Secure web traffic combining HTTP with TLS encryption over port 443. |
| 🔴 What is SSH? | Secure Shell; provides encrypted terminal access and remote command-line management over port 22. |
| **🟢 Secure File Transfer** | SFTP |
| 🔴 SFTP vs. FTPS | SFTP runs entirely inside an SSH tunnel (port 22); FTPS is standard FTP wrapped in explicit TLS encryption (ports 20/21). |
| **🟢 Identity & Directory Access** | LDAP |
| 🔴 LDAPS vs. LDAP | LDAP transmits directory data in plaintext (port 389); LDAPS encrypts directory traffic using TLS over port 636. |
| 🔴 What is 802.1X? | An IEEE standard providing port-based network access control to authenticate devices before granting LAN/WLAN entry. |
| **🟢 Management & Infrastructure** | SNMP |
| 🔴 What is DNSSEC? | Domain Name System Security Extensions; adds cryptographic signatures to DNS records to prevent spoofing and cache poisoning. |
| 🔴 What is SNMPv3? | The secure version of Simple Network Management Protocol, adding authentication and encryption for network monitoring. |
| 🔴 What is NTP? | Network Time Protocol; synchronizes clocks across network devices, which is critical for accurate log auditing. |
| **🟢 Media & Messaging** | SRTP |
| 🔴 What is SRTP? | Secure Real-time Transport Protocol; provides encryption, message authentication, and replay protection for voice/video (VoIP) traffic. |
| 🔴 What are IMAPS and POPS? | Cryptographically secure email retrieval protocols wrapped in TLS (IMAPS: port 993, POPS: port 995). |
| **🟢 Insecure & Deprecated Protocols** |  |
| 🔴 Which protocols should be avoided entirely? | HTTP, Telnet, FTP, LDAP, and SNMPv1/v2, because they transmit sensitive credentials and data in clear plaintext. |


## 📝 Summary


Securing network communications requires replacing legacy, plaintext data streams with **secure protocols** wrapped in cryptographic encryption. Enterprise web environments deploy **HTTPS** alongside administrative infrastructure managed via **SSH** and **SNMPv3**. Data transfers leverage encrypted baselines via **SFTP** or **FTPS** to block packet interception, while directory lookups are hardened using **LDAPS**. Network layer services depend on **DNSSEC** to maintain domain name integrity, **NTP** to guarantee synchronized clock metrics across audit trails, and **802.1X** to enforce port-level access controls. Ultimately, modern security architectures mandate the strict deprecation of legacy legacy protocols—such as Telnet, FTP, and basic HTTP—to eliminate the threat of plaintext sniffing and credential hijacking.
