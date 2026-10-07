# GLPI Help Desk Home Lab

## Overview

This project documents my hands-on IT help desk home lab built to develop practical experience with ticket management, Windows troubleshooting, networking, asset management, and technical documentation.

The environment simulates a small business where users submit IT support tickets through GLPI and a help desk technician investigates, documents, and resolves the incidents.

## Lab Environment

- ZimaOS virtualization host
- Ubuntu Server VM
- GLPI help desk platform
- Windows 11 Pro workstation
- GLPI Agent
- Simulated employee and technician accounts

## Lab Architecture

## Lab Architecture

```text
ZimaOS
├── Ubuntu Server VM
│   └── GLPI Server
│
└── Windows 11 Pro VM
    ├── GLPI Agent
    └── Simulated Employee Workstation
```

## Skills Practiced

- Help desk ticket management
- Windows 11 troubleshooting
- TCP/IP networking
- DNS troubleshooting
- IT asset management
- GLPI administration
- Incident documentation
- Troubleshooting methodology

## Help Desk Tickets

### Ticket 01 - DNS Resolution Failure

**Issue:** User was unable to access websites from a Windows 11 workstation.

**Diagnosis:** External IP connectivity was functional, but DNS name resolution was failing.

**Resolution:** Isolated the issue to the workstation's DNS configuration, configured a functioning DNS server, flushed the DNS resolver cache, and verified successful hostname resolution.

[View Ticket 01 Documentation](Ticket-01-DNS-Resolution/README.md)

---

More troubleshooting scenarios will be added as the lab develops.
