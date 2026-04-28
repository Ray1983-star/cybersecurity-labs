# Home Network Penetration Test

Full penetration test against a real home network environment using Kali Linux 2025.4. Enumerated services, identified vulnerabilities, and applied full remediation across two routers.

---

## Objective

Conduct a full penetration test against a home network environment — enumerating services, identifying vulnerabilities, and applying remediations — simulating a real-world network security audit.

---

## Summary

Performed reconnaissance, port scanning, and service enumeration against a home router running outdated firmware. Identified multiple medium-severity vulnerabilities including an exposed UPnP service running MiniUPnP 1.8 (2014) and an outdated SSH daemon (Dropbear 2019.78). Applied full remediation including firmware update, service hardening, and credential hygiene across two routers.

---

## Key Findings

| Severity | Finding | Port |
|---|---|---|
| Medium | UPnP enabled — MiniUPnP 1.8 (known CVEs) | 1900/tcp |
| Medium | Outdated SSH — Dropbear 2019.78 | 20001/tcp |
| Low | Self-signed SSL certificate | 443/tcp |
| Low | Outdated firmware — BusyBox, dnsmasq | — |
| Positive | Account lockout working | — |
| Positive | Admin restricted to LAN only | — |

---

## Remediation

- ✅ Firmware updated (1.3.10 → 1.3.12)
- ✅ UPnP disabled
- ✅ SSH disabled
- ✅ HTTPS enforced for admin access
- ✅ Default WiFi credentials changed
- ✅ Auto-update enabled on both routers
- ✅ Remote management confirmed off

---

## Tools Used

- Nmap 7.98
- Searchsploit
- Kali Linux 2025.4
- TP-Link Tether

---

## Skills Demonstrated

`Network Scanning` `Service Enumeration` `CVE Research` `Router Hardening` `Firmware Management` `Remediation Verification`

---

📁 [View Full Lab Writeup](../../labs/Project-12-Home-Network-Pentest)

