# 🆔 Section 14: Identity & Access Management (IAM)


> Cornell Notes — CompTIA Security+ (SY0-701) | Maps to Domain 4.0 (Security Operations)


## ❓ Cue / Key Questions & Notes


| Question / Keyword | Answer |
| --- | --- |
| **🟢 IAM Foundations** |  |
| 🔴 What is Identity & Access Management? | IAM; A framework of business processes, policies, and technologies used to manage digital identities and control user access to critical resources. |
| 🔴 What is Single Sign-On? | SSO; An authentication mechanism that allows a user to log in once with a single set of credentials and gain access to multiple connected applications. |
| 🔴 What is identity federation? | Linking a user's single identity across completely separate, distinct organizations or security domains. |
| **🟢 Federation Protocols** | SAML |
| 🔴 What is SAML? | Security Assertion Markup Language; an XML-based open standard used to exchange authentication and authorization data between an Identity Provider (IdP) and a Service Provider (SP). |
| 🔴 What is OAuth? | An open-standard token framework used strictly for API **authorization**, allowing a third-party application to access resources without exposing the user's password. |
| 🔴 What is OpenID Connect? | OIDC; An identity verification layer built directly on top of the OAuth 2.0 framework to provide **authentication** capabilities. |
| **🟢 Access Control Models** | RBAC |
| 🔴 What is Role-Based Access Control? | RBAC; An access control model that grants system permissions based on a user's specific job function or title within an organization. |
| 🔴 What is Attribute-Based Access Control? | ABAC; An advanced access model that grants permissions dynamically based on contextual attributes (e.g., user department, resource type, current time, or IP location). |
| 🔴 Mandatory vs. Discretionary Access Control | MAC (Mandatory) grants access based on strict data labels and user clearances assigned by an administrator; DAC (Discretionary) allows the individual data owner to manage permissions at their own discretion. |
| **🟢 Privilege Governance** | PAM |
| 🔴 What is Privileged Access Management? | PAM; Specialized security tools and practices used to isolate, secure, log, and closely audit activities performed by high-level administrative (root/admin) accounts. |


## 📝 Summary


**Identity & Access Management (IAM)** establishes the infrastructure required to govern user lifecycles and technical permissions. Organizations streamline user authentication across multiple independent portals by deploying **Single Sign-On (SSO)**, which can scale into external boundaries via identity **federation**. This ecosystem relies on open standards like XML-driven **SAML** for corporate handshakes, alongside modern web frameworks that separate API-driven **OAuth** authorization tokens from identity-centric **OpenID Connect (OIDC)** authentication tokens. Once an identity is verified, access to resources is parsed through structured authorization models: static, job-aligned **RBAC** models, contextual and dynamic **ABAC** policies, strict data-labeled **MAC** clearances, or user-defined **DAC** structures. Finally, to defend against elevated system exploits, security teams isolate high-value admin rights within specialized **Privileged Access Management (PAM)** vault architectures.
