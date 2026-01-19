# Linux Active Directory Domain Controller with Samba & Kerberos

A complete Linux-based Active Directory environment implemented using Samba AD, Kerberos, and Ubuntu Server for identity and access management.

## 🎯 Project Overview
Deployed and configured a fully functional Active Directory domain controller with two client servers to demonstrate enterprise-level identity management in a Linux environment.

## 📋 Architecture

**DC1 (Domain Controller)** - `192.168.0.101`
- Samba AD Domain Controller
- Kerberos KDC
- Internal DNS Server
- NTP Server with AD integration

**CS1 (Client Server 1)** - `192.168.0.102`
- Joined to SVN.COM domain
- SSSD for authentication
- Kerberos client

**CS2 (Client Server 2)** - `192.168.0.103`
- Joined to SVN.COM domain
- SSSD for authentication
- Kerberos client
