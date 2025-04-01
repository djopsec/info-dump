# Security and Compliance Engineer Study Guide

## A

---

### **Access Control**

**Definition:**  
Access control is the process of defining who can access what in an information system. It ensures that only authorized users can view or use specific resources.

**Types:**
- **Discretionary Access Control (DAC):** Owner controls access.
- **Mandatory Access Control (MAC):** Central authority enforces rules.
- **Role-Based Access Control (RBAC):** Access based on job roles.
- **Attribute-Based Access Control (ABAC):** Access determined by user attributes (e.g., location, time).

**Example:**  
An HR employee can access personnel records, but not payroll systems. Meanwhile, finance employees can access payroll but not HR records.

---

### **AI Impact Assessments**

**Definition:**  
An AI Impact Assessment is a structured review of how an AI system may affect people, organizations, and systems. It evaluates potential risks, ethical concerns, and regulatory compliance.

**Why it matters:**  
AI systems can introduce bias, discrimination, or safety concerns. Assessments help organizations ensure responsible AI deployment.

**Key components:**
- Purpose of the AI system
- Data sources and training methodologies
- Risks to individuals (privacy, fairness)
- Mitigation and governance strategies

---

### **AI Management Systems Security and Compliance**

**Definition:**  
This refers to the governance and protection mechanisms applied to the full lifecycle of AI systems—from data collection and training to deployment and monitoring.

**Use Case:**  
An AI used in healthcare must comply with data privacy laws, document its decision-making, and ensure data is securely stored and used ethically.

**Focus Areas:**
- Access controls to training data
- Transparency and explainability
- Bias detection and mitigation
- Secure model deployment and logging

---

### **AI TRiSM (AI Trust, Risk, and Security Management)**

**Definition:**  
AI TRiSM encompasses the frameworks, practices, and tools used to build, deploy, and monitor AI systems responsibly and securely.

**Components:**
- **Trust:** Transparency, explainability, and ethical alignment.
- **Risk:** Identification and mitigation of model-related risks.
- **Security:** Protection of AI assets (e.g., data poisoning defense).

**Example:**  
An AI loan approval tool must be explainable (why was the loan denied?) and protected from adversarial attacks.

---

### **API Architectures and Usage**

**Definition:**  
APIs (Application Programming Interfaces) are contracts that allow software systems to talk to each other. API architecture refers to the design and structure of these communication methods.

**Types:**
- **REST:** Stateless, uses HTTP methods.
- **GraphQL:** Flexible, lets clients ask for specific data.
- **SOAP:** XML-based, strict standards.

**Security Practices:**
- Use authentication (e.g., API keys, OAuth)
- Validate and sanitize input
- Rate limiting and throttling
- Monitor for abuse

---

### **Application Hosting**

**Definition:**  
This refers to where and how applications are deployed and made accessible over a network.

**Types:**
- **On-premise:** Hosted on internal servers.
- **Cloud-based:** Hosted by a cloud provider.
- **Hybrid:** A mix of both.

**Security Considerations:**
- Proper access control
- Encryption in transit and at rest
- Monitoring and logging
- Secure configuration of the hosting environment

---

### **Authentication**

**Definition:**  
Authentication is the process of verifying the identity of a user, system, or service.

**Methods:**
- **Something you know:** Passwords or PINs.
- **Something you have:** Security token or smartphone.
- **Something you are:** Biometrics like fingerprints or face ID.

**Best Practices:**
- Use Multi-Factor Authentication (MFA)
- Avoid hardcoded credentials
- Rotate secrets and tokens regularly

**Analogy:**  
Authentication is like showing your ID at a club. You’re proving you are who you say you are.

---

## B

---

### **Best Practices for Training Employees on Cybersecurity Topics**

**Definition:**  
Cybersecurity awareness training helps employees understand threats and practice safe behavior to protect the organization’s data and systems.

**Core Goals:**
- Reduce phishing and social engineering risks
- Encourage strong password hygiene
- Promote responsible data handling

**Effective Tactics:**
- **Regular Training:** Quarterly or biannual sessions.
- **Interactive Exercises:** Simulated phishing attacks.
- **Role-Based Training:** Tailor content for engineering, HR, leadership, etc.
- **Gamification:** Make training fun and competitive.

