🧾 Incident Report: Active Directory User Account Creation
Ticket ID

INC-001-user-creation

🧩 Summary

New employee onboarding request requiring creation of an Active Directory user account for system access provisioning.

📌 Request Details

Create a new domain user account for:

Username: jdoe
Department: Not specified (assumed standard access profile)
Purpose: Initial onboarding / system access setup
🖥️ Environment
Domain: corp.local
Server Role: Windows Server Active Directory Domain Services (AD DS)
Management Tool: Active Directory Users and Computers (ADUC)
⚙️ Actions Taken
Opened Active Directory Users and Computers (ADUC)
Navigated to: Users container
Created new user object:
Username: jdoe
Display Name: John Doe
Assigned temporary password: Welcome123!
Enabled password policy:
✔ User must change password at next logon
Verified user object creation in ADUC list
🧪 Validation / Testing
Confirmed user account appears in correct OU/container
Verified account is enabled and not locked
Simulated first login conditions (password reset requirement enforced)
✅ Outcome

User account successfully created and provisioned in Active Directory. Account is ready for first login and further group/permission assignment if required.

🟢 Status

Resolved

🧠 Notes / Operational Context
Standard onboarding workflow completed within AD environment (corp.local)
No group memberships assigned in this task (future step: role-based access assignment depending on department)
Password policy compliance enforced per onboarding standards
📎 Evidence
Screenshot: 001-user-creation_aduc-user-list.png
(Optional improvement: include timestamped ADUC view showing user object creation)