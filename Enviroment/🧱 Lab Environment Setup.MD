🧱 Lab Environment Setup
Overview

This document outlines the configuration of the Active Directory lab environment used to simulate Tier 1 Help Desk scenarios including user management, authentication troubleshooting, and account security operations.

🖥️ Virtual Infrastructure
Hypervisor
Oracle VirtualBox (or VMware Workstation Player)
🧠 Virtual Machines
1. Domain Controller (DC01)
OS: Windows Server 2019 / 2022
Role: Active Directory Domain Services (AD DS)
Domain Name: corp.local
Services Installed:
Active Directory Domain Services
DNS Server
Static IP: Configured (required for domain controller stability)
2. Client Workstation (WIN10-CLIENT)
OS: Windows 10 or Windows 11
Role: Domain-joined user workstation
Joined to: corp.local
Used for:
Login testing
Authentication troubleshooting
User experience simulation
🌐 Network Configuration
Network Mode: Internal Network / Host-only Adapter (depending on setup)
Domain Communication: Enabled between DC01 and client VM
DNS: Pointed to Domain Controller IP (DC01)
🏗️ Active Directory Configuration
Domain Setup
Forest: corp.local
Domain Controller: DC01
Organizational Structure (example):
corp.local
└── Users
    ├── IT
    ├── Finance
    ├── HR
    └── Standard Users
User Accounts (Lab Examples)
jdoe (used across all incident simulations)
Additional test users created as needed for scenarios
Group Policy (GPO)

Configured policies include:

Password complexity enforcement
Account lockout policy:
5 invalid attempts
15-minute lockout duration
Password expiration rules
⚙️ Tools Used
Active Directory Users and Computers (ADUC)
Windows Server Manager
Command Line (ipconfig, ping for testing connectivity)
Event Viewer (optional troubleshooting expansion)
🧪 Lab Purpose

This environment is designed to simulate real-world Tier 1 Help Desk responsibilities, including:

User account creation and management
Password reset workflows
Account lockout resolution
Login troubleshooting
Active Directory navigation and verification
🎯 Skills Practiced
Active Directory administration fundamentals
Windows Server domain services
Authentication and identity troubleshooting
IT ticket-style documentation
Basic network/domain connectivity validation
🧠 Notes
All configurations are isolated within a virtual environment
No production systems are used
Scenarios are designed to reflect real help desk workflows
Environment is reusable for expanding additional incident scenarios (Tier 2 escalation simulations, GPO issues, DNS troubleshooting, etc.)