**Pro Tip:**  
Training should be engaging and ongoing—not a once-a-year checkbox.

---

### **Breach Preparation and Response**

**Definition:**  
This is the strategy and set of actions an organization takes to prepare for, detect, and respond to security breaches or data compromises.

**Preparation Includes:**
- Creating and testing an **Incident Response Plan (IRP)**
- Role assignments: Who handles communication, forensics, legal, etc.
- Logging and monitoring systems in place

**Response Steps:**
1. Detect and confirm the breach
2. Contain the incident (e.g., isolate affected systems)
3. Notify stakeholders
4. Investigate root cause
5. Remediate and prevent future issues

**Analogy:**  
Think of breach preparation like a fire drill. You don’t wait for the fire to start practicing what to do.

---

### **Business Impact Assessments (BIA)**

**Definition:**  
A BIA evaluates the effects of a disruption (like a cyberattack or system outage) on business operations. It helps prioritize systems and data based on their criticality.

**Key Elements:**
- Identify critical business functions
- Estimate financial and operational impact of downtime
- Define **Recovery Time Objectives (RTO)** and **Recovery Point Objectives (RPO)**

**Why it matters:**  
Knowing what’s critical helps allocate resources and respond effectively in a crisis.

---

## C

---

### **Containarizations**

**Definition:**  
Containerization is the practice of packaging software code and all its dependencies into a single, lightweight unit called a **container**.

**Why it matters:**  
Containers ensure that applications run reliably across different environments, whether it’s your laptop, a test server, or production.

**Popular Tools:**  
Container engines (like Docker) and orchestrators (like Kubernetes).

**Security Considerations:**
- Avoid running containers as root
- Use minimal base images
- Regularly update containers
- Isolate workloads using namespaces and control groups (cgroups)

**Analogy:**  
Think of containers like shipping containers—you can ship your app anywhere, and it’ll always run the same way.

---

### **Common Cyberattacks**

**Definition:**  
Cyberattacks are malicious attempts to access, alter, or destroy data, disrupt services, or gain unauthorized control of systems.

**Common Types:**
- **Phishing:** Tricking users into revealing credentials.
- **Ransomware:** Encrypting data and demanding payment.
- **DDoS (Distributed Denial of Service):** Overwhelming a system with traffic.
- **Man-in-the-Middle (MitM):** Intercepting communication between two parties.
- **Credential Stuffing:** Using leaked credentials to log into systems.

**Prevention Tools:**
- Firewalls, anti-malware, MFA, email filtering, and user education.

---

### **Cryptography**

**Definition:**  
Cryptography is the science of protecting information by transforming it into a secure format, often unreadable without a key.

**Key Concepts:**
- **Encryption:** Converts plaintext to unreadable ciphertext (can be reversed).
- **Hashing:** Irreversibly maps data to a fixed-length value (e.g., passwords).
- **Encoding:** For data formatting—not security (e.g., Base64).
- **Digital Signatures:** Ensure message authenticity and integrity.

**Types of Encryption:**
- **Symmetric:** Same key to encrypt and decrypt.
- **Asymmetric:** Public/private key pair (e.g., RSA).

**Use Case:**  
Encrypting emails or files to prevent unauthorized access.

---

## D

---

### **Data Loss Prevention (DLP)**

**Definition:**  
DLP refers to strategies and tools used to prevent unauthorized access, transmission, or destruction of sensitive data—like personal information, trade secrets, or financial records.

**Common Techniques:**
- **Content inspection**: Scan documents/emails for sensitive data (e.g., credit card numbers).
- **Endpoint controls**: Block USBs or unauthorized file transfers.
- **Email filtering**: Prevent accidental data leakage via attachments or external domains.

**Use Case:**  
Preventing an employee from emailing a spreadsheet full of customer SSNs outside the company.

---

### **DevOps**

**Definition:**  
DevOps is a set of practices combining software development (Dev) and IT operations (Ops) to shorten development cycles, increase deployment frequency, and improve reliability.

**Core Goals:**
- Automate repetitive tasks
- Foster collaboration between developers and operations teams
- Deliver value quickly and securely

**Common Tools:**  
CI/CD pipelines, infrastructure as code, container orchestration.

**Security Consideration:**  
Security must be integrated from the beginning—not bolted on at the end.

