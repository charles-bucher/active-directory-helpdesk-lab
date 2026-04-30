# Active Directory Help Desk Lab

Simulated IT help desk environment built using Windows Server and Active Directory.

This project replicates real-world Tier 1 IT support operations including user provisioning, authentication troubleshooting, network diagnostics, email issues, printing problems, and software installation support.

Each scenario is documented as a ticket-style incident with investigation steps, resolution actions, and verification results to reflect real support workflows.

---

## 🧠 Overview

This lab simulates daily responsibilities of a Tier 1 Help Desk Technician in an enterprise environment.

Each incident is structured as a real support ticket:

* User-reported issue
* Investigation and troubleshooting
* Resolution steps
* Verification of fix
* Supporting screenshots

The goal is to demonstrate job-ready IT support skills, not theoretical knowledge.

---

## 🏗️ Lab Environment

* Windows Server (Domain Controller: DC01)
* Active Directory Domain Services (AD DS)
* Domain: `corp.local`
* Virtualization: Oracle VirtualBox

### Tools Used

* Active Directory Users and Computers (ADUC)
* Group Policy Management (GPMC)
* Windows Event Viewer
* Command Line Tools (ipconfig, ping, etc.)

---

## 📁 Repository Structure

```
helpdesk-lab/
│
├── incidents/
│   ├── 001-user-creation/
│   ├── 002-password-reset/
│   ├── 003-account-locked/
│   ├── 004-login-failure/
│   ├── 005-outlook-not-sending/
│   ├── 006-network-connectivity-issue/
│   ├── 007-printer-not-working/
│   ├── 008-software-installation-failure/
│
├── screenshots/
└── notes/
```

Each incident folder contains:

* `incident-report.md` → full ticket documentation
* screenshots → evidence of troubleshooting and resolution

---

## 🎫 Help Desk Scenarios

### 001 - User Account Creation

* Created new Active Directory user account
* Configured initial password and enforced password change at next login
* Assigned appropriate Organizational Unit and group membership

### 002 - Password Reset

* Reset user password via ADUC
* Forced password change at next login
* Verified successful authentication

### 003 - Account Lockout

* Configured account lockout policy via Group Policy
* Simulated failed login attempts
* Unlocked account and restored access

### 004 - Login Failure (In Progress)

* Troubleshooting authentication failures
* Investigating credential, domain, and system-related causes

### 005 - Outlook Not Sending Emails

* Diagnosed emails stuck in Outbox
* Identified Outlook “Work Offline” mode enabled
* Restored email sending and verified external delivery

### 006 - Network Connectivity Issue

* Diagnosed loss of network and internet connectivity
* Identified DHCP failure (APIPA address assignment)
* Restored valid IP configuration and network access

### 007 - Printer Not Working

* Diagnosed print jobs stuck in queue
* Identified stale or incorrect printer mapping
* Reinstalled network printer and restored functionality

### 008 - Software Installation Failure

* Diagnosed installation failure due to insufficient permissions
* Installed software using administrative credentials
* Verified successful execution and functionality

### 009 - DNS Resolution Issue (Planned)

* Troubleshoot domain name resolution failures
* Analyze DNS configuration and connectivity

### 010 - Group Permissions (Planned)

* Assign users to security groups
* Manage access control and resource permissions

---

## 🔧 Skills Demonstrated

* Active Directory user and group management
* Password resets and account recovery
* Group Policy configuration (GPO)
* Network troubleshooting (IP, DHCP, DNS)
* Email client troubleshooting (Outlook)
* Printer and device support
* Software installation and permission management
* Incident documentation and ticket workflow simulation
* Windows Server administration fundamentals

---

## 🎯 Purpose

This project is designed to:

* Simulate real-world IT help desk workflows
* Build hands-on Active Directory experience
* Demonstrate troubleshooting and escalation thinking
* Provide a verifiable technical portfolio for employers

---

## 🚀 Future Improvements

* Add DNS and Group Policy failure deep-dive scenarios
* Introduce PowerShell automation (user provisioning, resets)
* Simulate ticketing system workflow (ServiceNow-style structure)
* Expand into endpoint security and permissions auditing
* Add network troubleshooting (firewall, routing, latency issues)

---

## 📌 Notes

This is a self-directed lab environment created for professional development and IT support portfolio demonstration.
