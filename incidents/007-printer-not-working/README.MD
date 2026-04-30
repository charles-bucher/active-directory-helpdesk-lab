# 🖨️ Incident 007 – Printer Not Working

This incident documents a simulated Tier 1 help desk case involving network printer failure in an Active Directory environment.

---

## 🧠 Scenario Overview

A user reported being unable to print documents to a shared network printer. Print jobs were sent successfully from the workstation but did not reach the printer or were stuck in the queue.

The issue was isolated to a single user workstation.

---

## 🔍 Key Symptoms

* Print jobs stuck in queue
* Printer status showing “Offline”
* Documents not reaching network printer
* No error messages from application

---

## 🛠️ Troubleshooting Focus Areas

This scenario simulates investigation of common printing issues:

* Stale or incorrect printer mappings
* Print spooler service behavior
* Network printer connectivity
* Queue congestion and stuck jobs
* Driver or configuration mismatches

---

## ⚙️ Tools Used

* Devices and Printers (Windows Control Panel)
* Print Spooler service management
* Network printer path validation (`\\print-server\printer-name`)
* Basic connectivity checks
* Print queue inspection

---

## 🎯 Learning Outcomes

This incident demonstrates practical skills in:

* Troubleshooting network printer issues
* Managing and resetting print queues
* Understanding print spooler service behavior
* Reconfiguring shared printer connections
* Isolating endpoint vs server-side printing issues

---

## 📎 Related Files

* `incident-report.md` → full step-by-step resolution
* Screenshots → printer status, queue behavior, and successful test print

---

## 🧭 Role Simulation Context

This scenario reflects a real-world Tier 1 help desk environment where printer issues are a common and recurring support ticket type. Proper diagnosis prevents unnecessary escalation to infrastructure teams.
