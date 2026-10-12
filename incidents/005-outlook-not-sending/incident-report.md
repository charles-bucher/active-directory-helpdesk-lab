# 🧾 Incident Report: Outlook Send Failure During Wi-Fi Interruption

## 🎫 Ticket Information

- **Ticket ID:** `INC-005-outlook-not-sending`
- **Issue Type:** Email / Outlook Troubleshooting
- **Priority:** Medium
- **Application:** New Outlook for Windows
- **Status:** Recovery observed; recipient delivery not independently verified

## 🧩 Summary

A controlled troubleshooting exercise was performed to observe Outlook's email-sending behavior during a temporary Wi-Fi interruption.

A test email was prepared in New Outlook. Wi-Fi was disconnected before the send attempt, and Outlook displayed an error. After Wi-Fi connectivity was restored, the test message was located in Sent Items.

The available evidence documents the connection interruption and the subsequent appearance of the message in Sent Items. Delivery to the recipient was not independently confirmed.

## 📌 Request Details

- **Scenario:** Test email encountered a sending problem during a network interruption.
- **Application:** New Outlook for Windows
- **Connection:** Wi-Fi
- **Test Subject:** `LAB TEST - INC-005 Outlook Troubleshooting`
- **Impact:** The test email encountered a sending problem during the controlled exercise.

This was a simulated lab scenario, not a verified production-user incident.

## 🖥️ Environment

- **Operating System:** Windows
- **Email Application:** New Outlook
- **Network Connection:** Wi-Fi
- **Test Mailbox:** User's own mailbox
- **Evidence Tools:** Windows Snipping Tool and Git

## 🔍 Symptoms and Observations

- A test email was prepared in Outlook.
- Wi-Fi was disconnected before the send attempt.
- Outlook displayed an error during the test.
- The message was initially observed in Archive.
- After Wi-Fi was restored, the message was located in Sent Items.

The exact Outlook error text was not recorded, so no specific error code or underlying application fault is claimed.

## ⚙️ Troubleshooting Steps

1. Opened New Outlook and accessed the mailbox.
2. Created a test email addressed to the user's own mailbox.
3. Entered the subject `LAB TEST - INC-005 Outlook Troubleshooting`.
4. Disconnected Wi-Fi for a controlled network-interruption test.
5. Attempted to send the test email and captured the resulting error.
6. Restored Wi-Fi connectivity.
7. Located the test message in Sent Items and captured screenshot evidence.

## 🧪 Validation

**Observed:**

- Outlook displayed an error during the disconnected-network test.
- After Wi-Fi connectivity was restored, the test message appeared in Sent Items.

**Not independently verified:**

- Receipt of the message in the destination inbox.
- Successful delivery beyond the Sent Items state.
- Whether the Wi-Fi interruption was the sole cause of the original error.

The evidence supports the observed troubleshooting sequence but does not establish a broader email-service root cause.

## ✅ Outcome

The test message was located in Sent Items after Wi-Fi connectivity was restored.

**Final Status:** Recovery observed; recipient delivery not independently verified.

## 📎 Screenshot Evidence

### 1. Outlook Network Failure

`005-outlook-network-failure.png`

Path: `screenshots/005-outlook-not-sending/005-outlook-network-failure.png`

Captures the sending error during the Wi-Fi interruption.

### 2. Outlook Send Success

`005-outlook-send-success.png`

Path: `screenshots/005-outlook-send-success/005-outlook-send-success.png`

Captures the test message in Sent Items after Wi-Fi was restored.

Confirm that both paths match the actual files in the repository.

## 🧠 Lessons Learned

- Check network connectivity when troubleshooting email-sending failures.
- Distinguish a test condition from a confirmed technical root cause.
- Verify the message's folder and status before documenting recovery.
- A message appearing in Sent Items does not independently confirm recipient delivery.
- Keep incident documentation aligned with captured evidence.