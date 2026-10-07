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
- Windows user account administration
- Password reset and authentication troubleshooting
- Least-privilege access management

## Help Desk Tickets

### Ticket 01 - DNS Resolution Failure

**Issue:** User was unable to access websites from a Windows 11 workstation.

**Diagnosis:** External IP connectivity was functional, but DNS name resolution was failing.

**Resolution:** Isolated the issue to the workstation's DNS configuration, configured a functioning DNS server, flushed the DNS resolver cache, and verified successful hostname resolution.

[View Ticket 01 Documentation](Ticket-01-DNS-Resolution/README.md)

### Ticket 02 - Application Installation & User Permissions

**Issue:** User was unable to install 7-Zip because the standard Windows account did not have administrative privileges.

**Diagnosis:** Reproduced the issue and verified that Windows User Account Control (UAC) required IT administrator credentials for the system-level installation.

**Resolution:** Authorized and installed 7-Zip using the dedicated IT administrator account, verified the application launched successfully, and maintained the user's standard account permissions in accordance with least-privilege practices.

[View Ticket 02 Documentation](Ticket-02-Application-Installation/README.md)

### Ticket 03 - Windows Password Reset

**Issue:** User was unable to sign in to workstation ACME-PC-001 due to an incorrect password.

**Diagnosis:** Verified the local Windows user account was active, enabled, and not locked out. The issue was isolated to the user's authentication credentials.

**Resolution:** Reset the user's password using an authorized IT administrator account and verified successful Windows authentication while maintaining the user's standard account permissions.

[View Ticket 03 Documentation](Ticket-03-Password-Reset/README.md)

---

More troubleshooting scenarios will be added as the lab develops.
