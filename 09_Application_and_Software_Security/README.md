# 💻 Section 9: Application & Software Security


> Cornell Notes — CompTIA Security+ (SY0-701) | Maps to Domain 2.0 & Domain 3.0 (Threats, Vulnerabilities, and Mitigations / Security Architecture)


## ❓ Cue / Key Questions & Notes


| Question / Keyword | Answer |
| --- | --- |
| **🟢 Injection & Input Attacks** | SQLi |
| 🔴 What is SQL Injection? | Inserting malicious SQL commands into database input fields to manipulate or bypass authentication. |
| 🔴 What is Cross-Site Scripting? | XSS; injecting malicious scripts into a trusted website that execute in a victim's web browser. |
| 🔴 What is input validation? | The practice of checking and filtering all user-supplied data to ensure it matches expected formats before processing. |
| 🔴 What are parameterized queries? | Pre-compiled database statements that completely isolate user input from executable command logic (the primary defense against SQLi). |
| **🟢 Web & Session Vulnerabilities** | CSRF |
| 🔴 What is Cross-Site Request Forgery? | CSRF; tricking an authenticated user's browser into executing an unauthorized, malicious action on a trusted web application. |
| 🔴 What is directory traversal? | Exploiting weak input sanitization to navigate outside the intended web server root directory using characters like `../`. |
| 🔴 What are API vulnerabilities? | Flaws in Application Programming Interfaces, such as lack of token authentication, weak rate limiting, or excessive data exposure. |
| **🟢 Memory & State Flaws** |  |
| 🔴 What is a buffer overflow? | Writing more data into a memory buffer than it can hold, overwriting adjacent memory spaces to cause a crash or execute arbitrary code. |
| 🔴 What is a race condition? | A software flaw where the system's output depends on the uncontrolled sequence or timing of concurrent execution threads. |
| 🔴 What is a memory leak? | A bug where an application fails to release memory it no longer needs, gradually consuming available RAM and causing system instability. |
| **🟢 Access & Privilege Exploitation** |  |
| 🔴 What is privilege escalation? | An attack where an adversary exploits a flaw to gain higher permissions (vertical) or different user roles (horizontal) than intended. |
| 🔴 What is improper error handling? | Displaying detailed system errors or stack traces to end-users, inadvertently leaking valuable system architecture data to attackers. |
| **🟢 Secure Code Testing** | SAST |
| 🔴 Static vs. Dynamic Code Analysis | Static testing (SAST) analyzes code while offline without running it; Dynamic testing (DAST) tests the application from the outside while it is running. |
| 🔴 What is code signing? | Utilizing a digital signature to cryptographically verify the author's identity and the baseline integrity of software executables. |


## 📝 Summary


Application security focuses on eliminating coding vulnerabilities that attackers leverage to hijack software execution. Input manipulation forms the foundation of attacks like **SQL Injection (SQLi)** and **Cross-Site Scripting (XSS)**, which can be mitigated through structural **input validation** and **parameterized queries**. Web applications are further exposed to session-based threats like **Cross-Site Request Forgery (CSRF)** and architecture bypasses like **directory traversal**. At the hardware execution layer, flaws like **buffer overflows** and **race conditions** threaten system memory integrity. Defending application ecosystems requires strict error handling policies, cryptographic **code signing**, and robust assurance frameworks that combine static (**SAST**) and dynamic (**DAST**) code analysis throughout the development lifecycle.
