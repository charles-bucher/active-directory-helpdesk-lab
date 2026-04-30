# 🎫 Incident Report – Network Connectivity Issue

## 📌 Ticket Information

* **Ticket ID:** INC-006
* **Title:** User Unable to Access Network Resources
* **Priority:** High
* **Status:** Resolved

---

## 👤 User Details

* **Name:** Michael Johnson
* **Department:** Operations
* **Request Type:** Network Connectivity

---

## 🧠 Issue Description

User reported inability to access internal network resources, including shared drives and web applications. The user also stated that internet access was unavailable.

Issue impacted productivity as the user could not perform daily tasks.

---

## 🔍 Investigation

* Confirmed issue by attempting to access internal resources from user’s workstation
* Verified no internet connectivity (web pages failed to load)
* Checked network icon status → indicated “No Internet Access”
* Ran `ipconfig` and identified missing/invalid IP address (APIPA range: 169.254.x.x)
* Attempted to ping default gateway → request timed out
* Tested network cable connection and physical link status
* Compared with another workstation on same network → functioning normally

---

## 🛠️ Resolution Steps

1. Inspected Ethernet cable connection and reseated cable
2. Switched to a known working Ethernet port
3. Ran `ipconfig /release` and `ipconfig /renew`
4. Confirmed system received valid IP address from DHCP server
5. Verified default gateway and DNS server assignment
6. Restarted workstation to ensure stable network configuration

---

## ✅ Verification

* Confirmed valid IP address assigned (non-APIPA range)
* Successfully pinged default gateway
* Successfully accessed internal shared drives
* Verified internet connectivity via web browser
* User confirmed full functionality restored

---

## 📎 Supporting Evidence

* Screenshot of `ipconfig` before (APIPA address)
* Screenshot of `ipconfig` after renewal (valid IP)
* Screenshot of successful ping to gateway

---

## 🧾 Notes

* Root cause identified as failure to obtain IP address from DHCP (likely due to port or connection issue)
* Issue resolved without escalation
* No broader network outage detected

---

## 🏁 Outcome

Network connectivity successfully restored. User regained access to both internal and external resources and resumed normal operations.
