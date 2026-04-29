\# Incident Report: Login Failure



\## Ticket ID

004-login-failure



\## Request

User reported inability to log into workstation/domain using valid credentials.



\## Environment

\- Domain: corp.local

\- System: Windows Server DC01 (Active Directory environment)

\- Tooling: Active Directory Users and Computers (ADUC)



\## Symptoms

\- User receives login failure message

\- Credentials appear correct but authentication is denied

\- No access to domain resources



\## Initial Checks

\- Verified user account exists in Active Directory

\- Confirmed account is not disabled or locked out

\- Verified password was recently reset in prior ticket scenarios



\## Root Cause Analysis

Login failure likely related to:

\- Cached credentials mismatch OR

\- Password not updated on client login attempt OR

\- Domain authentication sync delay (Kerberos/AD propagation)



\## Action Taken

\- Verified account status in ADUC

\- Confirmed user credentials (jdoe) are active

\- Ensured password reset policy is applied correctly

\- Re-tested login after waiting for policy sync



\## Result

User authentication restored after verifying account status and credentials consistency in Active Directory.



\## Status

Resolved



\## Evidence

\- Screenshot: 004-login-failure\_aduc.png



\## Notes

This scenario demonstrates basic authentication troubleshooting in an Active Directory environment, including verification of account status, credential validation, and domain login flow understanding.

