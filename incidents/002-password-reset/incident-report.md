# 🧾 Incident Report: Active Directory Password Reset

## 🎫 Ticket Information

- **Ticket ID:** `INC-002-password-reset`
- **Issue Type:** Account Access / Password Reset
- **Affected User:** Jamie Rivera (`jrivera`)
- **Domain:** `corp.local`
- **Status:** Password reset completed; successful sign-in not independently verified

## 🧩 Summary

A user-reported password issue prompted a password reset in the Active Directory lab. The reset was performed through Active Directory Users and Computers (ADUC).

The administrative confirmation dialog verified that Jamie Rivera's password had been changed successfully. A successful user sign-in was not captured as part of this incident's evidence.

## 📌 Request Details

- **Issue Type:** Login failure / password assistance
- **Reported Cause:** Forgotten password
- **Affected Account:** Jamie Rivera (`jrivera`)
- **Impact:** User reported difficulty accessing domain resources

The forgotten-password cause is based on the reported scenario, not an independently verified technical root cause.

## 🖥️ Environment

- **Domain:** `corp.local`
- **Domain Controller:** `DC01-NEW`
- **Operating System:** Windows Server 2022
- **Directory Service:** Active Directory Domain Services (AD DS)
- **Administrative Tool:** Active Directory Users and Computers (ADUC)
- **Virtualization Platform:** Oracle VirtualBox

## 🔍 Actions Taken

1. Opened Active Directory Users and Computers.
2. Located Jamie Rivera's account in the domain.
3. Initiated the password-reset operation.
4. Entered a new lab password.
5. Received Active Directory confirmation that the password had been changed.

The available screenshot does not establish whether **User must change password at next logon** was enabled during this incident, so that setting is not claimed as a completed action.

## 🧪 Validation

**Confirmed:**

ADUC displayed the following confirmation message:

> The password for jamie Rivera has been changed.

This confirms completion of the administrative password-reset operation.

**Not independently verified:**

- Successful interactive sign-in by Jamie Rivera.
- Successful access to domain resources using the reset password.
- A forced password-change prompt at the next logon.

These steps require separate testing and evidence before they can be recorded as successful.

## ✅ Outcome

The password-reset operation completed successfully according to the Active Directory confirmation dialog.

**Final Status:** Password reset completed; user sign-in verification remains outstanding.

## 📎 Evidence

**Screenshot directory:** `screenshots/002-password-reset/`

- `002-password-reset-success.png` — Active Directory confirmation that Jamie Rivera's password was changed.

## 🧠 Lessons Learned

- Confirm that the password-reset operation completed successfully.
- Distinguish an administrative confirmation from a successful user sign-in.
- Document password-change-at-next-logon settings only when verified.
- Capture separate evidence of authentication testing when validating end-to-end resolution.
- Never include passwords or other credentials in public portfolio documentation.