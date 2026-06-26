# 🔐 Section 10: Cryptographic Concepts & PKI


> Cornell Notes — CompTIA Security+ (SY0-701) | Maps to Domain 1.0 & Domain 3.0 (General Security Concepts / Security Architecture)


## ❓ Cue / Key Questions & Notes


| Question / Keyword | Answer |
| --- | --- |
| **🟢 Cryptographic Foundations** |  |
| 🔴 What is symmetric encryption? | A cryptographic method that uses a single shared key for both encrypting and decrypting data (fast, ideal for bulk data). |
| 🔴 What are common symmetric algorithms? | AES (Advanced Encryption Standard), DES, 3DES, Blowfish, and Twofish. |
| 🔴 What is asymmetric encryption? | A method using a mathematically linked key pair: a Public Key (to encrypt) and a Private Key (to decrypt). |
| 🔴 What are common asymmetric algorithms? | RSA and ECC (Elliptic Curve Cryptography). |
| 🔴 What is Elliptic Curve Cryptography? | ECC; a highly efficient form of asymmetric encryption providing strong security with smaller key sizes, ideal for mobile devices. |
| **🟢 Integrity & Password Hardening** |  |
| 🔴 What is a cryptographic salt? | Random characters added to a password before it is hashed to prevent rainbow table (precomputed hash) attacks. |
| 🔴 What is key stretching? | Intentional slowdown of password hashing (using Bcrypt or PBKDF2) to make brute-force attacks mathematically unfeasible. |
| **🟢 Key Exchange & Secrecy** | DH |
| 🔴 What is Diffie-Hellman? | A cryptographic protocol used to securely exchange a symmetric session key over an entirely unsecure communication channel. |
| 🔴 What is Perfect Forward Secrecy? | PFS; a feature ensuring that a compromise of long-term server keys will not expose past session keys or history. |
| **🟢 Public Key Infrastructure** | PKI |
| 🔴 What is a Certificate Authority? | CA; a trusted third-party entity that issues, signs, and manages digital certificates. |
| 🔴 What is a Registration Authority? | RA; an entity that verifies user identity and validates requests before forwarding them to the CA for signing. |
| 🔴 What is an X.509 certificate? | The standard format defining the structured fields inside a public key digital certificate. |
| **🟢 Certificate Revocation** | CRL |
| 🔴 What is a Certificate Revocation List? | CRL; a periodic, downloadable list of digital certificates that have been canceled by the CA before their expiration date. |
| 🔴 What is OCSP? | Online Certificate Status Protocol; a real-time, lightweight protocol used by browsers to check certificate validity instantly. |
| 🔴 What is certificate pinning? | Associating a specific host with their expected X.509 certificate to prevent Man-in-the-Middle attacks. |


## 📝 Summary


Cryptography underpins modern information assurance by protecting data across all operational environments. **Symmetric encryption** relies on a single shared key for rapid bulk processing, whereas **asymmetric encryption** utilizes a public-private key pair to securely encrypt data and scale operations. Legacy mathematical frameworks are continually optimized using **Elliptic Curve Cryptography (ECC)** for constrained systems, alongside **Diffie-Hellman** protocols for out-of-band key exchange and **Perfect Forward Secrecy (PFS)** to shield past communications from future breaches. At the software level, credential stores counter dictionary threats by embedding randomized **salts** and applying structural **key stretching** algorithms. Trust architecture is scaled globally via the **Public Key Infrastructure (PKI)**, wherein a **Certificate Authority (CA)** and **Registration Authority (RA)** validate identities using **X.509 certificates**, while downstream entities maintain validity states using real-time **OCSP** queries or standardized **Certificate Revocation Lists (CRLs)**.
