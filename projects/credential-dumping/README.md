# Credential Dumping (Post-Exploitation)

This project demonstrates credential extraction from a compromised Windows system following successful privilege escalation.

---

## Objective

Extract stored credentials from a compromised system to simulate post-exploitation attacker behavior.

---

## Lab Environment

- Kali Linux attacker machine  
- Windows target system  
- Administrative access obtained  

---

## Overview

Following privilege escalation, credential dumping techniques were used to extract authentication data from the target system.

This represents a critical post-exploitation phase where attackers gain access to additional credentials that can be reused for lateral movement or further compromise.

---

## Technique Used

- Credential dumping using post-exploitation tools  
- Extraction of NTLM password hashes  

---

## Evidence

### Credential Dump Output
![Credential Dump](images/Secretsdump.png)

Credential data was successfully extracted from the system, including user accounts and NTLM password hashes.

---

## Key Findings

- Credential dumping is possible after privilege escalation  
- NTLM hashes can be reused in pass-the-hash attacks  
- Extracted credentials enable further lateral movement  

---

## Tools Used

- Impacket (secretsdump) / Mimikatz  
- Kali Linux  

---

## Skills Demonstrated

- Post-exploitation techniques  
- Credential extraction  
- Understanding of Windows authentication mechanisms  

---

## Impact

This project demonstrates how attackers can extract credentials from compromised systems, enabling further access, lateral movement, and potential full domain compromise.
