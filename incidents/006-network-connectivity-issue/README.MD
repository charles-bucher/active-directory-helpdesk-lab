# 🌐 Incident 006 – Network Connectivity Issue

This incident documents a simulated Tier 1 help desk case involving complete loss of network and internet connectivity on a Windows workstation within an Active Directory environment.

---

## 🧠 Scenario Overview

A user reported being unable to access any network resources, including:

* Internal file shares
* Web applications
* Internet browsing

The issue was isolated to a single workstation, while other users in the same environment remained unaffected.

---

## 🔍 Key Symptoms

* No internet connectivity
* “No Internet Access” network status
* APIPA address assigned (169.254.x.x)
* Failed ping to default gateway
* Loss of access to internal network resources

---

## 🛠️ Troubleshooting Focus Areas

This incident simulates investigation across common network failure points:

* DHCP lease assignment failure
* Network adapter configuration issues
* Physical connectivity validation
* Local endpoint vs network-wide outage isolation
* IP addressing and gateway validation

---

## ⚙️ Tools Used

* `ipconfig` (IP configuration analysis)
* `ping` (connectivity testing)
* Windows Network Status diagnostics
* Physical port/cable validation
* DHCP lease renewal process

---

## 🎯 Learning Outcomes

This scenario demonstrates practical skills in:

* Identifying DHCP-related failures (APIPA detection)
* Differentiating endpoint vs infrastructure issues
* Basic network troubleshooting methodology
* Use of command-line diagnostic tools
* Structured problem isolation approach

---

## 📎 Related Files

* `incident-report.md` → full step-by-step resolution
* Screenshots → before/after IP configuration and connectivity tests

---

## 🧭 Role Simulation Context

This incident simulates a real Tier 1 Help Desk ticket in a corporate Active Directory environment, where rapid isolation of connectivity issues is critical to restoring user productivity.
