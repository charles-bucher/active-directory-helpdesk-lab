# 🧾 Incident Report: Active Directory User Account Creation

## 🎫 Ticket Information

- **Ticket ID:** `INC-001-user-creation`
- **Issue Type:** User Provisioning / Account Creation
- **Affected User:** Jamie Rivera (`jrivera`)
- **Domain:** `corp.local`
- **Priority:** Low
- **Status:** User object creation evidenced; additional account settings not independently verified

## 🧩 Summary

A new user account was created in the Active Directory lab to demonstrate a basic user-provisioning workflow. The account was created using Active Directory Users and Computers (ADUC) and appears in the domain's default Users container.

The available screenshot confirms that the Jamie Rivera user object is listed in Active Directory. It does not independently verify the account's enabled status, password settings, group memberships, or ability to sign in.

## 📌 Request Details

- **Request Type:** New user account creation
- **Display Name:** Jamie Rivera
- **Username:** `jrivera`
- **Department:** Not specified
- **Purpose:** Demonstrate account provisioning for domain access

## 🖥️ Environment

- **Domain:** `corp.local`
- **NetBIOS Domain Name:** `CORP`
- **Domain Controller:** `DC01-NEW`
- **Operating System:** Windows Server 2022
- **Directory Service:** Active Directory Domain Services (AD DS)
- **Management Tool:** Active Directory Users and Computers (ADUC)
- **Virtualization Platform:** Oracle VirtualBox

## ⚙️ Actions Taken

1. Opened Active Directory Users and Computers.
2. Navigated to the domain's Users container.
3. Created the Jamie Rivera user object with the username `jrivera`.
4. Completed the account-creation workflow in ADUC.
5. Located Jamie Rivera in the Users list and captured screenshot evidence.

The temporary password is intentionally excluded from public documentation. The available screenshot does not show the password or independently verify password-related options.

## 🧪 Validation

**Confirmed by screenshot:**

- Jamie Rivera appears in the Active Directory Users list.
- The user object is present in the Users container.

**Not established by the available screenshot:**

- Whether the account is enabled or disabled.
- Whether **User must change password at next logon** is enabled.
- Whether additional group memberships were assigned.
- Whether the user successfully signed in.

These checks require separate evidence before they can be recorded as verified.

## ✅ Outcome

The user-creation task is documented, and the available screenshot confirms that the Jamie Rivera user object appears in Active Directory.

**Final Status:** User object creation evidenced; account configuration and sign-in validation are not demonstrated by the available screenshot.

## 📎 Evidence

- **Screenshot:** `screenshots/001-user-creation_aduc-user-list/001-user-creation_aduc-user-list.png`

The screenshot displays the Active Directory Users list with Jamie Rivera selected. Confirm that the path and filename match the actual file in the repository.

## 🧠 Lessons Learned

- Verify the user's display name and account identifier before documenting a provisioning task.
- Capture evidence of the account appearing in Active Directory.
- Use separate screenshots to demonstrate account configuration, password requirements, and enabled status.
- Do not equate successful account creation with a successful user sign-in.
- Exclude temporary passwords and other credentials from public portfolio documentation.