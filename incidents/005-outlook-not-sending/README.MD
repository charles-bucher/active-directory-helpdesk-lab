# 🎫 Incident Report – Outlook Not Sending Emails

## 📌 Ticket Information

* **Ticket ID:** INC-005
* **Title:** Outlook Emails Stuck in Outbox / Not Sending
* **Priority:** High
* **Status:** Resolved

---

## 👤 User Details

* **Name:** Emily Carter
* **Department:** Finance
* **Device/System:** Windows 10 Workstation
* **Request Type:** Email / Outlook Issue

---

## 🧠 Issue Description

User reported that emails were not sending in Microsoft Outlook. Messages remained stuck in the Outbox and did not deliver to internal or external recipients.

Receiving emails was functioning normally. Issue began after user restarted their workstation.

---

## 🔍 Investigation

* Confirmed emails were stuck in Outbox
* Verified internet connectivity was stable
* Checked Outlook status bar and identified “Working Offline” mode enabled
* Reviewed Send/Receive settings and account configuration
* Verified mailbox storage quota was not exceeded
* Confirmed no password or authentication prompts were present
* Tested sending email after reconnecting to network (initial failure persisted)

---

## 🛠️ Resolution Steps

1. Opened Microsoft Outlook
2. Navigated to **Send/Receive tab**
3. Disabled **“Work Offline” mode**
4. Triggered manual **Send/Receive All Folders**
5. Monitored Outbox until queued messages began sending
6. Restarted Outlook to confirm persistent fix

---

## ✅ Verification

* Outbox cleared successfully
* Test email sent internally → delivered successfully
* Test email sent externally → delivered successfully
* User confirmed normal email functionality restored

---

## 📎 Supporting Evidence

* Screenshot of Outlook in “Work Offline” state
* Screenshot of Outbox with queued messages
* Screenshot of successful sent email confirmation

---

## 🧾 Notes / Root Cause

Root cause identified as Outlook being unintentionally set to **Offline Mode**, preventing message transmission.

No server-side or Exchange-level issues detected. Issue was client-side configuration.

---

## 🏁 Outcome

Email functionality fully restored. User able to send and receive emails without further issues.
