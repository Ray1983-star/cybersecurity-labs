# Cybersecurity Portfolio – Offensive Security Labs
Hands-on offensive security labs focused on initial access, lateral movement, privilege escalation, attack detection, Active Directory attack path analysis, and network penetration testing.
---
## About
This repository documents my practical cybersecurity work, focused on offensive security and penetration testing.
The projects simulate real-world attack scenarios across the offensive lifecycle, from reconnaissance and initial access through to lateral movement, privilege escalation, domain compromise, attack path analysis, and network security assessments.
---
## Projects Portfolio
 [View All Projects](./projects)
---
## Featured Projects
### AD Attack Path Analysis – BloodHound
Used BloodHound to map the MARVEL.LOCAL Active Directory environment and identify hidden attack paths to Domain Admin. Findings directly correlated with attacks performed across the full project series.
**Key skills:**
- Active Directory attack path analysis
- ADCS escalation path identification (ESC1 + ESC4)
- DCSync rights enumeration
- Offensive and defensive security reasoning

 [View Project](./projects/ad-attack-path-bloodhound)
---
### Credential Access & Pass-the-Hash Detection
Extracted credentials from memory using Mimikatz, performed lateral movement via Pass-the-Hash using Impacket, and validated detection using Elastic SIEM.
**Key skills:**
- Credential dumping
- Pass-the-Hash lateral movement
- SYSTEM-level remote execution
- SIEM detection validation

 [View Project](./projects/credential-dumping)
---
### Home Network Penetration Test
Full penetration test against a real home network environment. Enumerated services, identified vulnerabilities including an exposed UPnP service running MiniUPnP 1.8 and outdated SSH (Dropbear 2019.78), and applied full remediation across two routers.
**Key skills:**
- Network scanning and service enumeration
- CVE research and vulnerability analysis
- Router hardening and firmware management
- Remediation verification

 [View Project](./projects/Home-Network-Penetration-Test)
---
### SMB Brute Force Attack – Initial Access
Simulated a real-world attack where weak SMB credentials were exploited to gain unauthorized access to a target system.
**Key skills:**
- Service enumeration
- Credential brute forcing
- Initial access techniques

 [View Project](./projects/smb-brute-force-attack)
---
## Lab Environment
- Kali Linux
- Windows Server 2016 (Domain Controller)
- Windows 10 (Domain-joined workstations)
- Elastic Stack (SIEM)
- Domain: MARVEL.LOCAL
---
## Tools & Technologies
- Nmap
- Hydra
- NetExec
- Impacket
- Mimikatz
- BloodHound / SharpHound
- Elastic Stack / Kibana
- Hashcat
---
## Additional Labs
All foundational labs and step-by-step exercises are available in the `/labs` directory.
 [View Labs](./labs)
---
## Focus Areas
- Penetration Testing
- Active Directory Security
- Network Enumeration
- Privilege Escalation
- Lateral Movement
- Attack Path Analysis
- Network Security Assessment
- Security Detection & Log Analysis
