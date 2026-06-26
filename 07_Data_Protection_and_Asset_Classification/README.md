# 💾 Section 7: Data Protection & Asset Classification


> Cornell Notes — CompTIA Security+ (SY0-701) | Maps to Domain 3.0 (Security Architecture)


## ❓ Cue / Key Questions & Notes


| Question / Keyword | Answer |
| --- | --- |
| **🟢 Data Lifecycle & Classification** |  |
| 🔴 What is data classification? | Labeling data by sensitivity levels to determine and apply appropriate security protections. |
| 🔴 What are standard commercial classifications? | Public, Sensitive, Private, Confidential, and Critical. |
| 🔴 What are standard government classifications? | Unclassified, Confidential, Secret, and Top Secret. |
| 🔴 What is data minimization? | The practice of collecting, processing, and retaining only the absolute minimum amount of data necessary for specific business tasks. |
| **🟢 The Three Data States** |  |
| 🔴 What are the three states of data? | Data at rest (stored), data in transit/motion (moving across networks), and data in use (actively being processed in memory). |
| 🔴 How is data at rest protected? | Via full-disk encryption (FDE), file-level encryption, or database encryption. |
| 🔴 How is data in transit protected? | Via cryptographic network protocols like Transport Layer Security (TLS), Virtual Private Networks (VPNs), and IPsec. |
| 🔴 How is data in use protected? | Via strict access controls, hardware-based secure enclaves, and volatile memory protection. |
| **🟢 Privacy Governance & Roles** |  |
| 🔴 What is data sovereignty? | The legal principle that digital data is subject to the specific laws and regulations of the country in which it physically resides. |
| 🔴 Data Owner | A senior execution role ultimately accountable for the overall security and classification of a specific asset or data set. |
| 🔴 Data Controller vs. Processor | The Controller determines *why* and *how* data is processed; the Processor executes the data processing on behalf of the Controller. |
| 🔴 Data Custodian / Steward | An operational role responsible for managing day-to-day data storage, system backups, technical protections, and data quality. |
| **🟢 Information Exfiltration & Blinding** | DLP |
| 🔴 What is Data Loss Prevention? | Security tools designed to monitor, detect, and block the unauthorized transmission or malicious exfiltration of sensitive data. |
| 🔴 What are common data obfuscation methods? | Encryption, data masking, tokenization, and hashing. |
| 🔴 What is tokenization? | Replacing sensitive data fields with a non-sensitive, random surrogate value called a "token" (commonly used in payment processing). |
| 🔴 What is data masking? | Hiding specific structural portions of a data field (e.g., blanking out all but the last 4 digits of a credit card number). |
| 🔴 What are geographic and segmentation restrictions? | Setting up strict boundaries to limit the exact logical networks or physical regions where data can be stored and accessed. |


## 📝 Summary


Effective **data protection** operates on systemic **data classification** metrics, utilizing either commercial or government frameworks to deploy appropriate safeguards. Security operations must actively protect data across all three structural **data states**: static data **at rest** via file or full-disk encryption, data **in transit** across network segments using **TLS**, **IPsec**, or **VPNs**, and active data **in use** via volatile memory protections and secure enclaves. Organizationally, governance is maintained through defined personnel roles, dividing ultimate accountability (**data owner**) and tactical system upkeep (**data custodian/steward**) while satisfying external **data sovereignty** laws. When safeguarding privacy or handling consumer data, organizations apply data engineering principles like **data minimization** alongside automated **Data Loss Prevention (DLP)** systems and technical obfuscation methods—including structural **data masking** and secure **tokenization**—to dramatically minimize their active attack footprint.
