## Things I still mess up

09.04.2026:
  I need to really understand the difference between data custodian, steward, owner, controller...
  I still need to learn the ports on some of the protocols.
  I m doing much better with the Acronyms.
13.04.2026;
  I have zero problems with the acronyms. 
  I started watching cyberkraft PBQ and they look very nice. A lot more exciting than some basic theory questions.
  I m learning the ports, but I still mess them up sometimes.

Risk appetite = how much risk you want to take to chase goals
Risk tolerance = how much risk you can handle before it's too much
Risk acceptance = you know the risk exists and you say "fine, I'll take it" (yes/no decision for a specific risk)
Risk deterrence = taking actions to discourage threats from happening (like putting up cameras to scare off attackers)
Risk avoidance = eliminate the risk entirely by not doing the activity
Risk transference = shift the risk to someone else (buying insurance, outsourcing)
Risk mitigation = take steps to reduce the likelihood or impact of the risk
  
## nmap commands

## ports
20/21 - FTP - 20 for data, 21 for control
22 - SSH /SFTP
23 - Telnet
25 - SMTP
53 - DNS
67/68 - DHCP - 67 is server, 68 is client
80 - HTTP
88 - Keberos
110 - POP3
143 - IMAP
161/162 - SNMP - 161 for polling, 162 for traps
389 - LDAP (lightweight directory access protocol)
443 - HTTPS
500 - IPsec
587 - SMTPS
636- LDAPS
1433 - MSSQL (Microsoft sql server)
1812,1813 - RADIUS
3389 - RDP
5060 - SIP (Session initiating protocol)

## Hardware Security
- [ ] **TPM (Trusted Platform Module)** — Chip on Windows motherboards, stores keys/certificates/passwords
- [ ] **Secure Enclave** — Chip in Apple/Android devices, secures encryption keys only
- [ ] **HSM (Hardware Security Module)** — External physical device for managing digital keys, NOT embedded
- [ ] **UEFI (Unified Extensible Firmware Interface)** — Provides boot code for OS + enforces boot integrity checks
- [ ] **RoT (Hardware Root of Trust)** — Verifies boot signatures, does NOT provide boot code
## Cryptography
- [ ] **ECC (Elliptic Curve Cryptography)** — Asymmetric, short keys = same security as longer RSA keys
- [ ] **Diffie-Hellman** — Key EXCHANGE only, not encryption
- [ ] **DSA (Digital Signature Algorithm)** — Digital signatures only, not encryption
## Access Control
- [ ] **RBAC (Role-Based Access Control)** — Access based on role ONLY
- [ ] **ABAC (Attribute-Based Access Control)** — Access based on role + department + location + time + context
## Zero Trust
- [ ] **Policy Engine** — MAKES the access decision (the judge)
- [ ] **PEP (Policy Enforcement Point)** — ENFORCES the decision (the police)
- [ ] **Policy Administrator** — WRITES the policies (the lawmaker)
## Malware
- [ ] **Rootkit** — Hides from system tools, files mimic genuine executables
- [ ] **Spyware** — Browser redirects, webcam activation, DNS redirection, screenshots
- [ ] **RAT (Remote Access Trojan)** — Remote control access, but no DNS redirection
- [ ] **Virus** — Attaches to programs and spreads, doesn't hide processes
## DDoS Types
- [ ] **Reflected** — Responses redirected to victim's IP
- [ ] **Amplified** — Same as reflected BUT response is much larger than request
## DNS Attacks
- [ ] **Domain Hijacking** — Registration details changed, domain points elsewhere
- [ ] **DNS Poisoning** — DNS server records altered to redirect traffic
## Network Devices
- [ ] **Switch** — Layer 2, internal segmentation between departments
- [ ] **Router** — Layer 3, connects different networks (office to office)
- [ ] **Hub** — Layer 1, broadcasts everything, zero security
## Legislation
- [ ] **SOX (Sarbanes-Oxley Act)** — US corporate financial reporting transparency
- [ ] **Computer Security Act (1987)** — Federal agencies must secure confidential computer systems
- [ ] **FISMA (Federal Information Security Management Act)** — Broader federal information security management
- [ ] **GLBA (Gramm-Leach-Bliley Act)** — Financial sector customer data protection
- [ ] **GDPR (General Data Protection Regulation)** — EU personal data protection
## Standards
- [ ] **ISO/IEC 27001** — THE foundational ISMS framework
- [ ] **ISO/IEC 27002** — Guidance on ISMS controls, not the framework
- [ ] **ISO/IEC 27017** — 27001 extended for cloud
- [ ] **NIST SP 800-63** — US digital identity guidelines, not ISMS
## Governance
- [ ] **Committee** — Distributed decision-making across departments
- [ ] **Board** — Top-level oversight by directors
- [ ] **Stakeholders** — Representatives providing feedback from various departments
## Change Management
- [ ] **Approval Process** — Formalized review before implementation
- [ ] **Maintenance Window** — Scheduled time for changes
- [ ] **Backout Plan** — Revert plan if changes fail
## Security Awareness Phases
- [ ] **Development** — Creating new policies and procedures
- [ ] **Deployment** — Implementing existing strategies
- [ ] **Assessment** — Finding gaps in current protocols
- [ ] **Review** — Re-evaluating based on feedback
## Risk Documentation
- [ ] **Risk Report** — Summarized for executives, shows status and changes
- [ ] **Risk Register** — Ongoing tracker of all risks, not executive-facing
## Virtualization
- [ ] **VM Escape** — Breaking out of VM to host system
- [ ] **Best defense** — Patch the HYPERVISOR, not individual VMs
## Physical Security
- [ ] **Microwave Sensor** — Electromagnetic signals detecting movement
- [ ] **IR (Infrared) Sensor** — Heat/temperature changes detecting motion
## Data Protection
- [ ] **NDA (Non-Disclosure Agreement)** — Legally prevents unauthorized sharing of proprietary info
- [ ] **Misconfiguration** — Root cause of data disclosure (default passwords, open ports)
## Forensics
- [ ] **Timestamps** — Most valuable metadata when investigating leaked documents
- [ ] **Log Aggregation** — SIMPLIFIES log management, does NOT increase complexity
## Vulnerability Validation
- [ ] **Reviewing Event Logs** — Best method to confirm remediation worked
- [ ] **Rescanning** — Finds remaining vulnerabilities but no log insights
## Authentication
- [ ] **Passkey** — Public key crypto, unlock phone = prove identity, no password needed
## Networking
- [ ] **SDN (Software-Defined Networking)** — Separates control plane from data plane
## APIs
- [ ] **API (Application Programming Interface)** — Enables software interaction and automation, NOT for enhancing UI
## Web Security
- [ ] **WAF (Web Application Firewall)** — Protects web apps against SQLi and XSS specifically. Keywords: "HTTP application," "WordPress," "SQL injection," "cross-site scripting"
- [ ] **HIDS (Host-based IDS)** — Monitors a single host for suspicious activity, NOT designed for web application attacks specifically

