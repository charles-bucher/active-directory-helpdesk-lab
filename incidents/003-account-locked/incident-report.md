\# Incident Report: Account Lockout



\## Ticket ID

003-account-locked



\## Request

User unable to log in due to account lockout after multiple failed login attempts.



\## Environment

\- Domain: corp.local

\- System: Windows Server (DC01)

\- Tool: Active Directory Users and Computers (ADUC)



\## Cause

Account lockout triggered after exceeding configured login attempt threshold defined in Group Policy.



\## Action Taken

\- Attempted login with incorrect password multiple times to reproduce issue

\- Verified account lockout status in Active Directory (Account tab)

\- Opened user properties for account: jdoe

\- Unlocked account via "Unlock account" option

\- Confirmed account status returned to normal



\## Result

User account successfully unlocked. User is able to log in with correct credentials.



\## Status

Resolved



\## Evidence

\- Screenshot: 003-account-locked\_aduc.png



\## Notes

Account lockout policy configured via Group Policy:

\- Lockout threshold: 5 invalid attempts

\- Lockout duration: 15 minutes

\- Reset counter: 15 minutes



This scenario demonstrates troubleshooting of authentication issues and use of Active Directory account controls.