---

### **DevSecOps**

**Definition:**  
DevSecOps extends DevOps by embedding **security into every stage** of the software development lifecycle.

**Key Practices:**
- **Shift left**: Find and fix issues early (e.g., code scans, IaC security).
- Automate security checks in CI/CD pipelines
- Use policy-as-code to enforce rules
- Foster security culture across teams

**Analogy:**  
DevSecOps is like putting airbags in a car during the design phase—not after the crash test.

---

### **DNS (Domain Name System)**

**Definition:**  
DNS translates human-readable domain names (like `example.com`) into IP addresses that computers use to identify each other.

**How it works:**
1. You type `example.com`
2. DNS resolver asks a root server → top-level domain server → authoritative server
3. The IP address is returned, and your browser connects

**Security Risks:**
- **DNS Spoofing:** Attackers redirect traffic to fake sites.
- **DNS Tunneling:** Using DNS queries to exfiltrate data.

**Security Tips:**
- Use DNS filtering
- Enable DNSSEC (DNS Security Extensions)

---

## E

---

### **Endpoint Protection**

**Definition:**  
Endpoint protection involves securing devices like laptops, mobile phones, and desktops from threats.

**Core Components:**
- **Antivirus/anti-malware**
- **Endpoint detection and response (EDR)**
- **Firewall and application control**
- **Device encryption**

**Use Case:**  
If an employee's laptop is stolen, endpoint protection helps prevent data theft or lateral movement into the network.

Excellent! Let’s explore **Letter E** of your **Security and Compliance Engineer Study Guide**.

---

### **Enterprise Security & Compliance Culture**

**Definition:**  
Enterprise security and compliance culture refers to how well security and compliance values are integrated into an organization's daily operations, decision-making, and mindset—from executives to interns.

**Key Components:**
- **Top-down support:** Leadership must champion security and compliance.
- **Clear policies and standards:** Everyone knows what is expected.
- **Training and awareness:** Employees are equipped to make secure decisions.
- **Accountability:** Roles and responsibilities are defined and enforced.

**Why it matters:**  
Security tools are only effective if people use them correctly. A strong culture makes secure behavior the norm, not the exception.

**Example:**  
An organization with a healthy compliance culture has employees who proactively report phishing emails and understand why they need to use MFA.

---

### **Encoding, Encryption, and Hashing**

**Quick Reference:**

| Concept     | Reversible? | Purpose                          | Common Uses                      |
|-------------|-------------|----------------------------------|----------------------------------|
| Encoding    | ✅          | Data formatting                  | URL encoding, Base64             |
| Encryption  | ✅ (with key) | Data confidentiality             | Secure messages, HTTPS           |
| Hashing     | ❌          | Data integrity (fixed output)     | Password storage, file integrity |

**Analogy:**  
- **Encoding**: Putting your lunch in a labeled container.
- **Encryption**: Locking it with a key.
- **Hashing**: Taking a photo of your lunch and destroying the actual meal—can’t get the meal back from the photo.

---

## F

---

### **Firewall**

**Definition:**  
A firewall is a security system—either hardware, software, or both—that monitors and controls incoming and outgoing network traffic based on predetermined rules.

**Types:**
- **Network Firewall:** Positioned between internal networks and the internet to block unauthorized access.
- **Host-based Firewall:** Installed on individual devices to protect them.
- **Next-Gen Firewall (NGFW):** Adds features like intrusion prevention, app awareness, and user-based policies.

**Example:**  
A firewall might block all traffic from known malicious IP addresses or restrict employee devices from accessing social media during work hours.

**Analogy:**  
Think of a firewall as a nightclub bouncer—only letting approved guests through and turning away anyone who’s not on the list.

---

### **Federated Identity**

**Definition:**  
Federated identity is a system that allows users to access multiple services using a single set of credentials managed by a central identity provider.

**Use Case:**  
A user logs into a business app using their company email, which authenticates through a third-party identity provider. They can then access other connected services without logging in again.

**Benefits:**
- Simplifies user experience
- Reduces password reuse and fatigue
- Centralizes access management

**Security Note:**  
Federated identity systems need strong trust and security controls in place, including multi-factor authentication and monitoring.

---

## G

---

### **GDPR (General Data Protection Regulation)**

