\# 🧾 Incident Report: Active Directory Account Lockout



\## Ticket Information



\*\*Ticket ID:\*\* `INC-003-account-lockout`  

\*\*Issue Type:\*\* Account Access / Authentication  

\*\*Affected User:\*\* Jamie Rivera (`jrivera`)  

\*\*Domain:\*\* `corp.local`  

\*\*Status:\*\* Account unlock performed; successful sign-in not independently verified



\## 🧩 Summary



During Active Directory lab testing, Jamie Rivera's account was observed in a locked state. The account status was inspected through Active Directory Users and Computers (ADUC), and the account was subsequently unlocked.



The investigation also documented the domain's account lockout policy. The captured policy output showed a threshold of five invalid logon attempts, a lockout duration of 30 minutes, and a lockout observation window of 30 minutes.



\## 🖥️ Environment



\- \*\*Domain:\*\* `corp.local`

\- \*\*NetBIOS domain name:\*\* `CORP`

\- \*\*Domain controller:\*\* `DC01-NEW`

\- \*\*Operating system:\*\* Windows Server 2022

\- \*\*Directory service:\*\* Active Directory Domain Services (AD DS)

\- \*\*Management tool:\*\* Active Directory Users and Computers (ADUC)

\- \*\*Policy verification:\*\* `net accounts`



\## 🔍 Symptoms



The test account's status changed during the lab exercise. The screenshots show an initial account state and a subsequent state in which the \*\*Unlock account\*\* checkbox was selected.



The captured evidence documents the account status and the administrative unlock workflow. It does not include a successful post-unlock interactive sign-in.



\## ⚙️ Policy Configuration



The `003-account-lockout-policy.png` screenshot shows the output of `net accounts` with these values:



| Setting | Captured value |

|---|---:|

| Lockout threshold | 5 invalid attempts |

| Lockout duration | 30 minutes |

| Lockout observation window | 30 minutes |



These are the values shown in the captured evidence and should be reported as such unless the policy is changed and a new screenshot is captured.



\## 🛠️ Troubleshooting and Actions Taken



1\. Opened Active Directory Users and Computers.

2\. Located Jamie Rivera (`jrivera`) in the `corp.local` domain.

3\. Reviewed the user's Account tab.

4\. Captured an account state with \*\*Unlock account\*\* unchecked.

5\. Captured a subsequent account state with \*\*Unlock account\*\* checked, indicating the account was flagged as locked.

6\. Used ADUC to clear the lockout state.

7\. Captured the resulting Users list with Jamie Rivera selected.



\## 🧪 Validation



\*\*Confirmed by screenshots:\*\*

\- The domain lockout policy output showed a threshold of five attempts, a 30-minute lockout duration, and a 30-minute observation window.

\- The account's Account tab was captured both with the \*\*Unlock account\*\* checkbox unchecked and with it checked.



\*\*Evidence limitation:\*\*

\- The final screenshot shows the Users list rather than the Account tab after the unlock. It therefore does not independently display the cleared lockout checkbox.

\- A successful interactive sign-in was not captured.



For complete validation, the Account tab should be captured after unlocking, with \*\*Unlock account\*\* unchecked and \*\*Account is disabled\*\* unchecked. A successful sign-in test should be documented separately if completed.



\## ✅ Outcome



The account lockout was investigated through ADUC, and the administrative unlock action was performed. The screenshots demonstrate the configured policy and the observed account states.



\*\*Final status:\*\* Unlock action performed; post-unlock account state and successful sign-in require stronger final evidence.



\## 📎 Screenshot Evidence



All evidence is stored in `screenshots/003-account-locked/`.



1\. \*\*`003-account-lockout-policy.png`\*\*  

&#x20;  Captured `net accounts` output showing the threshold and lockout timing values.



2\. \*\*`003-account-locked-before.png`\*\*  

&#x20;  Jamie Rivera's Account tab with \*\*Unlock account\*\* unchecked.



3\. \*\*`003-account-locked-confirmed.png`\*\*  

&#x20;  Jamie Rivera's Account tab with \*\*Unlock account\*\* checked, indicating a locked state.



4\. \*\*`003-account-unlocked-after.png`\*\*  

&#x20;  Active Directory Users list with Jamie Rivera selected after the unlock workflow.



\## 🧠 Lessons Learned



\- Confirm the actual configured lockout settings before documenting policy values.

\- Distinguish an account's observed state from assumptions about successful authentication.

\- Capture evidence before and after an administrative change.

\- Verify the final account state and test sign-in before marking an authentication incident fully resolved.



