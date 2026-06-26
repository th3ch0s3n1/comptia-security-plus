# 📊 Section 16: Security Auditing & Monitoring Tools


> Cornell Notes — CompTIA Security+ (SY0-701) | Maps to Domain 4.0 (Security Operations)


## ❓ Cue / Key Questions & Notes


| Question / Keyword | Answer |
| --- | --- |
| **🟢 Threat Detection & Visibility** | SIEM |
| 🔴 What is a SIEM? | Security Information and Event Management; a centralized system that collects, aggregates, and analyzes log data from across an entire enterprise to detect threats. |
| 🔴 What is log aggregation? | The process of gathering raw log files from diverse sources (servers, firewalls, routers) into a single, centralized repository. |
| 🔴 What is correlation analysis? | A SIEM feature that links separate, seemingly unrelated events across different systems to identify a coordinated cyberattack. |
| 🔴 What is a log retention policy? | A compliance or operational rule defining exactly how long log data must be stored and archived before deletion. |
| **🟢 Automated Incident Response** | SOAR |
| 🔴 What is a SOAR system? | Security Orchestration, Automation, and Response; a platform that integrates security tools and automates incident response tasks without human intervention. |
| 🔴 Playbook vs. Runbook | A playbook defines the broader strategic workflow for responding to a specific threat; a runbook contains the exact, step-by-step automated actions executed by the SOAR. |
| **🟢 Network Scanners & Analyzers** |  |
| 🔴 What is Nmap? | A powerful network and port scanner used for network discovery, identifying active hosts, open ports, and operating system fingerprints. |
| 🔴 What is a packet analyzer? | Commonly called a sniffer (e.g., Wireshark); a tool used to intercept, decode, and analyze raw data packets traversing a network. |
| **🟢 Vulnerability Assessment** |  |
| 🔴 What is a vulnerability scanner? | An automated tool (e.g., Nessus) that tests systems, applications, and networks against a database of known security flaws. |
| 🔴 Credentialed vs. Non-Credentialed scan | A credentialed scan logs into the target system with administrative rights to find internal configuration flaws; a non-credentialed scan probes from the outside to find exposed entry points. |
| **🟢 Advanced Endpoint Defense** | EDR |
| 🔴 What is EDR? | Endpoint Detection and Response; continuous monitoring software installed on hosts to detect, isolate, and remediate advanced endpoint threats. |
| 🔴 EDR vs. XDR | EDR focuses strictly on monitoring individual host endpoints; XDR (Extended Detection and Response) expands this visibility across networks, cloud systems, and emails. |


## 📝 Summary


Security operations depend on robust visibility provided by advanced **security auditing and monitoring tools**. At the center of this ecosystem sits a **SIEM**, which drives threat discovery by executing **log aggregation** and **correlation analysis** across the enterprise network. To handle threats at scale, security teams augment their SIEM with **SOAR** platforms, translating high-level incident response **playbooks** into automated, machine-driven **runbooks**. On the ground, security analysts assess the active attack surface using **Nmap** for network topology mapping, **Wireshark** for deep packet inspection, and **vulnerability scanners** running both credentialed and non-credentialed checks. Finally, continuous endpoint integrity is maintained using host-level **EDR** agents, which scale into integrated, cloud-wide **XDR** fabrics to intercept complex, multi-vector attacks.
