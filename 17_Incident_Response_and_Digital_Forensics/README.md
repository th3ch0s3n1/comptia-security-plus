# 🚨 Section 17: Incident Response & Digital Forensics


> Cornell Notes — CompTIA Security+ (SY0-701) | Maps to Domain 4.0 (Security Operations)


## ❓ Cue / Key Questions & Notes


| Question / Keyword | Answer |
| --- | --- |
| **🟢 Incident Response Lifecycle** |  |
| 🔴 What is an incident response plan? | IRP; A structured framework outlining how an organization detects, contains, and recovers from a cyberattack. |
| 🔴 What are the 6 phases of the IR lifecycle? | 1. **Preparation**, 2. **Detection & Analysis**, 3. **Containment**, 4. **Eradication**, 5. **Recovery**, and 6. **Lessons Learned**. |
| 🔴 Preparation vs. Detection | Preparation involves training, creating playbooks, and hardening systems; Detection is identifying and validating a live security alert. |
| 🔴 Containment vs. Eradication | Containment safely isolates the threat to prevent it from spreading (e.g., disconnecting a host); Eradication completely removes the root cause (e.g., deleting malware). |
| 🔴 What happens during the Recovery phase? | Restoring systems to a known-good operational state from clean backups and continuously monitoring for re-infection. |
| 🔴 What happens during Lessons Learned? | A critical post-incident review to analyze what went wrong, patch remaining gaps, and update the IRP to prevent future breaches. |
| **🟢 Incident Readiness Exercises** |  |
| 🔴 What is a tabletop exercise? | A theoretical, discussion-based walkthrough of an incident scenario with key personnel sitting around a conference table. |
| 🔴 Simulation vs. Live-fire exercise | A simulation drops teams into a realistic, controlled test environment; a live-fire exercise tests real production defenses against simulated active attacks. |
| **🟢 Digital Forensics & Volatility** |  |
| 🔴 What is digital forensics? | The scientific collection, preservation, and analysis of digital evidence for legal or internal investigations. |
| 🔴 What is the Order of Volatility? | The strict sequence of capturing digital evidence starting from the most volatile (disappears fastest) to the least volatile. |
| 🔴 What is the standard Order of Volatility? | 1. **CPU Cache & Registers**, 2. **Routing Tables & RAM**, 3. **Temporary Files/Swap space**, 4. **Hard Drives**, and 5. **Remote Log Repositories / Backups**. |
| **🟢 Evidence Preservation** |  |
| 🔴 What is a chain of custody? | A chronological, legally binding paper trail documenting exactly who collected, handled, and secured a piece of evidence. |
| 🔴 What is a write-blocker? | A hardware or software tool that intercepts write commands to ensure forensic data collection does not accidentally modify the source drive. |
| 🔴 What is a bit-stream image? | An exact bit-by-bit duplicate of a storage drive, including hidden files, unallocated space, and deleted data fragments. |
| 🔴 How is forensic integrity proven? | By hashing the original drive and the forensic image; matching hashes (e.g., SHA-256) prove the evidence has not been altered. |


## 📝 Summary


Managing a security incident effectively requires a highly structured approach dividing response mechanics from evidentiary science. The **Incident Response Lifecycle** guides defenders from **Preparation** and live threat **Detection** into tactical containment and system **Eradication** before bringing systems back online during **Recovery**. Organizations validate this execution framework by running mock **tabletop exercises** and active network simulations. If an incident escalates into a legal or regulatory matter, **digital forensics** teams step in to preserve evidence. Analysts must secure data according to the strict **Order of Volatility**—capturing transient **RAM** and CPU caches before turning to fixed **hard drives**—utilizing cryptographic **hashes** to prove data integrity, physical **write-blockers** to protect original media, exact **bit-stream images**, and a airtight **chain of custody** log to guarantee legal admissibility.
