\# 🧾 Incident Report: Domain Login Failure



\## Ticket Information



\*\*Ticket ID:\*\* `INC-004-login-failure`  

\*\*Issue Type:\*\* Authentication / Sign-in troubleshooting  

\*\*Status:\*\* Investigated; interactive sign-in restriction remains unresolved  

\*\*Environment:\*\* Home lab using Oracle VirtualBox



\## 🧩 Summary



A domain user experienced authentication failures while testing domain credentials in a Windows Server Active Directory lab. Initial attempts returned a username/password error. A later interactive sign-in attempt returned error `1385`, indicating that the requested type of sign-in was not permitted.



The user's Active Directory account was inspected, and network access to the domain's SYSVOL share was subsequently verified using `runas /netonly`.



\*\*Important:\*\* Access to SYSVOL was successful, but an interactive Windows sign-in was not confirmed.



\## 📌 Request Details



\- \*\*Affected User:\*\* Jamie Rivera (`jrivera`)

\- \*\*Domain:\*\* `corp.local`

\- \*\*Impact:\*\* Domain sign-in test could not complete using the standard `runas` command.

\- \*\*Reported Behavior:\*\* Authentication errors occurred despite resetting the test user's password.



\## 🖥️ Environment



\- \*\*Domain:\*\* `corp.local`

\- \*\*NetBIOS Domain Name:\*\* `CORP`

\- \*\*Domain Controller:\*\* `DC01-NEW`

\- \*\*Operating System:\*\* Windows Server 2022

\- \*\*Directory Service:\*\* Active Directory Domain Services (AD DS)

\- \*\*Administrative Tool:\*\* Active Directory Users and Computers (ADUC)

\- \*\*Virtualization Platform:\*\* Oracle VirtualBox



\## 🔍 Symptoms



\- Initial `runas` attempts returned error `1326`: the username or password was reported as incorrect.

\- A subsequent interactive sign-in attempt returned error `1385`.

\- The user could not confirm a successful interactive sign-in as `CORP\\jrivera`.

\- Using `runas /netonly`, a new Command Prompt opened and a directory listing of `\\\\corp.local\\SYSVOL` succeeded.



\## 🔎 Initial Checks



The following checks were completed:



1\. Located Jamie Rivera's account in Active Directory Users and Computers.

2\. Confirmed that \*\*Account is disabled\*\* was unchecked.

3\. Confirmed that \*\*Unlock account\*\* was unchecked, indicating the account was not showing as locked.

4\. Confirmed that \*\*User must change password at next logon\*\* was unchecked.

5\. Reset the test user's password through ADUC.

6\. Verified that the administrative Command Prompt was running on `DC01-NEW` under the `CORP` domain.



\## 🧠 Analysis



The initial error `1326` did not establish whether the cause was an incorrect password or another authentication issue.



The later error `1385` indicated that the requested logon type was not granted. A sign-in restriction on the domain controller is a possible explanation, but the exact policy or setting responsible was not independently confirmed.



Successful access to SYSVOL using `runas /netonly` demonstrated that the supplied credentials could access that network resource. This does not prove that interactive logon was permitted or that every domain resource was accessible.



\## ⚙️ Actions Taken



\- Inspected the user's account status in ADUC.

\- Reset the test user's password.

\- Confirmed the server and domain context.

\- Retested the standard `runas` command and recorded the authentication errors.

\- Used `runas /netonly` to test access to a domain network resource without changing domain security policy.

\- Ran `dir \\\\corp.local\\SYSVOL` and verified that the command returned a directory listing.



\## 🧪 Validation



\*\*Successful validation:\*\* The SYSVOL directory listing was returned when using the `/netonly` test.



\*\*Not yet validated:\*\* A successful interactive sign-in as `CORP\\jrivera`.



No claim is made that a Windows user session or domain profile was successfully loaded.



\## ✅ Outcome



The investigation confirmed that the account was enabled and not showing as locked, and that the supplied credentials could access the domain's SYSVOL network share.



The interactive sign-in failure remains unresolved. Further investigation would need to identify which sign-in policy or user-right assignment caused error `1385`, without weakening domain controller security unnecessarily.



\## 📎 Evidence



Screenshots are stored in `screenshots/004-login-failure/`.



\- `004-login-failure-error.png` — Initial login failure evidence.

\- `004-login-failure-diagnostics.png` — Server, user, and domain context checks.

\- `004-login-failure-success.png` — Successful SYSVOL directory listing using the `/netonly` test.



\## 🧠 Lessons Learned



\- Verify the account state before repeatedly retrying authentication.

\- Distinguish invalid-credential errors from sign-in-right restrictions.

\- A successful network-resource authentication test does not prove interactive logon succeeded.

\- Record confirmed results separately from suspected root causes.

\- Avoid weakening domain controller security to make a lab test pass.



