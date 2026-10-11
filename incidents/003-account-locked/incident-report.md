\# Incident 003: Active Directory Account Lockout



\## Incident Summary



\*\*Ticket ID:\*\* INC-003  

\*\*Category:\*\* Account Access / Active Directory  

\*\*Severity:\*\* Low  

\*\*Affected User:\*\* `jdoe`  

\*\*Domain:\*\* `corp.local`  

\*\*Domain Controller:\*\* `DC01`  

\*\*Status:\*\* Resolved, pending final sign-in verification if not yet tested



\## Issue Description



The user account `jdoe` became locked in the Active Directory domain, preventing the user from authenticating with the account.



The objective was to verify the account lockout, identify the relevant account status in Active Directory Users and Computers (ADUC), unlock the account, and confirm the resulting state.



\## Environment



\- Windows Server domain controller: `DC01`

\- Active Directory domain: `corp.local`

\- Management tool: Active Directory Users and Computers (ADUC)

\- Affected account: `jdoe`



\## Troubleshooting and Resolution



1\. Opened Active Directory Users and Computers on the domain controller.

2\. Located the affected user account, `jdoe`.

3\. Inspected the account status to verify the lockout.

4\. Unlocked the account using the available Active Directory account-management options.

5\. Rechecked the account to verify the post-resolution state.

6\. A successful sign-in should be tested separately to confirm end-to-end authentication.



\## Screenshot Evidence



The following screenshots correspond to the evidence files in the repository's `screenshots/` directory:



\### 1. Account Locked Before Resolution



!\[Account locked before resolution](../../screenshots/003-account-locked-before/003-account-locked-before.png)



\*\*File:\*\* `screenshots/003-account-locked-before/003-account-locked-before.png`



Shows the account's state before the unlock action.



\### 2. Account Unlocked After Resolution



!\[Account unlocked after resolution](../../screenshots/003-account-unlocked-after/003-account-unlocked-after.png)



\*\*File:\*\* `screenshots/003-account-unlocked-after/003-account-unlocked-after.png`



Shows the account's state after the unlock action.



\## Root Cause and Prevention



The account reached the configured Active Directory account-lockout threshold. In this lab, the intended policy settings are:



\- \*\*Account lockout threshold:\*\* 5 invalid logon attempts

\- \*\*Account lockout duration:\*\* 15 minutes

\- \*\*Reset account lockout counter after:\*\* 15 minutes



These values should be confirmed against the actual domain policy before being treated as verified configuration.



\## Skills Demonstrated



\- Active Directory Users and Computers (ADUC)

\- User account troubleshooting

\- Account lockout identification and resolution

\- Windows Server administration

\- Evidence capture and incident documentation

\- Post-resolution verification



\## Outcome



The incident documents the account-lockout investigation and unlock procedure. Final authentication success should only be recorded after a successful sign-in has actually been tested.





