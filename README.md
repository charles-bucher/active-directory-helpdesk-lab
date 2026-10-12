Active Directory Help Desk Lab

A self-directed IT support lab built with Windows Server, Active Directory Domain Services (AD DS), and Oracle VirtualBox.

The project simulates Tier 1 help desk scenarios involving account provisioning, password resets, account lockouts, authentication troubleshooting, network connectivity, email troubleshooting, printer support, and software installation.

Each completed incident is documented with troubleshooting steps, resolution notes, and supporting screenshots where available. The goal is to demonstrate practical IT support skills and a structured, evidence-based approach to problem solving.

Overview

This lab models common Tier 1 IT support workflows. Each incident is organized like a support ticket and may include:

User-reported issue

Investigation and diagnostic steps

Resolution actions

Verification of the outcome

Supporting screenshots

Incidents are marked as in progress or planned when the troubleshooting and evidence are not yet complete.

Lab Environment

Operating system: Windows Server 2022

Domain controller: DC01-NEW

Active Directory domain: corp.local

NetBIOS domain name: CORP

Virtualization: Oracle VirtualBox

Tools

Active Directory Users and Computers (ADUC)

Group Policy Management (GPMC)

Windows Command Prompt

Windows PowerShell

Windows Event Viewer

Network utilities such as ipconfig, ping, and nslookup

Repository Structure

helpdesk-lab/
├── incidents/
│   ├── 001-user-creation/
│   ├── 002-password-reset/
│   ├── 003-account-locked/
│   ├── 004-login-failure/
│   ├── 005-outlook-not-sending/
│   ├── 006-network-connectivity-issue/
│   ├── 007-printer-not-working/
│   └── 008-software-installation-failure/
├── screenshots/
└── notes/
