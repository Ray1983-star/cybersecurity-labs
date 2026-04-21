# SMB Brute Force Attack – Initial Access

## Objective
Simulate an SMB brute force attack to gain initial access to a target system.

## Lab Environment
- Kali Linux attacker machine
- Windows target host
- SMB service exposed on the target

## Attack Overview
This project demonstrates how exposed SMB services and weak credentials can be used to gain unauthorized access to a system.

## Reconnaissance
Identified SMB service running on the target using network scanning.

## Enumeration
Enumerated SMB to identify access points and prepare for authentication attacks.

## Exploitation
Executed a brute force attack against SMB authentication and obtained valid credentials, allowing access to the system.

## Evidence
(Add screenshots here)

## Key Findings
- Weak passwords can lead directly to system compromise
- SMB is a high-value target in internal environments

## Tools Used
- Nmap
- Hydra
- SMB tools
