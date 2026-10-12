# 🖨️ Incident Report: Printer Connectivity and Queue Troubleshooting

## 🎫 Ticket Information

- **Ticket ID:** `INC-007-printer-not-working`
- **Issue Type:** Printer / Printing Troubleshooting
- **Priority:** Medium
- **Environment:** Windows support lab
- **Status:** Investigation documented; resolution requires supporting evidence

## 🧩 Summary

This lab scenario covers troubleshooting a reported printing problem in which print jobs remain in the queue and the printer may appear offline on the workstation.

The investigation focuses on distinguishing workstation configuration problems from printer, network, and print-spooler issues.

The exact root cause and successful restoration of printing should only be recorded after the relevant checks and tests have been completed.

## 📌 Issue Description

A simulated user reports being unable to print to a shared network printer. Print jobs may remain queued instead of completing.

**Potential impact:** Delayed printing of business documents.

## 🖥️ Environment

- **Operating System:** Windows
- **Printer Type:** Shared network printer
- **Troubleshooting Tools:** Windows printer settings, print queue, Print Spooler service, and printer connection settings

## 🔍 Investigation

The following checks can be used to investigate the reported issue:

1. Inspect the print queue for stuck or pending jobs.
2. Check the printer's displayed status.
3. Confirm that the workstation has network connectivity.
4. Review the printer's configured connection or shared printer path.
5. Check the Print Spooler service if queue processing appears stalled.
6. Determine whether the problem affects one workstation or multiple users.

Record only checks that have actually been performed and results that have been observed.

## 🛠️ Troubleshooting and Resolution

If an incorrect or outdated printer connection is confirmed, the corrective workflow may include:

1. Open the Windows printer settings.
2. Review the existing shared printer connection.
3. Remove the outdated connection if appropriate.
4. Add the correct shared printer path.
5. Check the Print Spooler service if necessary.
6. Submit a test print and inspect the result.

The actual corrective action and final outcome must be updated to match the work completed in the lab.

## 🧪 Verification

**Evidence to capture:**

- The initial printer status or queue condition.
- The printer connection or configuration being investigated.
- The final printer status after troubleshooting.
- A successful test print, if performed.

A printer showing **Ready** does not, by itself, prove that a document printed successfully.

## 📎 Supporting Evidence

Add screenshots to the repository after capturing and verifying the files.

Suggested evidence:

- `screenshots/007-printer-not-working/007-printer-queue-before.png`
- `screenshots/007-printer-not-working/007-printer-offline.png`
- `screenshots/007-printer-not-working/007-printer-test-print-success.png`

These are suggested filenames, not confirmation that the files already exist.

## 🧠 Lessons Learned

- Inspect the print queue before changing printer settings.
- Check whether the issue is isolated to one workstation.
- Verify the configured shared printer path.
- Restart services only when troubleshooting findings justify it.
- Use a test print to validate actual printing functionality.
- Document the observed root cause and evidence-supported outcome.

## 🏁 Outcome

This incident documents a Tier 1 printer-troubleshooting workflow. The root cause and successful restoration of printing remain unconfirmed until supported by actual lab results and evidence.

**Final Status:** Investigation documented; resolution pending verification.