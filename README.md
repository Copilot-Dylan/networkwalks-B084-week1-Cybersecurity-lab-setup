# Cybersecurity Lab setup

## Overview
This simple project focuses on setting up virtual cybersecurity environment lab using virtual box and kali linux for testing and other cybersecurity purposes.

---

## Objectives
- Install VirtualBox.
- Install Kali Linux as a virtual machine.
- Create a private NAT Network for the cybersecurity lab.
- Configure network connectivity for Kali Linux.
- Assign a consistent IP address to the Kali VM.
- Verify network connectivity and DNS resolution.
- Take a snapshot for recovery in virtual box.
  
---

# Lab setup Process

## Step 1. Install Z-zip
7-Zip was installed from its official website for the extraction of the Kali Linux virtual-machine package.

## Step 2. Install VirtualBox
Oracle VirtualBox was installed in which the lab was created.

## Step 3. Create NAT Network
A dedicated NAT Network was created in VirtualBox with the below configuration:

Configuration:
Network Name: NatNetwork
IPv4 Prefix:  10.0.0.0/24
DHCP:         Enabled
IPv6:         Disabled

NAT Network was selected because multiple virtual machines connected to the same NAT Network can communicate with one another while also having outbound network connectivity allowing future attacker and target VMs to communicate within the lab.

## Step 4. Import Kali Linux
The Kali Linux virtual machine was downloaded from the official Kali Linux website and imported into VirtualBox.

## Step 5. Configure the Kali Linux Network
The Kali Linux network configuration was configured with a consistent IPv4 address as a consistent IP address makes it easier to document the lab and reference the Kali machine in future exercises.

## Step 6. Create a VM Snapshot
After completing the initial configuration, a VirtualBox snapshot was created. The snapshot represents the baseline of the lab. Incase if the VM configuration is changed or damaged in the future, the machine can be restored to this baseline or state.

---

## Learnings and Insights
Through this project, I learned how to create and configure a virtual environment for cybersecurity practice.
And I also learned different concepts like NAT network, Static IP configuration, VM Snapshots, Clean documentation, etc.

