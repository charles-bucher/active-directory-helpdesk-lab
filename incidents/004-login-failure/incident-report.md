\# Incident Report: Login Failure



\## Ticket ID

`004-login-failure`



\## Request

User reported being unable to log in to the workstation/domain using their credentials.



\## Environment

\- \*\*Domain:\*\* `corp.local`

\- \*\*Domain Controller:\*\* `DC01`

\- \*\*Affected User:\*\* `jdoe`

\- \*\*Platform:\*\* Windows Server / Active Directory lab

\- \*\*Tooling:\*\* Active Directory Users and Computers (ADUC)



\## Symptoms

\- Login attempt returned an authentication failure.

\- User could not access the domain using the attempted credentials.

\- Additional troubleshooting was required to identify and resolve the issue.



\## Initial Checks

1\. Confirmed the `jdoe` account exists in Active Directory.

2\. Checked whether the account was disabled or locked.

3\. Considered the recent password-reset scenario from Incident 002.

4\. Reviewed the login failure and available diagnostic evidence.



\## Root Cause Analysis

Potential causes of a domain login failure include:

\- Incorrect or outdated password.

\- Account lockout or disabled account.

\- Incorrect username or domain format.

\- Client connectivity or domain authentication problems.



The exact root cause should only be documented once the diagnostic evidence confirms it.



\## Action Taken

1\. Reviewed the login failure message.

2\. Checked the account status in Active Directory Users and Computers.

3\. Investigated the issue using the available troubleshooting evidence.

4\. Retested authentication after the corrective action.



\## Result

The lab includes evidence of the login failure, diagnostic troubleshooting, and a subsequent successful login. The precise corrective action should be recorded based on what was actually performed in the lab.



\## Status

Resolved, based on the successful-login evidence.



\## Screenshot Evidence



The following filenames match the screenshot folder names currently listed in the repository. The image paths below assume each folder contains a PNG file with the same name.



\### 1. Login Failure



!\[Login failure evidence](../../screenshots/004-login-failure-error/004-login-failure-error.png)



\*\*File:\*\* `screenshots/004-login-failure-error/004-login-failure-error.png`



Shows the initial authentication failure.



\### 2. Login Failure Diagnostics



!\[Login failure diagnostic evidence](../../screenshots/004-login-failure-diagnostics/004-login-failure-diagnostics.png)



\*\*File:\*\* `screenshots/004-login-failure-diagnostics/004-login-failure-diagnostics.png`



Supports the troubleshooting and diagnostic steps.



\### 3. Successful Login



!\[Successful login evidence](../../screenshots/004-login-success/004-login-success.png)



\*\*File:\*\* `screenshots/004-login-success/004-login-success.png`



Shows the successful login after troubleshooting.



\## Skills Demonstrated

\- Active Directory account verification

\- Windows authentication troubleshooting

\- Account status checks

\- Login error investigation

\- Troubleshooting documentation

\- Evidence capture and resolution verification



