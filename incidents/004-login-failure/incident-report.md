# 🧾 Incident Report: Windows Domain Login Failure

## 🎫 Ticket Information

- **Ticket ID:** `INC-004-login-failure`
- **Issue Type:** Authentication / Account Access
- **Priority:** Medium
- **Affected User:** `jdoe`
- **Domain:** `corp.local`
- **Domain Controller:** `DC01-NEW`
- **Status:** Successful login documented; exact root cause and corrective action require confirmation

## 🧩 Summary

This lab exercise documents troubleshooting a Windows domain login failure in an Active Directory environment.

The workflow covers reviewing the authentication error, checking the affected account in Active Directory Users and Computers (ADUC), examining available diagnostic evidence, and retesting authentication after troubleshooting.

The exact root cause should only be recorded when supported by the diagnostic evidence.

## 📌 Issue Description

The user reported being unable to sign in to the workstation or domain using the attempted credentials.

A domain login failure can result from several conditions, including incorrect credentials, account restrictions, or problems communicating with a domain controller.

## 🖥️ Environment

- **Domain:** `corp.local`
- **Domain Controller:** `DC01-NEW`
- **Affected Account:** `jdoe`
- **Platform:** Windows Server / Active Directory lab
- **Directory Service:** Active Directory Domain Services (AD DS)
- **Management Tool:** Active Directory Users and Computers (ADUC)
- **Virtualization Platform:** Oracle VirtualBox

## 🔍 Initial Checks

1. Checked the affected username and reviewed the login failure.
2. Located the `jdoe` account in Active Directory.
3. Reviewed the account's status for relevant restrictions, such as disabled or locked status.
4. Considered whether credential issues or recent password changes could be relevant.
5. Reviewed the available diagnostic evidence.

Only checks actually performed should be recorded as completed.

## 🧠 Root Cause Analysis

Potential causes of a domain login failure include:

- Incorrect or outdated password.
- Account lockout or disabled status.
- Incorrect username or domain format.
- Workstation connectivity or domain controller communication problems.

**Confirmed root cause:** Not specified in the current documentation.

The exact cause should be added once the diagnostic evidence identifies the condition responsible for the failure.

## 🛠️ Troubleshooting and Resolution

1. Reviewed the initial login failure.
2. Checked the affected account in Active Directory Users and Computers.
3. Examined the available diagnostic evidence.
4. Performed the corrective action used in the lab.
5. Retested authentication and captured evidence of the subsequent successful login.

Document the specific corrective action once it has been confirmed from the actual lab work.

## 🧪 Validation

**Evidence described in this lab:**

- Initial authentication failure.
- Diagnostic troubleshooting evidence.
- Subsequent successful login.

The successful-login screenshot supports recovery of authentication in the demonstrated scenario. It does not independently establish the exact root cause unless the diagnostic evidence identifies it.

## 📸 Screenshot Evidence

### 1. Initial Login Failure

![Login failure evidence](../../screenshots/004-login-failure-error/004-login-failure-error.png)

**File:** `screenshots/004-login-failure-error/004-login-failure-error.png`

Shows the initial authentication failure.

### 2. Login Failure Diagnostics

![Login failure diagnostic evidence](../../screenshots/004-login-failure-diagnostics/004-login-failure-diagnostics.png)

**File:** `screenshots/004-login-failure-diagnostics/004-login-failure-diagnostics.png`

Supports the troubleshooting investigation.

### 3. Successful Login

![Successful login evidence](../../screenshots/004-login-success/004-login-success.png)

**File:** `screenshots/004-login-success/004-login-success.png`

Shows the subsequent successful login.

Confirm that all three image files exist at these paths and that their contents match the descriptions.

## 🧠 Lessons Learned

- Verify the affected account before making changes.
- Check account status and credential-related issues before assuming a root cause.
- Distinguish observed symptoms from confirmed causes.
- Retest authentication after corrective action.
- Use screenshots to support the documented troubleshooting sequence.

## ✅ Outcome

The lab documentation describes an initial login failure, investigation, and subsequent successful authentication.

**Final Status:** Successful login documented; exact root cause and corrective action should be confirmed against the lab evidence.