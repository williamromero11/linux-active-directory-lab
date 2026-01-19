# Linux Active Directory Domain Controller with Samba & Kerberos

A complete Linux-based Active Directory environment implemented using Samba AD, Kerberos, and Ubuntu Server for identity and access management.

## 🎯 Project Overview
A complete enterprise-level identity management system built on Linux using Samba 4 as an Active Directory domain controller. This project demonstrates setting up a Windows-compatible directory service in a Linux environment with Kerberos authentication, DNS, NTP, and file sharing services.

## 📋 Architecture

```
                    ┌─────────────────────────────────────┐
                    │         SVN.COM Domain              │
                    │        192.168.0.0/24 Network       │
                    └──────────────────┬──────────────────┘
                                       │
                    ┌──────────────────┼──────────────────┐
                    │                  │                  │
           ┌────────▼────────┐ ┌──────▼──────┐ ┌─────────▼────────┐
           │   DC1           │ │    CS1      │ │       CS2        │
           │ 192.168.0.101   │ │192.168.0.102│ │   192.168.0.103  │
           ├─────────────────┤ ├─────────────┤ ├──────────────────┤
           │ • Samba AD DC   │ │ • Domain    │ │ • Domain Joined  │
           │ • Kerberos KDC  │ │   Joined    │ │ • SSSD Configured│
           │ • DNS Server    │ │ • SSSD Auth │ │ • Kerberos Client│
           │ • NTP Server    │ │ • Kerberos  │ └──────────────────┘
           └─────────────────┘ │   Client    │
                               └─────────────┘
```
## 🛠️ Technologies Used
- Ubuntu Server 24.04 - Base operating system
- Samba 4 - Active Directory Domain Services
- Kerberos 5 - Network authentication protocol
- SSSD - System Security Services Daemon
- Chrony - NTP time synchronization
- Bash/PowerShell - Automation and scripting
- VirtualBox - Virtualization platform
- SSH - Secure remote administration

## 📸 Project Evidence

[PDF 1](screenshots/1.pdf) – Samba AD DC Setup  