**Definition:**  
The **General Data Protection Regulation** is a comprehensive data protection law from the European Union that governs how organizations collect, process, and store personal data of individuals within the EU and EEA.

**Core Principles:**
- **Lawfulness, fairness, and transparency**
- **Purpose limitation**
- **Data minimization**
- **Accuracy**
- **Storage limitation**
- **Integrity and confidentiality**
- **Accountability**

**Key Rights for Individuals:**
- Right to access their data
- Right to be forgotten (data erasure)
- Right to data portability
- Right to object to processing

**Organizational Requirements:**
- Obtain valid consent
- Maintain a lawful basis for processing data
- Implement appropriate security controls
- Report data breaches within 72 hours

**Example:**  
A company offering services to EU residents must clearly disclose how they use personal data, gain explicit opt-in consent, and allow users to delete their account data upon request.

---

## H

---

### **Hardening (Endpoint, Cloud, Asset, etc.)**

**Definition:**  
Hardening refers to the process of securing systems by reducing their attack surface—removing unnecessary software, services, permissions, and potential vulnerabilities.

**Hardening Targets:**
- **Endpoints:** Disable unused ports, enforce encryption, apply strong password policies.
- **Servers:** Remove default accounts, configure firewalls, keep only necessary services.
- **Cloud environments:** Implement least privilege IAM policies, enable logging, secure APIs.
- **Applications:** Disable debug modes, validate inputs, apply secure defaults.

**Example:**  
A hardened cloud server might only allow SSH access from a specific IP range, require MFA for console access, and have automatic patching enabled.

**Analogy:**  
Hardening is like reinforcing a house—installing locks, removing ladders outside, and sealing windows to keep out intruders.

---

### **HTTP (Hypertext Transfer Protocol)**

**Definition:**  
HTTP is the protocol used for transferring web pages and resources between web servers and browsers.

**HTTP Methods:**
- **GET:** Retrieve data
- **POST:** Submit data
- **PUT/PATCH:** Update data
- **DELETE:** Remove data

**Security Considerations:**
- Use **HTTPS** (secure HTTP) to encrypt traffic and protect data in transit.
- Validate and sanitize input to avoid injection attacks.
- Rate-limit sensitive endpoints.

**Analogy:**  
HTTP is like the postal system for the internet—sending and receiving information, and HTTPS is the secure, sealed envelope version.

---

### **HTTPS / SSL (Secure Sockets Layer)**  
*(Covered under "SSL" in a future letter. HTTP/HTTPS distinction explained above; SSL/TLS will be detailed with S.)*

---

## I

---

### **IDS (Intrusion Detection System)**

**Definition:**  
An IDS is a system that monitors network or system activity for suspicious behavior or policy violations and alerts administrators when potential threats are detected.

**Types:**
- **Network-based IDS (NIDS):** Monitors traffic across the network.
- **Host-based IDS (HIDS):** Monitors activity on individual devices.

**Function:**  
An IDS is a detection-only tool. It does **not block** threats—it logs and alerts.

**Use Case:**  
An IDS might detect repeated failed login attempts or port scanning activity on a network, alerting the security team to investigate.

---

### **IPS (Intrusion Prevention System)**

**Definition:**  
An IPS is a real-time network security system that not only detects potential threats like an IDS, but also **actively blocks or prevents them** from executing.

**Common Actions:**
- Drop malicious packets
- Block IP addresses
- Terminate suspicious sessions

**Difference from IDS:**  
An IPS adds **automatic intervention** to threat detection.

**Use Case:**  
If an IPS detects known malware signatures in incoming web traffic, it can block that traffic before it reaches the target server.

---

### **Incident Response**

**Definition:**  
Incident response refers to the structured process an organization follows when detecting, responding to, and recovering from cybersecurity incidents or data breaches.

**NIST-Based Phases:**
1. **Preparation:** Build an incident response plan (IRP), assign roles.
2. **Detection & Analysis:** Identify signs of incidents (alerts, logs, etc.).
3. **Containment, Eradication & Recovery:** Stop the threat, remove it, and restore normal operations.
4. **Post-Incident Review:** Analyze what happened and improve response processes.

**Why It Matters:**  
Well-prepared teams can limit damage, reduce recovery time, and prevent future attacks.

---

