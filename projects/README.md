# Cybersecurity Projects Portfolio
A collection of hands-on offensive security projects demonstrating initial access, post-exploitation, privilege escalation, network penetration testing, and supporting detection analysis.
Each project simulates real-world attack scenarios and includes methodology, tools used, and detection insights.
---
## Attack Detection with Elastic SIEM
Detection of authentication-based attacks using Windows Security Logs and Elastic SIEM.
**Focus:**
- Event ID 4776 analysis (Credential Validation)
- Failed authentication detection
- User enumeration identification
**Techniques Demonstrated:**
- Brute force detection
- Credential spraying analysis
- Log correlation in SIEM
 [View Project](./attack-detection-elastic)
---
## SMB Brute Force Attack – Initial Access
Simulated brute force attack against SMB services to gain unauthorized access.
**Focus:**
- SMB enumeration
- Password brute forcing
- Initial access techniques
**Tools Used:**
- Hydra
- Nmap
- SMB enumeration tools
 [View Project](./smb-brute-force-attack)
---
## Suspicious Logon Detection
Analysis of abnormal login patterns and suspicious authentication behavior.
**Focus:**
- Logon Type analysis (Event ID 4624)
- Detection of unusual login activity
- Behavioral analysis of authentication logs
 [View Project](./suspicious-logon-detection)
---
## Lateral Movement Simulation
Simulation of attacker movement across systems after initial compromise.
**Focus:**
- Internal network movement
- Credential reuse
- Post-exploitation techniques
 [View Project](./lateral-movement-simulation)
---
## Privilege Escalation – Domain Compromise
Demonstration of privilege escalation techniques leading to domain-level access.
**Focus:**
- Privilege escalation methods
- Domain compromise techniques
- Attack chain progression
 [View Project](./privilege-escalation-domain-compromise)
---
## Credential Dumping – Pass-the-Hash
Post-exploitation credential extraction and lateral movement using Pass-the-Hash.
**Focus:**
- Credential dumping with Mimikatz
- Pass-the-Hash authentication with Impacket
- SYSTEM-level remote access
- Detection validation in Elastic
 [View Project](./credential-dumping)
---
## AD Attack Path Analysis – BloodHound
Active Directory attack path analysis using BloodHound to map misconfigurations and identify privilege escalation paths to Domain Admin.
**Focus:**
- Active Directory data collection with SharpHound
- Graph-based attack path analysis with BloodHound
- ADCS escalation path identification (ESC1 + ESC4)
- DCSync rights enumeration
- Correlation of attack paths with real-world exploitation
**Tools Used:**
- BloodHound Community Edition
- SharpHound
- Kali Linux
 [View Project](./ad-attack-path-bloodhound)
---
## Home Network Penetration Test
Full penetration test against a real home network environment using Kali Linux 2025.4. Enumerated services, identified vulnerabilities including an exposed UPnP service running MiniUPnP 1.8 and outdated SSH (Dropbear 2019.78), and applied full remediation across two routers.
**Focus:**
- Network scanning and host discovery
- Service enumeration and version analysis
- CVE research and vulnerability identification
- Router hardening and firmware management
- Remediation verification
**Tools Used:**
- Nmap 7.98
- Searchsploit
- Kali Linux 2025.4
- TP-Link Tether
 [View Project](./home-network-penetration-test)
---
## Core Skills Demonstrated
- SIEM log analysis (Elastic)
- Windows Event Log investigation
- Brute force & credential attack detection
- Network enumeration & exploitation
- Attack pattern recognition
- Security monitoring & detection engineering
- Active Directory attack path analysis
- ADCS vulnerability identification
- DCSync rights enumeration
- Network penetration testing
- Router hardening and remediation
---
## Notes
These projects are part of a structured offensive security learning path, covering:
1. Reconnaissance
2. Enumeration
3. Initial Access
4. Post-Exploitation
5. Detection & Analysis
6. Attack Path Analysis
7. Network Security Assessment
Each project builds on the previous to simulate real-world attack workflows.
---
