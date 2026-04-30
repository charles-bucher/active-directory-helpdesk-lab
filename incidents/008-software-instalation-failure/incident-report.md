# 🎫 Incident Report – Software Installation Failure

## 📌 Ticket Information

* **Ticket ID:** INC-008
* **Title:** User Unable to Install Approved Software
* **Priority:** Medium
* **Status:** Resolved

---

## 👤 User Details

* **Name:** David Lee
* **Department:** Marketing
* **Request Type:** Software Installation

---

## 🧠 Issue Description

User reported failure when attempting to install approved company software. Installation process terminated with an error indicating insufficient permissions.

User required the software to complete assigned marketing tasks.

---

## 🔍 Investigation

* Confirmed installation failure and captured error message
* Verified software is approved for use within organization
* Checked user account permissions → standard user (no local admin rights)
* Reviewed system policies restricting software installation
* Confirmed installer file integrity and compatibility with operating system
* Verified sufficient disk space available

---

## 🛠️ Resolution Steps

1. Logged into workstation with administrative credentials
2. Re-ran installer using **“Run as administrator”**
3. Followed installation prompts and completed setup
4. Verified software installed in correct directory
5. Ensured application shortcuts were accessible to the user
6. Logged out of admin session and returned system to user

---

## ✅ Verification

* Launched application successfully
* Confirmed no errors during startup
* User tested core functionality → working as expected
* Confirmed user can access application without admin privileges

---

## 📎 Supporting Evidence

* Screenshot of installation error message
* Screenshot of successful installation completion
* Screenshot of application running

---

## 🧾 Notes

* Root cause identified as lack of administrative permissions
* Installation completed using authorized admin credentials
* Followed standard IT policy for software installation

---

## 🏁 Outcome

Software successfully installed and operational. User able to perform required tasks without further issues.
