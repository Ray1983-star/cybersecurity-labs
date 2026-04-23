# Cybersecurity Portfolio – Offensive Security Labs

Hands-on offensive security labs focused on initial access, lateral movement, privilege escalation, attack detection, and Active Directory attack path analysis.

---

## About

This repository documents my practical cybersecurity work, focused on offensive security and penetration testing.

The projects simulate real-world attack scenarios across the offensive lifecycle, from reconnaissance and initial access through to lateral movement, privilege escalation, domain compromise, and attack path analysis.

---

## 📁 Projects Portfolio

👉 [View All Projects](./projects)

---

## Featured Projects

### 🩸 AD Attack Path Analysis – BloodHound

Used BloodHound to map the MARVEL.LOCAL Active Directory environment and identify hidden attack paths to Domain Admin. Findings directly correlated with attacks performed across the full project series.

**Key skills:**
- Active Directory attack path analysis
- ADCS escalation path identification (ESC1 + ESC4)
- DCSync rights enumeration
- Offensive and defensive security reasoning

➡️ [View Project](./projects/ad-attack-path-bloodhound)

---

### 🗝️ Credential Access & Pass-the-Hash Detection

Extracted credentials from memory using Mimikatz, performed lateral movement via Pass-the-Hash using Impacket, and validated detection using Elastic SIEM.

**Key skills:**
- Credential dumping
- Pass-the-Hash lateral movement
- SYSTEM-level remote execution
- SIEM detection validation

➡️ [View Project](./projects/credential-dumping)

---

### 🔴 SMB Brute Force Attack – Initial Access

Simulated a real-world attack where weak SMB credentials were exploited to gain unauthorized access to a target system.

**Key skills:**
- Service enumeration
- Credential brute forcing
- Initial access techniques

➡️ [View Project](./projects/smb-brute-force-attack)

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

➡️ [View Labs](./labs)

---

## Focus Areas

- Penetration Testing
- Active Directory Security
- Network Enumeration
- Privilege Escalation
- Lateral Movement
- Attack Path Analysis
- Security Detection & Log Analysis
