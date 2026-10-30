# Cybersecurity Lab Setup — NetworkWalks Week 1

## Project Overview

This project documents the setup and verification of a cybersecurity lab environment using VirtualBox and Kali Linux as part of the NetworkWalks Cybersecurity & Ethical Hacking training program.

The objective is to prepare a virtual environment for future cybersecurity and ethical hacking exercises.

## Objectives

- Configure a NAT Network in VirtualBox.
- Install and configure Kali Linux.
- Assign the required static IP address.
- Verify network and internet connectivity.
- Configure clipboard, drag-and-drop, and shared-folder functionality.
- Create a VM snapshot for recovery.

## Lab Architecture

| Component | Configuration |
|---|---|
| Host OS | Windows |
| Virtualization platform | VirtualBox |
| Virtual machine | Kali Linux |
| Network type | NAT Network |
| Network subnet | `10.0.0.0/24` |
| Kali Linux IP | `10.0.0.2/24` |
| Expected gateway | `10.0.0.1` |
| Shared folder | `/downloads` |

## Implementation and Verification

### 1. Virtual Network Configuration

Configured the VirtualBox NAT Network using the required subnet.

**Evidence:** `screenshots/01-virtualbox-nat-network.png`

### 2. Kali Linux Configuration

Configured the Kali Linux virtual machine and verified its network interface and IP address.

**Evidence:** `screenshots/03-kali-ip-configuration.png`

### 3. Network Connectivity

The following commands were used to test connectivity and inspect the network configuration.

```bash
ip -br address
ip route
ping -c 4 10.0.0.1
ping -c 4 8.8.8.8
getent hosts google.com
```

**Results:** Update this section with the actual results of each test.

**Evidence:** Add links to the relevant screenshots.

### 4. Shared Folder and VM Settings

Configured the required VirtualBox integration settings and shared-folder access.

**Evidence:** Add the relevant screenshots after verification.

### 5. VM Snapshot

Created a snapshot to preserve the configured lab environment for recovery.

**Evidence:** `screenshots/07-vm-snapshot.png`

## Troubleshooting

Document any issues encountered during setup, the commands or configuration changes used to investigate them, and the results.

Do not include unverified fixes or claim that an issue was resolved unless you confirmed the result.

## Key Learnings

- Virtualization and virtual machine management.
- NAT networking and IP addressing.
- Linux network configuration and troubleshooting.
- Connectivity testing and DNS resolution.
- Virtual machine snapshots and recovery.

## Project Status

Update this section as each requirement is completed and verified.

## Training Program

NetworkWalks — Cybersecurity & Ethical Hacking Training

Project Module 1: Lab Setup VirtualBox and Kali Linux.