### **ISO 27001 (Information Security Management System – ISMS)**

**Definition:**  
ISO 27001 is the international standard for establishing, implementing, maintaining, and improving an **Information Security Management System (ISMS)**.

**Focus Areas:**
- Information security policy and objectives
- Risk assessments and risk treatment plans
- Roles and responsibilities
- Incident management procedures
- Training and awareness

**Annex A Control Domains (2022 Update):**
1. **Organizational controls**
2. **People controls**
3. **Physical controls**
4. **Technological controls**

**Use Case:**  
An organization seeking to protect customer data and pass vendor security reviews implements ISO 27001 to establish a repeatable, auditable security program.

---

### **ISO 42001 (Artificial Intelligence Management Systems)**

**Definition:**  
ISO 42001 is an emerging international standard focused on the **governance and risk management of AI systems**.

**Core Themes:**
- Responsible AI development and use
- Lifecycle governance (from training to deployment)
- Human oversight and explainability
- Compliance with legal and ethical obligations

**Why It’s Important:**  
As AI systems become widespread in decision-making (e.g., hiring, lending, healthcare), organizations need a formal framework for accountability and transparency.

---

### **ISO 9001 (Quality Management System – QMS)**

**Definition:**  
ISO 9001 is an international standard that provides a framework for a **Quality Management System (QMS)** to ensure consistent processes, continuous improvement, and customer satisfaction.

**Relation to Security & Compliance:**
- Helps structure policy and documentation practices.
- Aligns well with ISO 27001 in terms of repeatable, measurable improvements.
- Often seen in mature organizations that value compliance and risk management.

**Use Case:**  
A company aligning its security practices with ISO 27001 may also adopt ISO 9001 to reinforce consistent quality in operations and reporting.

---

## J

---

### **JavaScript**

**Definition:**  
JavaScript is a popular, high-level programming language used primarily to add interactivity and dynamic behavior to web pages. It's run in the browser and is a core part of modern web applications.

**Security Considerations:**
- **Cross-Site Scripting (XSS):** One of the most common vulnerabilities involving JavaScript.
- **DOM Manipulation Risks:** Attackers can exploit poorly validated user input.
- **Third-Party Libraries:** Libraries and dependencies can introduce vulnerabilities.

**Best Practices:**
- Sanitize all user input
- Use secure coding frameworks and linters
- Apply Content Security Policy (CSP)

**Example:**  
JavaScript can validate form fields before sending data to the server—but if not properly secured, malicious input might still be submitted and executed.

---

### **jQuery**

**Definition:**  
jQuery is a lightweight JavaScript library that simplifies DOM manipulation, event handling, and AJAX interactions.

**Security Tip:**  
Because it allows direct DOM access, insecure use of jQuery can introduce XSS or logic vulnerabilities. Many security teams now favor modern frameworks like React or Vue, which offer better structure and security by default.

**Use Case:**  
Form validation, animations, and asynchronous page updates.

---

### **JSON (JavaScript Object Notation)**

**Definition:**  
JSON is a lightweight data-interchange format used widely in APIs, configuration files, and data storage.

**Why It Matters:**  
Most modern web applications use JSON to send and receive structured data between clients and servers.

**Security Considerations:**
- **Injection Risks:** Malicious data could tamper with app logic if not validated.
- **Exposed Sensitive Data:** Be cautious of over-sharing data in API responses.
- **Parsing:** Improper parsing could lead to crashes or logic errors.

**Example:**  
A login API might return `{ "user": "soft", "token": "abc123" }`. That token must be securely stored and transmitted via HTTPS.

---

## K

---

### **Kill Chain**

**Definition:**  
The **Cyber Kill Chain** is a model developed to describe the stages of a cyberattack, from initial reconnaissance to achieving the attacker’s objective. It helps defenders understand, detect, and disrupt attacks at various stages.

**Kill Chain Phases:**
1. **Reconnaissance:** Attacker gathers intel (e.g., employee names, exposed services).
2. **Weaponization:** Creating malware or tools based on intel.
3. **Delivery:** Sending the payload (e.g., phishing email, malicious USB).
4. **Exploitation:** Triggering the payload to gain access.
5. **Installation:** Installing malware or persistence mechanisms.
6. **Command and Control (C2):** Attacker connects back to the compromised system.
7. **Actions on Objectives:** Exfiltrating data, encrypting systems, or lateral movement.

