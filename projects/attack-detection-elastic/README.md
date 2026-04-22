# Attack Detection & Log Analysis (Elastic SIEM)

## Objective
Detect attacker activity within a compromised environment using Windows Security logs and Elastic SIEM, focusing on authentication abuse, lateral movement, and privilege escalation.

## Lab Environment
- Windows Domain Controller (HYDRA-DC)
- Windows target systems
- Kali Linux attacker machine
- Elastic Stack (Elasticsearch, Kibana, Winlogbeat)

## Overview
Following a simulated attack involving SMB brute force, credential reuse, and privilege escalation, log data was analyzed in Elastic SIEM to identify indicators of compromise and detect attacker behavior across the network.

## Detection Strategy
Detection focused on identifying abnormal authentication patterns and suspicious account activity using Windows Event Logs.

### Key Events Monitored
- **4624** – Successful logon
- **4625** – Failed logon (brute force attempts)
- **4672** – Special privileges assigned (Administrator login)
- **4776** – Credential validation events

## Attack Detection Workflow
- Identified multiple failed login attempts (brute force activity)
- Detected successful authentication following failures
- Observed repeated logins across multiple hosts
- Detected privileged account usage
- Correlated events to confirm lateral movement and escalation

## Evidence

### Brute Force & Authentication Activity (Event ID 4776)
![Authentication Logs](images/authentication.png)

Multiple credential validation attempts were observed, indicating repeated authentication attempts consistent with brute force activity.

### Successful Logon & Lateral Movement (Event ID 4624)
![Successful Logon](images/logon.png)

Successful logins from the same account across multiple systems confirmed lateral movement using compromised credentials.

### Privileged Access Detection (Event ID 4672)
![Privilege Escalation](images/privileges.png)

Special privileges assigned to the account indicate administrative access, confirming privilege escalation within the environment.

## Key Findings
- Brute force activity is visible through repeated authentication failures
- Successful login patterns following failures indicate credential compromise
- Lateral movement can be identified through logins across multiple hosts
- Privileged logins provide strong indicators of escalation
- Correlating multiple event types is critical for accurate detection

## Tools Used
- Elastic SIEM (Kibana)
- Winlogbeat
- Windows Event Logs

## Skills Demonstrated
- SIEM log analysis
- Threat detection
- Event correlation
- Identification of attack patterns
- Blue team investigation techniques

## Impact
Attack activity was successfully detected and reconstructed using log data, demonstrating how SIEM solutions can identify and track attacker behavior from initial access through to privilege escalation.
