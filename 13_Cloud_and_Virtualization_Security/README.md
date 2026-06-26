# ☁️ Section 13: Cloud & Virtualization Security


> Cornell Notes — CompTIA Security+ (SY0-701) | Maps to Domain 3.0 (Security Architecture)


## ❓ Cue / Key Questions & Notes


| Question / Keyword | Answer |
| --- | --- |
| **🟢 Virtualization Technologies** | VM |
| 🔴 What is a Virtual Machine? | A software-based emulation of a physical computer that runs its own independent operating system. |
| 🔴 What is a hypervisor? | Software that creates, runs, and manages virtual machines by allocating physical hardware resources. |
| 🔴 Type 1 vs. Type 2 Hypervisor | Type 1 (Bare-Metal) runs directly on the physical hardware; Type 2 (Hosted) runs on top of an existing host operating system. |
| 🔴 What is a container? | A lightweight, isolated package that contains an application and only its dependencies, sharing the host OS kernel rather than virtualizing hardware. |
| **🟢 Cloud Service Models** | SPI |
| 🔴 What is Infrastructure as Code? | IaC; managing and provisioning cloud infrastructure using machine-readable configuration files instead of manual setup. |
| 🔴 What is Infrastructure as a Service? | IaaS; cloud provider hosts basic computing infrastructure (servers, storage, networking) while the client manages the OS and applications. |
| 🔴 What is Platform as a Service? | PaaS; cloud provider handles the hardware and the OS environment, allowing clients to focus strictly on deploying and managing applications. |
| 🔴 What is Software as a Service? | SaaS; a complete application hosted, managed, and maintained by the cloud provider and accessed by clients via a web browser. |
| 🔴 What is the Shared Responsibility Model? | A security framework defining which security tasks belong to the cloud provider and which belong to the client based on the service model. |
| **🟢 Cloud Deployment Models** |  |
| 🔴 Public vs. Private Cloud | Public cloud resources are shared dynamically over the internet by multiple organizations; Private cloud infrastructure is dedicated exclusively to one organization. |
| 🔴 What is a Hybrid Cloud? | A cloud computing environment that blends public and private cloud environments, allowing data and apps to be shared between them. |
| 🔴 What is a Community Cloud? | A cloud infrastructure shared mutually by several organizations with common concerns (e.g., compliance, security requirements, or mission goals). |
| **🟢 Modern Cloud Infrastructures** |  |
| 🔴 What is edge computing? | Processing data closer to the source of generation (the "edge" of the network) rather than relying on a centralized cloud data center to reduce latency. |
| 🔴 What is a Cloud Access Security Broker? | CASB; a software tool or service placed between an organization's on-premises infrastructure and cloud provider to enforce security, compliance, and governance policies. |


## 📝 Summary


Securing contemporary enterprise ecosystems requires adapting traditional perimeter controls to **virtualization** and cloud environments. At the virtualization layer, hardware utilization is managed via bare-metal **Type 1** or hosted **Type 2 hypervisors** to run individual **Virtual Machines (VMs)**, while microservices scale using lightweight **containers** that share the host kernel. Organizations provision these systems efficiently using **Infrastructure as Code (IaC)** templates. Depending on business requirements, services are deployed using **IaaS**, **PaaS**, or **SaaS** service models across **public**, **private**, **hybrid**, or **community cloud** environments. Ultimately, cloud security depends on navigating the **Shared Responsibility Model**, utilizing tools like a **Cloud Access Security Broker (CASB)** to audit data baselines, and implementing **edge computing** architectures to securely handle low-latency processing requirements.
