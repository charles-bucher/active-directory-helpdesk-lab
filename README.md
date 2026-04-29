<<<<<<< HEAD
﻿\# Active Directory Help Desk Lab



Simulated IT help desk environment built using Windows Server and Active Directory.  

This lab demonstrates real-world Tier 1 support tasks including user provisioning, password resets, account lockouts, and access management.



\---



\## 🧠 Overview



This project replicates common help desk responsibilities in a controlled virtual environment.  

Each scenario is documented as a ticket with step-by-step actions and supporting screenshots.



The goal is to demonstrate practical, job-ready IT support skills rather than theoretical knowledge.



\---



\## 🏗️ Lab Environment



\- Windows Server (Domain Controller: DC01)

\- Active Directory Domain Services (AD DS)

\- Domain: `corp.local`

\- Tools:

&#x20; - Active Directory Users and Computers (ADUC)

&#x20; - Group Policy Management

\- Virtualized using Oracle VirtualBox



\---



\## 📁 Repository Structure





helpdesk-lab/

│

├── incidents/

│ ├── 001-user-creation/

│ ├── 002-password-reset/

│ ├── 003-account-locked/

│ ├── 004-login-failure/

│ └── 005-group-permissions/

│

├── screenshots/

└── notes/





Each incident folder contains:

\- `incident-report.md` → ticket documentation

\- related screenshots → evidence of actions taken



\---



\## 🎫 Help Desk Scenarios



\### 001 - User Account Creation

\- Created new user in Active Directory

\- Configured initial password and login requirements



\### 002 - Password Reset

\- Reset user password

\- Forced password change at next login



\### 003 - Account Lockout

\- Configured Group Policy lockout threshold

\- Simulated failed logins

\- Unlocked user account via ADUC



\### 004 - Login Failure \*(planned / in progress)\*

\- Troubleshoot authentication issues



\### 005 - Group Permissions \*(planned / in progress)\*

\- Assign users to security groups

\- Manage access control



\---



\## 🔧 Skills Demonstrated



\- Active Directory user management

\- Password and account recovery

\- Group Policy configuration (GPO)

\- Troubleshooting authentication issues

\- Ticket documentation and resolution workflow

\- Basic Windows Server administration



\---



\## 🎯 Purpose



This lab is designed to:

\- Simulate real IT help desk tasks

\- Build hands-on experience with Active Directory

\- Demonstrate troubleshooting and documentation skills

\- Provide a portfolio of verifiable technical work



\---



\## 🚀 Next Steps



\- Expand scenarios (DNS issues, group policy troubleshooting)

\- Add PowerShell-based user management

\- Simulate ticket queue workflows

\- Integrate basic networking troubleshooting



\---



\## 📌 Notes



This is a self-directed lab environment created for learning and portfolio purposes.  

All scenarios are simulated but reflect real-world IT support tasks.



\---

=======
# active-directory-helpdesk-lab
Simulated IT Help Desk environment using Active Directory and Windows Server. Includes password resets, user provisioning, account lockouts, and troubleshooting scenarios documented with ticket-style incident reports and screenshots
>>>>>>> b5aded3774b0563ffb0612b069bb3a2807ceebba