## Virtualization vs Containerization
- [ ] **Virtualization** — Creates multiple ISOLATED ENVIRONMENTS (full OS) on a single physical device
- [ ] **Containerization** — Packages an APPLICATION and its dependencies, shares the host OS kernel, NOT full isolation

## CVSS Metrics
- [ ] **AV (Attack Vector)** — HOW the exploit reaches the target: network, adjacent, local, or physical
- [ ] **AC (Attack Complexity)** — How DIFFICULT it is to exploit, not the method of access
- [ ] **S (Scope)** — Whether the vulnerability impacts resources beyond its own security scope
- [ ] **UI (User Interaction)** — Whether a user must take action for the exploit to work

## Data Roles
- [ ] **Data Owner** — Determines data CLASSIFICATION and ensures alignment with organizational policies
- [ ] **Data Controller** — Defines purposes and means of data PROCESSING
- [ ] **Data Processor** — Processes data on behalf of the controller
- [ ] **Data Custodian** — Manages access and day-to-day handling of data

## Data Protection Techniques
- [ ] **Tokenization** — Substitutes sensitive data with non-sensitive TOKENS, both stored in a SEPARATE DATABASE. Keywords: "substitute," "non-sensitive representation," "separate database"
- [ ] **Obfuscation** — Makes data unclear/confusing but doesn't substitute with tokens in a separate database
- [ ] **Hashing** — One-way function producing fixed output, no way to retrieve original data

## Hardware Security (updated)
- [ ] **HSM** — EXTERNAL physical device for key storage. Keywords: "external system," "not embedded"
- [ ] **TPM** — EMBEDDED on Windows motherboards
- [ ] **Secure Enclave** — EMBEDDED in Apple/Android devices
- [ ] **Key Management System** — POLICY/PROCESS for managing keys, NOT a physical device

## Governance (updated)
- [ ] **Board** — EXTERNAL experienced individuals working with CEO to set policies. Keywords: "from outside the company," "works with CEO"
- [ ] **Committee** — INTERNAL employees from different departments making collaborative decisions. Keywords: "diverse groups of employees"

