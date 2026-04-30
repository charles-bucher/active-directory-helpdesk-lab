# 🎫 Incident Report – Printer Not Working

## 📌 Ticket Information

* **Ticket ID:** INC-007
* **Title:** User Unable to Print to Network Printer
* **Priority:** Medium
* **Status:** Resolved

---

## 👤 User Details

* **Name:** Sarah Williams
* **Department:** Human Resources
* **Request Type:** Printing Issue

---

## 🧠 Issue Description

User reported that print jobs were not being processed when attempting to print to a shared network printer. Documents remained in the print queue and did not reach the printer.

Issue impacted ability to print important HR documents.

---

## 🔍 Investigation

* Confirmed issue by sending test print → job remained in queue
* Checked printer status → device showed as “Offline” on user workstation
* Verified other users were able to print successfully → ruled out printer hardware failure
* Checked network connectivity → user workstation connected to network
* Restarted Print Spooler service → no change
* Reviewed printer mapping and identified incorrect/outdated printer connection

---

## 🛠️ Resolution Steps

1. Opened **Devices and Printers** on user workstation
2. Removed existing network printer
3. Re-added printer using correct network path (\print-server\HR-Printer)
4. Restarted **Print Spooler** service
5. Sent test print job

---

## ✅ Verification

* Confirmed printer status displayed as “Ready”
* Test document printed successfully
* Cleared stuck print queue
* User confirmed ability to print normally

---

## 📎 Supporting Evidence

* Screenshot of stuck print queue
* Screenshot of printer showing “Offline” status
* Screenshot of successful test print

---

## 🧾 Notes

* Issue caused by incorrect or stale printer mapping
* No hardware issues identified
* No escalation required

---

## 🏁 Outcome

Printer functionality restored. User successfully able to print documents without further issues.
