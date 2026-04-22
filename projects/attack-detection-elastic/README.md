# Attack Detection with Elastic SIEM

This project focuses on detecting attacker activity within a compromised Active Directory environment using Elastic SIEM. It highlights how authentication logs can be used to identify brute force attempts and credential abuse.

---

## Objective

Identify and analyze suspicious authentication activity using centralized logging and SIEM-based detection.

---

## Lab Environment

- Kali Linux attacker machine  
- Windows Active Directory environment  
- Elastic Stack (SIEM)  
- Winlogbeat for log ingestion  

---

## Overview

Following an initial SMB brute force attack, authentication events were generated on the domain controller. These logs were ingested into Elastic SIEM, where they were analyzed to detect patterns of abnormal login activity.

This project demonstrates how attacker behavior leaves identifiable traces within system logs, and how those traces can be leveraged for detection.

---

## Detection Strategy

The detection focused on identifying high volumes of credential validation events within a short time frame.

Key indicators:
- Repeated authentication attempts  
- High frequency of Event ID 4776  
- Consistent source host generating login requests  

These patterns are commonly associated with:
- Brute force attacks  
- Credential spraying  
- Unauthorized authentication attempts  

---

## Evidence

### Credential Validation Activity (Event ID 4776)
![Credential Validation Logs](images/credential_validation.png)

A spike in credential validation events (Event ID 4776) was observed in Elastic SIEM, indicating abnormal authentication activity originating from a single source. The volume and frequency of these events are consistent with brute force or credential spraying attempts, demonstrating how authentication attacks can be identified through SIEM log analysis.

---

## Key Findings

- Authentication logs provide strong indicators of attack activity  
- Brute force attacks generate detectable patterns in SIEM  
- High-frequency login attempts are a reliable detection signal  
- Centralized logging enables visibility across the environment  

---

## Tools Used

- Elastic SIEM  
- Winlogbeat  
- Windows Security Logs  

---

## Skills Demonstrated

- SIEM log analysis  
- Threat detection and pattern recognition  
- Windows event log analysis  
- Understanding of authentication-based attacks  

---

## Impact

This project demonstrates how authentication attacks can be detected through log analysis, highlighting the importance of monitoring and correlating security events to identify malicious activity early.
