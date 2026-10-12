# 💿 Incident Report: Software Installation Failure

## 🎫 Ticket Information

- **Ticket ID:** `INC-008-software-installation`
- **Title:** User Unable to Install Approved Software
- **Priority:** Medium
- **Environment:** Windows Server lab
- **Status:** Installation troubleshooting documented; final verification pending

## 👤 User Details

- **Name:** David Lee
- **Department:** Marketing
- **Request Type:** Software Installation

*David Lee is a simulated user for this lab exercise.*

## 🧠 Issue Description

The simulated user reports that an attempted software installation fails with a permissions-related error.

The objective is to investigate the installation failure, identify the relevant permission or policy restriction, and determine an appropriate resolution.

## 🔍 Investigation

The troubleshooting workflow includes:

1. Review the installation error message.
2. Determine whether the software is approved for use.
3. Review the account permissions relevant to the installation.
4. Check applicable installation policies.
5. Confirm installer compatibility and available disk space.

Only checks actually performed should be recorded as completed findings.

## 🛠️ Troubleshooting and Resolution

When administrative permissions are confirmed as the cause and the installation is authorized:

1. Use an approved administrative account or authorized elevation method.
2. Run the installer with the required permissions.
3. Follow the installation prompts.
4. Confirm the installation completes successfully.
5. Verify the installed application can be accessed by the intended user.

Administrative credentials should not be shared with the user. Any elevation must follow the organization's software installation policy.

## ✅ Verification

The final verification should establish:

- Whether the installer completed successfully.
- Whether the application appears in the expected installation location.
- Whether the application launches without errors.
- Whether the intended user can access the application.

A successful installation dialog alone does not prove that the application launches or works correctly.

## 📎 Supporting Evidence

Suggested screenshot locations:

- `screenshots/008-software-installation-failure/008-software-installation-failure.png`
- `screenshots/008-software-installation-failure/008-software-installation-success.png`

Add an application-launch screenshot only if you capture one.

These paths are suggested until the actual files are confirmed.

## 🧠 Technical Notes

- Standard user accounts may lack permission to install certain applications.
- Installation failures can also result from application policy, compatibility, installer integrity, or other restrictions.
- Administrative elevation should only be used when authorized.
- The documented root cause must match the observed error and troubleshooting results.

## 🏁 Outcome

This incident demonstrates a Tier 1 software-installation troubleshooting workflow. The confirmed cause, corrective action, and final operational status should be updated to reflect the actual lab results and available screenshots.
