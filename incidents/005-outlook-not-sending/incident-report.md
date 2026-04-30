# 🎫 Incident Report – Outlook Not Sending Emails

## 📌 Ticket Information

* **Ticket ID:** INC-005
* **Title:** User Unable to Send Emails in Outlook
* **Priority:** High
* **Status:** Resolved

---

## 👤 User Details

* **Name:** Jane Smith
* **Department:** Finance
* **Request Type:** Email Issue

---

## 🧠 Issue Description

User reported that emails in Microsoft Outlook were not sending. Messages remained stuck in the Outbox, and new emails could not be delivered.

Receiving emails was functioning normally.

---

## 🔍 Investigation

* Confirmed issue by observing multiple emails stuck in the Outbox
* Verified internet connectivity was active
* Checked Outlook status bar and identified “Working Offline” mode enabled
* Reviewed Send/Receive settings
* Confirmed mailbox was not over quota
* Verified no credential prompts or authentication failures

---

## 🛠️ Resolution Steps

1. Opened Microsoft Outlook
2. Navigated to **Send/Receive** tab
3. Disabled **“Work Offline”** mode
4. Initiated manual **Send/Receive All Folders**
5. Monitored Outbox as queued emails began sending
6. Restarted Outlook to ensure settings persisted

---

## ✅ Verification

* Confirmed Outbox cleared successfully
* Sent test email to internal user → delivered successfully
* Sent test email to external address → delivered successfully
* User confirmed ability to send emails normally

---

## 📎 Supporting Evidence

* Screenshot of Outlook in “Work Offline” mode
* Screenshot of Outbox before and after resolution
* Screenshot of successful sent email

---

## 🧾 Notes

* Issue caused by Outlook being in offline mode, likely enabled unintentionally
* No server-side or account issues identified
* No escalation required

---

## 🏁 Outcome

Email functionality restored. User able to send and receive emails without further issues.
