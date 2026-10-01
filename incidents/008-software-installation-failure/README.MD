# 💻 Incident 008 – Software Installation Failure

This incident documents a simulated Tier 1 help desk case involving software installation failure on a Windows workstation within an Active Directory environment.

---

## 🧠 Scenario Overview

A user reported being unable to install approved software required for daily work tasks. The installation process terminated unexpectedly with an error related to permissions.

The issue was isolated to a single workstation and user account.

---

## 🔍 Key Symptoms

* Installation process fails mid-execution
* Error indicating insufficient permissions
* No successful application launch after install attempt
* Software installation blocked on standard user account

---

## 🛠️ Troubleshooting Focus Areas

This scenario simulates investigation of common software deployment issues:

* User privilege and local admin rights
* Software installation permissions
* System policy restrictions (GPO)
* Installer integrity and compatibility
* Windows security controls affecting execution

---

## ⚙️ Tools Used

* Windows Installer / setup executable
* Run as Administrator functionality
* Local user permissions review
* Group Policy awareness (installation restrictions)
* Basic system validation (disk space, compatibility checks)

---

## 🎯 Learning Outcomes

This incident demonstrates practical skills in:

* Diagnosing permission-based installation failures
* Understanding local vs administrative privilege boundaries
* Applying correct installation methods in Windows environments
* Recognizing policy-driven software restrictions
* Ensuring successful application deployment and validation

---

## 📎 Related Files

* `incident-report.md` → full step-by-step resolution
* Screenshots → installation error and successful completion evidence

---

## 🧭 Role Simulation Context

This scenario reflects a real Tier 1 help desk task where users frequently require assistance with software installation issues due to permission restrictions, policy enforcement, or configuration limitations in managed enterprise environments.
