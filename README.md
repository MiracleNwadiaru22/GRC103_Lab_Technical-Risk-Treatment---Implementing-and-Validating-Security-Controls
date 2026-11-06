## Overview
This project demonstrates the implementation and validation of technical security controls for a fictional organisation, **Northbridge Services**, as part of the GRC 103 Practical Laboratory at the International Cybersecurity and Digital Forensics Academy (ICDFA).

The exercise focused on identifying and treating four risks affecting an internal document server.

## Lab Environment
- **Server:** Ubuntu Server 24.04 LTS
- **Testing machine:** Kali Linux
- **Web server:** Nginx
- **Firewall:** UFW
- **Network:** Isolated Host-only network

## Risk Treatment Activities

| Risk | Treatment | Validation |
|---|---|---|
| Unnecessary legacy service | Avoidance – disabled service on port 8080 | Service inactive; port initially reported closed |
| Exposed archive files | Mitigation – moved archive outside web root and restricted access | HTTP 403 for archive requests |
| Unauthorised network access | Mitigation – configured UFW firewall rules | Authorised access returned HTTP 200; unauthorised source was blocked |
| Loss of portal content | Mitigation – backup and recovery | Successful restoration and SHA-256 checksum verification |

## Key Results
- Retired the unnecessary legacy service.
- Restricted access to sensitive archive files.
- Configured firewall rules to permit HTTP access only from an authorised source.
- Reviewed Nginx and UFW logs.
- Successfully restored portal content from backup.
- Recorded an observed recovery time of **11 minutes and 37 seconds**.
- Assessed residual risks and considered risk transfer, acceptance and treatment costs.

## Tools and Technologies
`Kali Linux` · `Ubuntu Server` · `Nmap` · `Nginx` · `UFW` · `systemd` · `curl` · `SHA-256` · `Linux CLI`

## Evidence
The project evidence includes:
- Configuration files
- Network and HTTP test outputs
- Firewall and web-server logs
- Recovery and checksum evidence
- Lab screenshots
- Risk assessment and cost analysis

## Key Learning
This exercise strengthened my practical understanding of technical risk treatment, security control implementation, vulnerability validation, access restriction, backup and recovery, log review, and residual risk assessment.

**Note:** This was an authorised, simulated lab conducted in an isolated virtual environment using dummy data.
