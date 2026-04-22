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
- Credentials reused to authenticate to additional systems  
- Remote execution performed across multiple hosts  

## Lateral Movement Techniques
- SMB authentication  
- Remote command execution  
- Credential reuse  

## Evidence

### Remote Execution Using Compromised Credentials
![Remote Execution](images/remote_execution.png)

Compromised Administrator credentials were reused to authenticate across multiple systems, successfully executing remote actions and confirming lateral movement within the network.

## Key Findings
- Credential reuse enables rapid network compromise  
- Lateral movement does not always require exploits  
- Valid accounts are one of the most powerful attacker tools  

## Tools Used
- NetExec (nxc)  
- SMB tools  
- Kali Linux  

## Skills Demonstrated
- Post-exploitation techniques  
- Lateral movement  
- Credential abuse  
- Remote execution  

## Impact
Compromised credentials enabled movement across multiple systems, demonstrating how a single point of failure can lead to widespread network compromise.