## Certificate Validation
- [ ] **OCSP (Online Certificate Status Protocol)** — QUICKEST way to check if a certificate has been revoked, real-time status
- [ ] **CRL (Certificate Revocation List)** — Published LIST of revoked certificates, must download and search, SLOWER than OCSP
- [ ] **CA (Certificate Authority)** — Issues and manages certificates, not for quick status checks




















## Concepts
ARCHITECTURE (3.1) — your biggest leak
Virtualization = multiple OS on one physical server, sharing resources. That's it.
SDN = separates network control plane from hardware. Key word: decouple.
Serverless = cloud provider manages infrastructure, you only write code. No servers to provision.
Microservices = app broken into small independent services. Not about hardware.
Containerization = packages app + its dependencies together. Not about network control.
RTOS = prioritizes performance over security features (like buffer overflow protection). That's the security risk.
ICS = biggest security concern is inability to patch (immutable components, can't take offline, proprietary/legacy systems).
Cloud = computing services delivered over the internet. On-prem and virtualization are NOT cloud.

RISK TERMS (5.2) — memorize these exactly
EF (Exposure Factor) = percentage of asset value lost in one incident
SLE = Asset Value × EF (cost of one incident)
ALE = SLE × ARO (yearly cost)
Likelihood = qualitative probability: low/medium/high
Risk Register = document that tracks risks, likelihood, impact, mitigation
Risk Appetite = how much risk the org is willing to take to pursue goals
Risk Tolerance = how much risk the org can withstand
Risk Acceptance = binary decision — you accept a specific risk or you don't

MALWARE DISTINCTIONS (2.4)
Rootkit = hides itself + gives attacker persistent admin-level access. If the scenario says "attacker gained admin privileges and is hidden" → rootkit.
Trojan = disguised as legit software, but does NOT give admin privileges.
Ransomware = encrypts data, demands payment. Never hides.
Worm = self-replicates across networks, no user interaction needed.

HARDWARE/MOBILE VULNERABILITIES (2.3)
Firmware vulnerability = attacker modifies device firmware (the software baked into hardware)
Sideloading = installing apps outside official app store
End-of-life = device no longer gets vendor updates/support
Legacy = device is outdated/obsolete but still in use

WEB ATTACKS (2.3)
SQLi = malicious SQL in input fields → attacker controls the database
XSS = malicious script injected into a web page → runs in victim's browser
CSRF = tricks authenticated user into performing unwanted action on a site they're logged into
Directory traversal = accesses files outside the intended web directory (../../etc/passwd)

SECURITY TOOLS — what makes each one unique (3.2 / 4.5)
IDS = detects and alerts. That's all. No blocking.
UTM = all-in-one security device but can cause latency.
SWG (Secure Web Gateway) = filters user web traffic + URL blacklists + DLP + CASB integrated.
NGFW = advanced firewall but not optimized for high-throughput user browsing.
Content filter = blocks URLs but no threat analysis.
DLP = prevents data leaving the org, not broad filtering.

IDENTITY & AUTH (4.6)
SSO = log in once, access multiple systems. Solves interoperability.
Physical security key = hardware token, plugs into USB.
Smart card = needs a card reader, may contain personal data.
Software token = virtual/digital, no physical device.

WIRELESS (4.1)
WPA3 uses Diffie-Hellman key agreement (replaced the WPA2 4-way handshake/PSK). Provides individualized encryption even on open networks.
EAP-TLS works with WPA3 but is not part of WPA3.

LOGS & METADATA (4.9)
Firewall logs contain: source IP, destination port, timestamps. NOT a list of open ports on the destination device.
File metadata contains: creator name, last modified date, file size. NOT which users accessed the file (but may include IP addresses that accessed it).

OTHER SINGLES
S/MIME = uses email certificates to sign + encrypt email content. TLS only encrypts the path, SPF checks sender IP, DMARC checks domain.
HMI (Human-Machine Interface) = where operators interact with ICS. That's the one you secure for operator access.
FDE (Full Disk Encryption) = protects data if physical server is stolen. RAID/clustering/deduplication don't encrypt.
Journaling = tracks all transactions continuously for recovery. Snapshots capture one moment, incremental backups save changes since last backup.
Tabletop exercise = discussion-based, no tech involved. If they're just talking through a scenario → tabletop.
Port 1433 = Microsoft SQL Server.
Web reputation score = evaluates site reliability/security risk. Not about popularity or SSL alone.
Agentless NAC = less granular data than agent-based. Supports more device types.
Capability (threat actor) = their skill in creating new exploits. Funding and resources are different.
Client-based software = installed on your machine, gets vendor updates directly. Attack vector if update process is compromised.
