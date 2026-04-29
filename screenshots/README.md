📎 Evidence Documentation
Purpose

This section provides visual proof of actions performed within the lab environment. Evidence is included to validate configuration changes, troubleshooting steps, and final system state after resolution.

🖥️ Evidence Types Included

The following types of screenshots may be included in each incident report:

Active Directory Users and Computers (ADUC) showing user/account status
Account properties (enabled/disabled, password status, group membership)
Login or authentication behavior (where applicable in simulation)
System configuration changes in Windows Server environment
Confirmation of successful resolution (final state verification)
📂 File Naming Convention

All evidence files follow a consistent naming format:

[TICKET-ID]_[short-description].png
Example:
INC-001-user-creation_aduc-user-list.png
INC-002-password-reset_aduc.png
INC-003-account-locked_aduc.png

This ensures traceability between incident documentation and supporting evidence.

🔍 Validation Standard

Each screenshot should clearly show:

Relevant system interface (e.g., ADUC console)
Visible user or object being referenced (e.g., jdoe account)
Status indicators (enabled, locked, group membership, etc.)
Context confirming the action described in the ticket

Screenshots are used to support:

Troubleshooting steps
Configuration changes
Final resolution confirmation
🧠 Notes
Evidence should be captured immediately after completing each major action
Only relevant windows should be included (avoid unnecessary UI clutter)
Each incident should include at least one supporting screenshot for verification
Evidence is treated as part of the audit trail for each ticket