# Incident Report: Outlook Unable to Send Emails

## Ticket Information

- **Ticket ID:** `INC-005`
- **Title:** Outlook Emails Stuck in Outbox
- **Priority:** High
- **Status:** Resolved, pending any verification not yet completed
- **Category:** Email / Microsoft Outlook

## User Details

- **Affected User:** `Jane Smith` (lab scenario)
- **Department:** Finance (lab scenario)
- **Request Type:** Email Issue

## Issue Description

The user reported that Microsoft Outlook was not sending email messages. Messages remained in the Outbox, preventing them from being sent.

The objective was to investigate Outlook's connection state, restore normal sending behavior, and verify the outcome.

## Environment

- **Application:** Microsoft Outlook
- **User Account:** Lab user account
- **Network:** Lab environment
- **Troubleshooting Tools:** Outlook Send/Receive settings and application status indicators

## Symptoms

- Email messages remained in the Outbox.
- Sending messages did not complete as expected.
- Outlook displayed the **Work Offline** state.

## Investigation

1. Reviewed the Outlook status indicator.
2. Identified that **Work Offline** mode was enabled.
3. Checked the application's Send/Receive controls.
4. Considered network connectivity and account authentication as alternative causes.

## Root Cause

Outlook was in **Work Offline** mode, preventing normal online sending behavior.

## Resolution Steps

1. Opened Microsoft Outlook.
2. Selected the **Send/Receive** tab.
3. Disabled **Work Offline** mode.
4. Initiated **Send/Receive All Folders**.
5. Checked whether queued messages began sending.
6. Reopened Outlook, if performed, to check whether normal sending behavior continued.

## Verification

Verify and document the checks actually completed:

- [ ] Confirmed the Outbox cleared.
- [ ] Sent a test email to an internal recipient.
- [ ] Confirmed successful delivery.
- [ ] Sent a test email to an external recipient.
- [ ] Confirmed successful delivery.
- [ ] Confirmed normal sending behavior after restarting Outlook, if tested.

Only mark a check complete after observing the result.

## Screenshot Evidence

The screenshot folders in the repository are named `005-outlook-work-offline` and `005-outlook-send-success`.

### 1. Outlook Work Offline

**Evidence folder:** `screenshots/005-outlook-work-offline/`

Shows Outlook's offline state before the corrective action.

### 2. Outlook Send Success

**Evidence folder:** `screenshots/005-outlook-send-success/`

Shows evidence of the sending process after troubleshooting.

> **Note:** Confirm the image filenames and extensions inside these folders before adding Markdown image embeds. The folder names alone do not establish the exact image paths.

## Skills Demonstrated

- Microsoft Outlook troubleshooting
- Investigating email delivery problems
- Identifying application connection states
- Using Send/Receive controls
- Testing corrective actions
- Documenting incident resolution
- Capturing supporting technical evidence

## Outcome

The incident documents the investigation of Outlook's offline state and the corrective action taken to restore normal sending behavior. The incident should remain marked **Resolved** once the successful outcome