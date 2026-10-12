# ðŸŒ Incident 006: Network Connectivity Troubleshooting

## ðŸ§  Scenario Overview

This lab exercise documents the initial investigation of network configuration on a Windows virtual machine running in Oracle VirtualBox.

The objective is to inspect the assigned IP address and use standard troubleshooting commands to investigate network connectivity.

**Environment:** Windows virtual machine
**Virtualization:** Oracle VirtualBox
**Observed IPv4 address:** `10.0.2.15`

## ðŸ” Initial Findings

- Inspected the network configuration using `ipconfig`.
- Observed the IPv4 address `10.0.2.15`.
- Identified the need for additional testing to determine whether the gateway, DNS resolution, and external connectivity are functioning correctly.

The observed address is commonly used by VirtualBox's default NAT networking. It does not, by itself, indicate a network failure or DHCP problem.

## ðŸ› ï¸ Troubleshooting Focus Areas

The investigation can include:

- Inspecting adapter settings with `ipconfig /all`
- Identifying the default gateway and DNS servers
- Testing gateway reachability with `ping`
- Checking DNS resolution with `nslookup`
- Testing external connectivity, if applicable
- Recording results and capturing screenshots of actual command output

Only troubleshooting steps that have actually been performed should be documented as completed.

## âš™ï¸ Tools Used

- `ipconfig`
- `ipconfig /all`
- `ping`
- `nslookup`
- Oracle VirtualBox network settings

## ðŸŽ¯ Learning Outcomes

This exercise demonstrates:

- Reading and interpreting IPv4 configuration
- Understanding the difference between a private IPv4 address and an APIPA address
- Identifying the default gateway and DNS configuration
- Using command-line tools to investigate connectivity
- Documenting findings without assuming an unverified root cause

## ðŸ“Ž Related Files

- `incident-report.md` contains the investigation details and verification status.
- The `screenshots/` directory contains supporting evidence as it is captured and committed.

Add links to individual screenshots here only after confirming that the corresponding files exist in the repository.

## ðŸ§­ Tier 1 Help Desk Context

Network troubleshooting is a common Tier 1 support responsibility. A structured investigation helps determine whether a problem involves local IP configuration, gateway connectivity, DNS resolution, or external network access.

**Current status:** Initial IP configuration documented. Further connectivity testing is required before confirming a fault or resolution.
