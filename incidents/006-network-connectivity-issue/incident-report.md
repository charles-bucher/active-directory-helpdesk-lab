# 🎫 Incident Report: Network Connectivity Troubleshooting

## 📌 Ticket Information

- **Ticket ID:** `INC-006-network-connectivity`
- **Issue Type:** Network Configuration / Connectivity Troubleshooting
- **Priority:** Medium
- **Environment:** Windows virtual machine running in Oracle VirtualBox
- **Status:** Initial IP configuration documented; connectivity verification pending

## 🧠 Summary

This lab exercise documents the initial investigation of network configuration on a Windows virtual machine.

The objective is to inspect the assigned IP address and use standard troubleshooting commands to determine whether the default gateway, DNS resolution, and external network connectivity are functioning.

The available command output shows the IPv4 address `10.0.2.15`. This address is commonly associated with VirtualBox's default NAT networking and does not, by itself, indicate a network fault.

## 🖥️ Lab Environment

- **Platform:** Oracle VirtualBox
- **Operating System:** Windows
- **Network Configuration:** VirtualBox virtual network adapter
- **Tools:** Command Prompt, `ipconfig`, `ping`, and `nslookup`

## 🔍 Investigation Performed

1. Opened Command Prompt in the Windows virtual machine.
2. Ran `ipconfig` to inspect the current network configuration.
3. Observed the IPv4 address `10.0.2.15`.
4. Documented the observed address for further connectivity investigation.

## 🛠️ Next Troubleshooting Steps

The following checks remain to be performed and documented:

1. Run `ipconfig /all` to inspect the adapter, subnet mask, default gateway, and DNS servers.
2. Ping the configured default gateway to test gateway reachability.
3. Run `nslookup` against a known domain to test DNS resolution.
4. Test external connectivity if the virtual machine is expected to have internet access.
5. Capture screenshots of the actual command output and record the results.

These are planned checks, not completed actions. Update this section as each test is performed.

## 🧪 Verification

**Confirmed by the available command output:**

- The virtual machine has the IPv4 address `10.0.2.15`.

**Not yet established:**

- Whether the default gateway is reachable.
- Whether DNS resolution is working.
- Whether external network access is available.
- Whether a network fault occurred or was successfully resolved.

## 📎 Supporting Evidence

The following are intended screenshot filenames. Confirm each file exists and is committed before adding a link to it.

- `screenshots/006-network-connectivity-issue/006-ipconfig-before.png`
- `screenshots/006-network-connectivity-issue/006-ipconfig-after.png`
- `screenshots/006-network-connectivity-issue/006-connectivity-verified.png`

## 🧾 Technical Notes

The IPv4 address `10.0.2.15` is commonly assigned to virtual machines using VirtualBox's default NAT configuration. It is not an APIPA address.

An IPv4 address in the `169.254.x.x` range is a link-local address that can indicate a failure to obtain a DHCP lease. The available evidence does not show that condition.

## 🧠 Skills Demonstrated

- Inspecting Windows IP configuration
- Understanding private IPv4 and APIPA addressing
- Identifying gateway and DNS configuration
- Using command-line network troubleshooting tools
- Recording evidence without assuming an unverified root cause

## 🏁 Outcome

The initial IP configuration was inspected, and the assigned IPv4 address was documented. Additional connectivity tests are required before a network fault, root cause, or successful resolution can be confirmed.

**Final Status:** Initial investigation documented; connectivity verification pending.