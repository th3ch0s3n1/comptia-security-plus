# Section 2: Fundamentals of Security


> Cornell Notes — CompTIA Security+ (SY0-701) | Maps to Domain 1.0 (General Security Concepts)


## Cue / Key Questions & Notes

| Question / Keyword | Answer |
| ------------------ | ------ |
| **🟢 InfoSec** |  |
| 🔴 What is information security? | Protecting data and systems from unauthorized access, disclosure, alteration, or destruction. |
| 🔴 What is information systems security? | Protecting the hardware, software, and networks that process data. |
| **🟢 CIA Triad** | CIA |
| 🔴 What is the CIA Triad? | **Confidentiality**, **Integrity**, **Availability** — the three pillars of security. |
| 🔴 What is Confidentiality? | Only authorized people can access information (encryption, access controls, MFA). |
| 🔴 What is Integrity? | Data remains accurate and unaltered. |
| 🔴 What tools guarantee Integrity? | Hashing, checksums, and digital signatures. |
| 🔴 What is Availability? | Information/systems are accessible when needed (redundancy, backups, failover). |
| **🟢 Integrity Tools** |  |
| 🔴 What is hashing? | Function converting any size input into a fixed-length hex string. Collisions can occur! |
| 🔴 What is a checksum? | A calculated value used to verify file integrity and detect accidental errors. |
| 🔴 What is a digital signature? | A private-key encrypted hash proving sender identity and data integrity. |
| 🔴 What is Non-repudiation? | Assurance that a party cannot deny an action (provided by digital signatures). |
| **🟢 AAA Framework** | AAA |
| 🔴 What is the AAA of security? | **Authentication**, **Authorization**, **Accounting**. |
| 🔴 What is Authentication? | Verifying identity (passwords, biometrics, tokens). |
| 🔴 What are the five authentication factors? | Something you know, have, are, somewhere you are, something you do. |
| 🔴 What is Authorization? | Granting specific permissions/rights after authentication. |
| 🔴 What is Accounting? | Tracking and logging user activity for audits or billing purposes. |
| 🔴 What does accounting provide? | Accountability and a detailed audit trail of who did what, and when. |
| **🟢 CIANA Pentagon** | CIANA |
| 🔴 What is the security control triad/CIANA? | CIA triad plus **Non-repudiation** and **Authentication** (Pentagon model). |
| **🟢 Security Controls** |  |
| 🔴 What are security controls? | Measures designed to reduce risk and protect CIA. |
| 🔴 What are the categories of controls? | Technical, Managerial, Operational, Physical. |
| 🔴 What are the types of controls? | Preventive, Deterrent, Detective, Corrective, Compensating, Directive. |
| **🟢 Zero Trust Architecture** | ZTA |
| 🔴 What is the core rule of Zero Trust? | "Never trust, always verify"; no implicit trust based on network location. |
| 🔴 What is the Control Plane? | Adaptive identity, threat scope reduction, policy-driven access, Policy Decision Point. |
| 🔴 What is the Data Plane? | Subject/system traffic passing through a Policy Enforcement Point. |
| **🟢 Risk Management** |  |
| 🔴 Threat vs. vulnerability | **Threat** = potential cause of harm; **vulnerability** = weakness a threat can exploit. |
| 🔴 What is Risk? | Likelihood multiplied by the impact of a threat exploiting a vulnerability. |
| 🔴 Threat + no vulnerability = ? | No risk. |
| 🔴 Vulnerability + no threat = ? | No risk. |
| 🔴 What is a gap analysis? | Comparing current security posture to the desired target state. |

## Summary

Security rests on the **CIA Triad** (Confidentiality, Integrity, Availability), extended by **Non-repudiation** and **Authentication** (CIANA). The **AAA** framework governs identity (Authenticate, Authorize, Account) using up to five factors. Risk arises when a **threat** exploits a **vulnerability**, and is managed through **security controls** organized by category (Technical, Managerial, Operational, Physical) and type (Preventive, Deterrent, Detective, Corrective, Compensating, Directive). **Zero Trust** removes implicit trust, enforcing verification via Control and Data Planes.

