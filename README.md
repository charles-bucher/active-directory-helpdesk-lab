# Active Directory Help Desk Lab

A self-directed IT support portfolio built with **Windows Server 2022, Active Directory Domain Services (AD DS), and Oracle VirtualBox**.

This project demonstrates common Tier 1 help desk workflows through simulated support incidents, technical troubleshooting, documentation, and supporting screenshots.

## 🎯 Project Goals

- Practice common Level 1 help desk tasks in a Windows domain environment.
- Develop foundational Active Directory and Windows troubleshooting skills.
- Document incidents using a structured, ticket-based workflow.
- Capture evidence of troubleshooting steps and verified outcomes.
- Build a practical portfolio for entry-level IT support and service desk roles.

## 🖥️ Lab Environment

| Component | Configuration |
|---|---|
| Operating system | Windows Server 2022 |
| Domain controller | `DC01-NEW` |
| Active Directory domain | `corp.local` |
| NetBIOS domain name | `CORP` |
| Virtualization platform | Oracle VirtualBox |

## 🧰 Tools and Technologies

- **Active Directory Users and Computers (ADUC):** User account administration and password resets
- **Group Policy Management (GPMC):** Group Policy review and configuration
- **Windows Command Prompt:** System and network diagnostics
- **Windows PowerShell:** Windows administration and command-line troubleshooting
- **Windows Event Viewer:** System and authentication event investigation
- **Network utilities:** `ipconfig`, `ping`, and `nslookup`
- **Git and GitHub:** Version control and portfolio documentation

## 🎫 Help Desk Incident Scenarios

Each incident is organized as a support ticket, with documentation covering the reported issue, investigation, troubleshooting, resolution, and verification where completed.

| Incident | Scenario | Skills Demonstrated |
|---|---|---|
| 001 | User Account Creation | Active Directory user provisioning |
| 002 | Password Reset | Account administration and password management |
| 003 | Account Lockout | Account recovery and lockout troubleshooting |
| 004 | Login Failure | Authentication troubleshooting |
| 005 | Outlook Not Sending | Email troubleshooting and connectivity testing |
| 006 | Network Connectivity Issue | IP configuration and network diagnostics |
| 007 | Printer Not Working | Printer troubleshooting workflow |
| 008 | Software Installation Failure | Installation permissions and application troubleshooting |

**Evidence standard:** Incidents are documented according to the work actually completed. Screenshots support recorded findings, and unverified resolutions remain marked as pending rather than being presented as successful outcomes.

## 📁 Repository Structure

```text
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
```

Each incident folder contains its own documentation. The screenshots directory stores supporting evidence captured during lab exercises.

## 📋 Incident Documentation Workflow

1. **Identify:** Record the reported issue and its impact.
2. **Investigate:** Gather relevant system information and diagnostic evidence.
3. **Troubleshoot:** Test likely causes using appropriate tools.
4. **Resolve:** Apply an appropriate corrective action when identified.
5. **Verify:** Confirm the outcome rather than assuming the fix worked.
6. **Document:** Record findings, evidence, and any remaining limitations.

## 💼 Skills Practiced

- Active Directory user account management
- Password reset procedures
- Account lockout investigation
- Windows authentication troubleshooting
- Basic networking diagnostics
- Email and printer troubleshooting workflows
- Software installation troubleshooting
- Technical documentation and incident reporting
- Evidence management and Git-based version control

## 🚀 Project Purpose

This portfolio is part of my preparation for an entry-level **Help Desk Technician, IT Support Specialist, or Service Desk Analyst** role.

It demonstrates hands-on lab practice, a methodical troubleshooting process, and a commitment to documenting technical work accurately.

**Note:** This is a self-directed educational lab using simulated incidents. It is intended to demonstrate practical learning and foundational skills, not paid professional IT experience.
