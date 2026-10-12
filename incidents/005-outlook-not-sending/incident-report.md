# 🧾 Incident Report: Outlook Send Failure During Wi-Fi Interruption

## Ticket Information

**Ticket ID:** `INC-005`  
**Issue Type:** Email / Outlook Troubleshooting  
**Environment:** New Outlook for Windows  
**Status:** Recovery observed; recipient delivery not independently verified

## 🧩 Summary

A controlled troubleshooting exercise was performed to observe Outlook's email-sending behavior during a temporary Wi-Fi interruption.

A test email was prepared in New Outlook. Wi-Fi was disconnected before the user attempted to send it, and Outlook displayed an error. After Wi-Fi was restored, the test message was located in Sent Items.

The evidence documents the connection interruption and the subsequent appearance of the message in Sent Items. Delivery to the recipient was not independently confirmed.

## 📌 Request Details

- **Scenario:** Test email encountered a sending problem during a network interruption.
- **Application:** New Outlook for Windows
- **Connection:** Wi-Fi
- **Test subject:** `LAB TEST - INC-005 Outlook Troubleshooting`
- **Impact:** Test message sending was interrupted during the controlled exercise.

This was a simulated lab scenario, not a report of a verified production-user incident.

## 🖥️ Environment

- **Operating system:** Windows
- **Email application:** New Outlook
- **Network connection:** Wi-Fi
- **Test mailbox:** User's own mailbox
- **Evidence tools:** Windows Snipping Tool and Git

## 🔍 Symptoms

- A test email was prepared in Outlook.
- Wi-Fi was disconnected before the send attempt.
- Outlook displayed an error during the test.
- The user initially observed the message in Archive.
- After Wi-Fi was restored, the message was found in Sent Items.

The exact error text was not recorded in the incident notes, so no specific Outlook error code is claimed.

## ⚙️ Troubleshooting Steps

1. Opened New Outlook and accessed the inbox.
2. Created a test email addressed to the user's own mailbox.
3. Used the subject `LAB TEST - INC-005 Outlook Troubleshooting`.
4. Disconnected Wi-Fi for a controlled network-interruption test.
5. Attempted to send the test email and captured the resulting error.
6. Restored the Wi-Fi connection.
7. Located the test message in Sent Items and captured a screenshot.

## 🧪 Validation

**Observed:**
- Outlook displayed an error during the disconnected-network test.
- After Wi-Fi was restored, the test message appeared in Sent Items.

**Not independently verified:**
- Receipt of the message in the destination inbox.
- Successful delivery beyond the Sent Items state.
- Whether the original error was caused exclusively by the Wi-Fi interruption.

The test demonstrates the observed behavior and recovery sequence, but does not establish a broader email-service root cause.

## ✅ Outcome

The test message was located in Sent Items after network connectivity was restored.

**Final status:** Recovery observed; recipient delivery not independently verified.

## 📎 Screenshot Evidence

1. `screenshots/005-outlook-not-sending/005-outlook-network-failure.png`  
   Captures the sending error during the Wi-Fi interruption.

2. `screenshots/005-outlook-send-success/005-outlook-send-success.png`  
   Captures the test message in Sent Items after Wi-Fi was restored.

## 🧠 Lessons Learned

- Check network connectivity when troubleshooting email-sending failures.
- Distinguish an error observed during a test from a confirmed root cause.
- Verify the message's actual folder and status before reporting a resolution.
- A message appearing in Sent Items is not the same as independently confirming delivery.
- Keep incident reports aligned with captured evidence.
