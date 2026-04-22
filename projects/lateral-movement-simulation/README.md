# Lateral Movement Simulation

This project simulates lateral movement within a compromised network using valid credentials obtained during an initial access attack.

## Objective
Simulate lateral movement using compromised credentials to access additional systems within the network.

## Lab Environment
- Kali Linux attacker machine  
- Windows systems  
- SMB services enabled  

## Overview
Following initial access via SMB brute force, valid credentials were used to move laterally across the network and access additional systems.

## Attack Workflow
- Initial access obtained via SMB brute force  
- Valid credentials identified  
- Credentials reused to authenticate to another system  
- Successful access to additional resources achieved  

## Lateral Movement Techniques
- SMB authentication  
- Remote command execution  
- Credential reuse  

## Evidence

(Add screenshots here)

## Key Findings
- Credential reuse enables rapid network compromise  
- Lateral movement does not always require exploits  
- Valid accounts are one of the most powerful attacker tools  

## Tools Used
- SMB tools  
- PsExec / WMIC (if used)  
- Kali Linux  

## Skills Demonstrated
- Post-exploitation techniques  
- Lateral movement  
- Credential abuse  
- Network navigation  

## Impact
Compromised credentials enabled movement across systems, demonstrating how a single point of failure can lead to broader network compromise.