**Use Case:**  
If you detect a phishing attempt (Delivery stage), you can stop the attack before it progresses to Exploitation or Installation.

**Bonus:**  
Modern defenders often pair this with MITRE ATT&CK for more granular tactics and techniques.

---

### **Kubernetes**

**Definition:**  
Kubernetes (often abbreviated as **K8s**) is an open-source container orchestration platform that automates the deployment, scaling, and management of containerized applications.

**Key Components:**
- **Pods:** Smallest unit in Kubernetes, usually holding one or more containers.
- **Nodes:** Machines (virtual or physical) running your workloads.
- **Control Plane:** Manages cluster-wide activities (scheduling, scaling, etc.).
- **Services & Ingress:** Handle traffic routing and load balancing.

**Security Considerations:**
- **RBAC (Role-Based Access Control):** Control who can do what.
- **Secrets Management:** Avoid hardcoding credentials; use Kubernetes secrets.
- **Network Policies:** Limit communication between pods to reduce lateral movement.
- **Container Hardening:** Just like with Docker—minimal base images, no root users.

**Use Case:**  
You might use Kubernetes to manage hundreds of microservices in production, ensuring they scale up during peak hours and down when traffic is low—without manual intervention.

---

## L

---

### **Load Balancers**

**Definition:**  
A load balancer is a networking tool that distributes incoming traffic across multiple servers or resources to ensure no single system becomes overwhelmed.

**Types:**
- **Layer 4 (Transport Layer):** Balances traffic based on TCP/UDP data.
- **Layer 7 (Application Layer):** Balances traffic using application-level data (e.g., URLs, cookies, headers).

**Benefits:**
- Improves **availability** by rerouting traffic if a server fails.
- Enhances **performance** by spreading load evenly.
- Supports **security** via features like SSL termination and DDoS mitigation.

**Example:**  
An e-commerce website with spikes in traffic during sales events uses a load balancer to spread requests across multiple web servers to avoid crashes.

**Analogy:**  
Think of it like a restaurant host guiding guests to different tables to prevent any single server from getting swamped.

---

## M

---

### **Machine Learning Operations (ML Ops)**

**Definition:**  
ML Ops is the set of practices for managing the lifecycle of machine learning models—from development to deployment to monitoring in production.

**Why It Matters for Security:**
- ML models can leak sensitive training data if not handled carefully.
- Adversaries may perform **model inversion**, **membership inference**, or **data poisoning**.
- Pipelines need to be secured like any software stack (access control, CI/CD, logging).

**Security Focus Areas:**
- Validate training data sources
- Version control models and training scripts
- Use audit trails for model changes
- Restrict who can deploy or query models

---

### **Man-in-the-Middle (MitM) Attack**

**Definition:**  
A MitM attack occurs when an attacker secretly intercepts and possibly alters the communication between two parties who believe they’re directly communicating with each other.

**Common Scenarios:**
- Intercepting traffic on public Wi-Fi
- DNS spoofing or ARP poisoning
- HTTPS stripping

**Defenses:**
- Enforce **HTTPS everywhere**
- Use **VPNs** on untrusted networks
- Implement **TLS pinning** in apps
- Educate users about certificate warnings

**Analogy:**  
It’s like someone tapping your phone line and pretending to be your friend—while changing your messages.

---

### **Monitoring**

**Definition:**  
Monitoring is the continuous collection, analysis, and alerting on system or network data to ensure performance, availability, and **security visibility**.

**Security Monitoring Includes:**
- Log aggregation (system logs, app logs, auth events)
- Anomaly detection (e.g., unusual login times)
- Alerting and escalation (to on-call or incident response teams)

**Tools May Track:**
- Failed login attempts
- Unusual network traffic
- File integrity changes
- Admin privilege escalations

**Best Practices:**
- Set baselines to detect deviations
- Store logs securely and centrally
- Retain logs for auditing and forensics

---

### **Multifactor Authentication (MFA)**

**Definition:**  
MFA is a security mechanism that requires users to provide two or more verification factors to gain access to a system or account.

**Common Factors:**
- **Something you know:** Password or PIN
- **Something you have:** Phone, security key
- **Something you are:** Fingerprint, face recognition

