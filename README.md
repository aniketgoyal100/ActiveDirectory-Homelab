# Active Directory Homelab (Azure Virtual Environment)

## Overview
This project simulates a real-world enterprise IT environment using Microsoft Azure, Windows Server 2022 Datacenter (Azure Edition), and Windows 10 virtual machines. The lab demonstrates domain configuration, DNS and DHCP setup, user management, and Group Policy administration within a secure, cloud-hosted virtual network.

## Technologies Used
- Microsoft Azure Virtual Machines  
- Windows Server 2022 Datacenter (Azure Edition)  
- Windows 10 (Client)  
- Active Directory Domain Services (AD DS)  
- DNS and DHCP Configuration  
- Group Policy Management Console (GPMC)  
- PowerShell  

## Network Architecture
| Component | Role | IP Address | Notes |
|------------|------|-------------|--------|
| DC1 | Domain Controller, DNS, DHCP | 172.16.0.4 | lab.local domain |
| Client1 | Domain-Joined Windows 10 | 172.16.0.5 | Joined to lab.local |
| Azure VNet | Handles NAT and private subnet | 172.16.0.0/24 | Cloud-managed |

## Key Features
- Configured Active Directory domain: lab.local  
- Created OUs for Admins, Staff, and Students  
- Set up DNS and DHCP for domain name resolution and IP leasing  
- Joined a Windows 10 client to the domain  
- Applied a Group Policy Object (GPO) to enforce a mandatory wallpaper  
- Verified RDP access for all domain users  

## Screenshots

- Active Directory Users and Computers (OUs and accounts)  
- Client1 joined to lab.local  
- Successful RDP login as lab\jdoe  
- Group Policy wallpaper applied  

## Outcome
This homelab successfully simulates a managed IT infrastructure where domain users and systems are controlled through centralized policies and services. The setup demonstrates core enterprise administration skills, including Active Directory, DHCP, DNS, and Group Policy management.

[Detailed Setup Guide (Coming Soon)](./DetailedSetup.md)
