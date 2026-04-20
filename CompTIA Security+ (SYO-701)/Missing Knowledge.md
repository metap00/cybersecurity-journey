## Things I still mess up

09.04.2026:
  I need to really understand the difference between data custodian, steward, owner, controller...
  I still need to learn the ports on some of the protocols.
  I m doing much better with the Acronyms.
13.04.2026;
  I have zero problems with the acronyms. 
  I started watching cyberkraft PBQ and they look very nice. A lot more exciting than some basic theory questions.
  I m learning the ports, but I still mess them up sometimes.
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
