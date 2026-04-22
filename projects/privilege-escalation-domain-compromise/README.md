# Privilege Escalation & Domain Compromise

## Objective
Escalate privileges within a compromised environment and obtain domain-level access using credential extraction and post-exploitation techniques.

## Lab Environment
- Kali Linux attacker machine
- Windows Domain environment
- Domain-joined systems
- Compromised Administrator credentials

## Overview
Following successful lateral movement, additional techniques were used to extract credentials and escalate privileges, ultimately leading to domain-level compromise.

## Attack Workflow
- Initial access and lateral movement completed
- Credentials harvested from compromised systems
- Privilege escalation techniques executed
- Domain-level access achieved

## Techniques Used
- Credential dumping
- Privilege escalation
- Token/credential abuse

## Evidence

### Credential Dumping / Privilege Escalation
![Privilege Escalation](images/priv_esc.png)

Compromised credentials were extracted from memory and reused to escalate privileges, enabling full control over domain resources.

## Key Findings
- Credential storage in memory presents a major risk
- Privilege escalation can occur without exploits
- Domain compromise can follow quickly after initial access

## Tools Used
- Mimikatz / alternative
- NetExec (nxc)
- Kali Linux

## Skills Demonstrated
- Privilege escalation
- Credential extraction
- Post-exploitation
- Domain compromise techniques

## Impact
Privilege escalation enabled full domain compromise, demonstrating how attackers can gain complete control of an environment once initial access is obtained.
