# Project 2 - Network Reconnaissance

## Active Directory Pentesting Lab  
Environment Build and Network Configuration  

---

## Objective

The purpose of this lab was to build a controlled Active Directory environment suitable for penetration testing practice and attack simulation.

The environment simulates a small enterprise domain with:
- One domain controller  
- Two domain-joined client machines  
- One attacker machine (Kali Linux)  

The lab is fully isolated from the internet except for the Kali machine, which maintains internet access for tool updates.

### Primary Objectives:
- Create a functional Active Directory domain  
- Establish internal-only communication  
- Provide controlled internet access for attacker machine  
- Support enumeration, credential attacks, privilege escalation, and lateral movement  

---

## Scope

This lab simulates an internal enterprise network containing an Active Directory domain.

All attacks originate from the Kali Linux attacker machine.

### Systems in Scope:
- **HYDRA-DC** – Domain Controller  
- **THEPUNISHER** – Workstation  
- **SPIDERMAN** – Workstation  

---

## Learning Objectives

- Network reconnaissance and host discovery  
- Service enumeration  
- Credential harvesting and password attacks  
- Lateral movement  
- Privilege escalation  

---

## Environment Components

| Role              | Hostname      | Operating System        |
|------------------|--------------|------------------------|
| Attacker         | Kali         | Kali Linux             |
| Domain Controller| HYDRA-DC     | Windows Server         |
| Workstation      | THEPUNISHER  | Windows 10 Enterprise  |
| Workstation      | SPIDERMAN    | Windows 10 Enterprise  |

**Domain:** MARVEL.local  

---

## Network Design

Two VMware networks are used:

### VMnet1 (Host-Only)
- Subnet: 192.168.208.0 / 24  
- Internal lab communication only  

### VMnet8 (NAT)
- Used only by Kali Linux  
- Provides internet access  

---

## IP Addressing

| System        | IP Address        |
|--------------|------------------|
| HYDRA-DC     | 192.168.208.130  |
| THEPUNISHER  | 192.168.208.128  |
| SPIDERMAN    | 192.168.208.129  |
| Kali (eth1)  | 192.168.208.131  |

- Subnet Mask: 255.255.255.0  
- DNS: 192.168.208.130  
- No default gateway on domain systems (intentional isolation)  

---

## Issues Encountered

### Duplicate IP Conflict
- Kali was assigned the same IP as HYDRA-DC  
- Domain controller lost connectivity (APIPA address assigned)  
- Fixed by correcting IP configuration  

### Windows Adapter Issue
- Workstation not responding to ping  
- Fixed by disabling/re-enabling network adapter  

### VMware Network Mismatch
- Systems were on different virtual networks  
- Fixed by aligning all to VMnet1  

---

## Network Topology

![Network Topology](./images/network_topology.png)

---

## Final Status

The lab is now fully operational.

- All systems communicate internally  
- Kali has internet access via NAT  
- Environment is ready for:

- Network enumeration  
- Service discovery  
- Credential attacks  
- Lateral movement  
- Privilege escalation 
