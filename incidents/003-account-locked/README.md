🧾 Incident Report: Active Directory Account Lockout
Ticket ID

INC-003-account-lockout

🧩 Summary

User account was locked due to multiple failed authentication attempts, preventing successful login to domain resources.

📌 Request Details
Issue Type: Authentication failure
Affected User: jdoe
Impact: User unable to log into domain systems
Reported Behavior: Repeated login failure prompt / account lock message
🖥️ Environment
Domain: corp.local
Domain Controller: DC01
System: Windows Server Active Directory Domain Services (AD DS)
Tool: Active Directory Users and Computers (ADUC)
Policy Source: Group Policy Object (GPO)
🔍 Root Cause

Account lockout was triggered by the configured domain security policy after multiple invalid password attempts exceeded the defined threshold.

Policy Details:

Lockout threshold: 5 invalid attempts
Lockout duration: 15 minutes
Reset counter: 15 minutes
⚙️ Actions Taken
Opened Active Directory Users and Computers (ADUC)
Searched and located user account: jdoe
Reviewed account status under Account tab
Confirmed account was in a locked state
Performed account unlock using:
✔ “Unlock account” option in ADUC
Verified account status returned to active state
🧪 Validation / Testing
Confirmed account lockout flag was cleared in ADUC
Verified user account is enabled and not restricted
Simulated expected behavior post-unlock (successful authentication path assumed with valid credentials)
✅ Outcome

User account successfully unlocked. User regained ability to authenticate to domain resources using correct credentials.

🟢 Status

Resolved

🧠 Notes / Operational Context
Issue aligns with standard Active Directory account lockout policy enforcement
No evidence of malicious activity identified in this scenario (assumed benign user error)
No escalation required
Future mitigation: user advised to verify credentials before repeated login attempts
📎 Evidence
Screenshot: 003-account-locked_aduc.png