# 🔑 Section 15: Account Management & AAA


> Cornell Notes — CompTIA Security+ (SY0-701) | Maps to Domain 4.0 (Security Operations)


## ❓ Cue / Key Questions & Notes


| Question / Keyword | Answer |
| --- | --- |
| **🟢 AAA Architecture** | AAA |
| 🔴 What are the core components of AAA? | **Authentication** (verifying identity), **Authorization** (granting permissions), and **Accounting** (logging user activities). |
| 🔴 What is RADIUS? | Remote Authentication Dial-In User Service; an open-standard centralized AAA protocol that encrypts only the password field (runs over UDP). |
| 🔴 What is TACACS+? | Terminal Access Controller Access-Control System Plus; a Cisco AAA protocol that encrypts the entire packet payload and separates AAA into distinct functions (runs over TCP port 49). |
| 🔴 What is Kerberos? | A ticket-based network authentication protocol used by Windows Active Directory to provide secure Single Sign-On (SSO) using a Key Distribution Center (KDC). |
| **🟢 Authentication Mechanics** | MFA |
| 🔴 What are the five authentication factors? | Something you **know** (password), something you **have** (smart card), something you **are** (biometric), somewhere you **are** (location), and something you **do** (behavior/gait). |
| 🔴 What is Multi-Factor Authentication? | Requiring a user to present two or more *different* categories of authentication factors to verify identity. |
| 🔴 Hard token vs. soft token | A hard token is a physical device (e.g., hardware security key); a soft token is an application-based code generator (e.g., Google Authenticator). |
| 🔴 TOTP vs. HOTP | Time-based One-Time Password (expires after a set window, usually 30 seconds); HMAC-based One-Time Password (expires only after it is used, based on a counter). |
| **🟢 Account Types** |  |
| 🔴 What is a service account? | A non-human account explicitly used by applications or system processes to run automated tasks under a specific security context. |
| 🔴 Shared vs. Guest accounts | Shared accounts are used by multiple users (destroying accountability); Guest accounts are temporary, highly restricted accounts for short-term network access. |
| 🔴 What is a privileged account? | High-level administrative accounts (such as `root` or `Administrator`) that possess full command capabilities across a system. |
| **🟢 Account Security Policies** |  |
| 🔴 What is an account lockout policy? | Disabling an account automatically after a specific number of consecutive failed login attempts to block brute-force attacks. |
| 🔴 Time-of-day vs. location restrictions | Time-of-day limits logins to specific working hours; location restrictions block access if a user attempts entry from an unapproved IP range or geographic region. |
| 🔴 What is access recertification? | The periodic review process where auditors or management verify that an employee's current access rights are still required for their job role. |


## 📝 Summary


The **AAA framework** provides identity governance by chaining **Authentication**, **Authorization**, and **Accounting** into a unified security pipeline. Systems scale this control centrally across corporate networks using protocols like open-standard **RADIUS**, payload-encrypted **TACACS+**, or ticket-driven Windows **Kerberos** architectures. Strong access management mandates **Multi-Factor Authentication (MFA)**, requiring users to supply components spanning at least two of the **five authentication factors** (know, have, are, somewhere, do) using mechanisms like time-sensitive **TOTP** or event-driven **HOTP** tokens. Finally, administrators must classify and segment network identity types—isolating human user accounts from automated **service accounts** and elevated **privileged accounts**—while applying strict operational guardrails like automated **account lockouts**, time/location restrictions, and periodic **access recertification** audits to eliminate privilege creep.