**Why It Matters:**  
Even if passwords are stolen, an attacker would need the second factor to log in—making account takeovers much harder.

**Use Case:**  
Your cloud provider admin panel should require MFA for all logins—ideally with hardware keys or time-based one-time passwords (TOTP).

---

### **Metadata and Privacy**

**Definition:**  
Metadata is data about data—such as timestamps, file authors, email routing details, or geolocation embedded in photos.

**Security Concerns:**
- Metadata can reveal sensitive or contextual information.
- Attackers can exploit metadata to learn about internal systems or users.

**Use Case:**  
Before sharing internal documents externally, sanitize metadata to avoid leaking internal usernames, software versions, or author notes.

---

### **Mobile Security**

**Definition:**  
Mobile security refers to the protection of smartphones, tablets, and other portable devices from threats and vulnerabilities.

**Key Areas:**
- App sandboxing and permissions
- Encrypted communication
- Secure app development
- Mobile device management (MDM)

**Common Threats:**
- Malicious apps
- Jailbreaking/rooting
- Insecure app data storage

**Compliance Tip:**  
Ensure personal devices used for work meet security policies before allowing access to sensitive systems or data (BYOD security policy).

---

## N

---

### **Network Security**

**Definition:**  
Network security encompasses technologies, policies, and practices used to protect the integrity, confidentiality, and availability of networked systems and data.

**Core Concepts:**
- **Segmentation:** Isolate sensitive systems (e.g., production vs. development).
- **Access Control:** Use firewalls, VLANs, and security groups to control traffic.
- **Traffic Monitoring:** IDS/IPS, flow analysis, anomaly detection.
- **Encryption in Transit:** Secure data using TLS/SSL or VPNs.
- **Zero Trust Model:** Never trust, always verify—enforce authentication and authorization at every step.

**Use Case:**  
A company segments its network so that IoT devices cannot communicate directly with corporate workstations or servers.

---

### **Networking Basics**

**Definition:**  
Networking is the interconnection of computers and devices to share resources, data, and services. It forms the foundation of the internet and organizational infrastructure.

**Key Concepts:**
- **IP Address:** A unique identifier for a device on a network.
- **MAC Address:** A hardware-based identifier used on local networks.
- **Switches vs. Routers:**
  - **Switches:** Connect devices within a local network (Layer 2).
  - **Routers:** Connect different networks and route traffic (Layer 3).
- **Ports:** Numbers that specify types of services (e.g., 80 for HTTP, 443 for HTTPS).

**Analogy:**  
Think of a network like a city—IP addresses are like street addresses, switches are intersections, routers are highways, and ports are doors to specific rooms in a building.

---

### **NIST AI Framework (NIST AIF)**

**Definition:**  
The NIST AI Framework (AIF) provides guidance on developing, deploying, and managing trustworthy AI systems.

**Key Principles:**
- **Transparency**
- **Accountability**
- **Reliability**
- **Fairness**
- **Privacy and Security**

**Why It Matters:**  
As AI becomes embedded in critical systems (healthcare, finance, hiring), ensuring safety, explainability, and ethical use is essential.

**Use Case:**  
A fintech startup uses the NIST AIF to assess its credit scoring AI for bias and security before launch.

---

### **NIST AI RMF (Risk Management Framework)**

**Definition:**  
A complementary framework to the NIST AIF, the AI RMF offers a structured approach to identifying and managing risks associated with AI technologies.

**Core Functions:**
1. **Map:** Understand context and intended use.
2. **Measure:** Assess risks to safety, fairness, etc.
3. **Manage:** Implement controls and safeguards.
4. **Govern:** Establish policies and accountability.

**Tip:**  
AI RMF helps bridge the gap between innovation and compliance, supporting responsible AI adoption.

---

### **NAT (Network Address Translation)**

**Definition:**  
NAT is a method that translates private IP addresses into a public IP address, allowing multiple devices on a local network to share a single public-facing IP.

**Why It’s Useful:**
- Conserves IPv4 addresses
- Adds a layer of obfuscation for internal devices
- Enables internet access from private networks

**Security Note:**  
While NAT hides internal IPs, it’s **not a security control**—combine it with firewalls and proper network segmentation.

---

## O-Z TODO
