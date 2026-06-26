# 🏢 Section 12: Network Security Architecture


> Cornell Notes — CompTIA Security+ (SY0-701) | Maps to Domain 3.0 (Security Architecture)


## ❓ Cue / Key Questions & Notes


| Question / Keyword | Answer |
| --- | --- |
| **🟢 Perimeter Defense** | NGFW |
| 🔴 What is a firewall? | A network security device that monitors and filters incoming and outgoing network traffic based on an organization's previously established security rules. |
| 🔴 Packet filtering vs. stateful inspection | Packet filtering inspects packets individually based on IP/port headers; stateful inspection tracks the active state of network connections to make filtering decisions. |
| 🔴 What is a Next-Generation Firewall? | An advanced firewall that combines traditional packet filtering with deep packet inspection (DPI), application awareness, and integrated intrusion prevention. |
| 🔴 What is a Web Application Firewall? | WAF; a specialized firewall designed specifically to inspect and filter HTTP/HTTPS traffic to protect web applications from layer 7 attacks (like SQLi and XSS). |
| **🟢 Traffic Monitoring & Prevention** | IDS / IPS |
| 🔴 IDS vs. IPS | An Intrusion Detection System (IDS) monitors traffic and alerts administrators to threats (passive); an Intrusion Prevention System (IPS) actively blocks or drops malicious traffic (active). |
| 🔴 Signature vs. anomaly-based detection | Signature-based detection looks for known patterns or definitions of past threats; anomaly-based detection establishes a baseline of normal behavior and flags deviations. |
| **🟢 Network Isolation** | DMZ |
| 🔴 What is network segmentation? | Dividing a larger network into smaller, isolated subnets (commonly using VLANs) to contain breaches and control traffic flow. |
| 🔴 What is a Demilitarized Zone? | A physical or logical subnetwork that exposes an organization's external-facing services (like web servers) to the untrusted internet while isolating them from the internal network. |
| **🟢 Traffic Optimization & Redirection** |  |
| 🔴 What is a load balancer? | A device that distributes incoming network traffic across a cluster of servers to optimize resource utilization, maximize throughput, and prevent overload. |
| 🔴 Forward proxy vs. reverse proxy | A forward proxy protects and hides internal clients accessing the internet; a reverse proxy protects and hides backend web servers accepting internet traffic. |
| **🟢 Remote Access & Encryption** | VPN |
| 🔴 What is a Virtual Private Network? | An encrypted tunnel that establishes a secure network connection over an unsecure public network (like the internet). |
| 🔴 IPsec vs. SSL/TLS VPNs | IPsec VPNs typically connect whole networks (site-to-site) or require client software at the OS layer; SSL/TLS VPNs provide secure access through standard web browsers (clientless). |
| **🟢 Modern Cloud Networking** | SASE |
| 🔴 What is SASE? | Secure Access Service Edge; a cloud architecture model that rolls software-defined networking (SD-WAN) and comprehensive security functions into a single cloud service provider. |
| 🔴 What is SD-WAN? | Software-Defined Wide Area Network; uses software to dynamically manage and optimize traffic routing across multiple geographic network connections. |


## 📝 Summary


Designing a resilient **network security architecture** requires implementing a multi-layered defensive posture. At the perimeter, organizations deploy **Next-Generation Firewalls (NGFW)** alongside targeted **Web Application Firewalls (WAF)** to handle deep packet inspection. Internal systems rely on **Network Segmentation** via VLANs and isolated **Demilitarized Zones (DMZs)** to isolate external-facing resources from core databases. Traffic paths are monitored continuously using **IDS/IPS** mechanisms driven by signature and anomaly detection, optimized via **load balancers**, and redirected through forward or reverse **proxies**. Remote workforces securely bridge into these corporate environments via encrypted **VPN tunnels** (IPsec or SSL/TLS). To scale these boundaries globally, modern enterprises are migrating toward cloud-native solutions like **SD-WAN** and integrated **Secure Access Service Edge (SASE)** frameworks.
