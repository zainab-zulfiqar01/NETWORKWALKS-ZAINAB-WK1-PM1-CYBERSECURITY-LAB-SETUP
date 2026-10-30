# NETWORKWALKS-ZAINAB-WK1-PM1-CYBERSECURITY-LAB-SETUP
Week 1 Project Module 1 - Cybersecurity Lab Setup using VMware and Kali Linux

## 📌 Project Overview

In this project, I set up a cybersecurity testing lab using VMware Workstation Pro and Kali Linux.

The goal was to prepare a virtual environment for learning and practicing cybersecurity concepts, network configuration and ethical hacking activities.

## 🎯 Objectives

- Set up Kali Linux in VMware Workstation Pro.
- Configure the VMware NAT network.
- Assign a static IP address to Kali Linux.
- Configure network connectivity.
- Enable clipboard and drag-and-drop.
- Set up a shared folder.
- Prepare the lab for future cybersecurity tasks.

## 🛡️ Purpose of the Lab

This lab provides a virtual environment where I can practice:

- Network scanning
- Reconnaissance
- Vulnerability assessment
- Web security testing
- Cybersecurity tools

**Note:** All testing should only be performed on authorized systems.

## 🏗️ Lab Architecture

The lab uses VMware Workstation Pro to run Kali Linux as a virtual machine. The Kali machine is connected through the VMware NAT network (VMnet8).

## ⚙️ Lab Configuration

| Component | Configuration |
|---|---|
| Host OS | Windows 11 |
| Processor | Intel Core i7-1355U |
| Hypervisor | VMware Workstation Pro |
| Security OS | Kali Linux |
| Network Type | NAT (VMnet8) |
| Network Address | 10.0.0.0/24 |
| Kali IP | 10.0.0.2/24 |
| Gateway | 10.0.0.254 |
| DNS | 8.8.8.8 |

## 🪜 Lab Setup Procedure

### Step 1. Install 7-Zip

I used 7-Zip to extract the downloaded Kali Linux virtual machine files.

### Step 2. Install VMware Workstation Pro

VMware Workstation Pro was used to create and manage the Kali Linux virtual machine.

### Step 3. Configure NAT Network

I configured the VMware virtual network using VMnet8 with NAT networking.

This allows Kali Linux to access the network through the host computer.

**Screenshot 1: VMware Network Settings**

![VMware Network Settings](VMware%20Network%20Settings.png)

### Step 4. Download and Open Kali Linux

I downloaded the Kali Linux VMware image from the official website, extracted it and opened the virtual machine in VMware Workstation Pro.

**Screenshot 2: Kali Linux in VMware**

![Kali Linux in VMware](Kali%20Linux%20in%20VMware.png)

### Step 5. Configure Network Adapter

I selected NAT as the network connection for the Kali Linux virtual machine and enabled the Connected and Connect at power on options.

### Step 6. Enable Clipboard and Shared Folder

I enabled copy-and-paste and drag-and-drop through VMware Guest Isolation settings. I also configured a shared folder to transfer files between Windows and Kali Linux.

### Step 7. Configure Kali Linux IP Address

I configured the IPv4 settings manually with the following details:

- IP Address: 10.0.0.2
- Subnet Mask: 255.255.255.0
- Gateway: 10.0.0.254
- DNS: 8.8.8.8

**Screenshot 3: Kali Linux Network Settings**

![Kali Network Settings](Kali%20Network%20Settings.png)

### Step 8. Verify Network Configuration

I used the following command to check the assigned IP address:

```bash
ip a
```

**Screenshot 4: Kali Linux IP Configuration**

![Kali Linux IP Configuration](Kali%20Linux%20IP%20Configuration.png)
### Step 9. Create a VM Snapshot

After configuring the virtual machine, I created a snapshot in VMware Workstation Pro so I could restore the lab to its initial state if needed.

## 🔎 Lab Verification

| Test | Command |
|---|---|
| Check IP Address | `ip a` |
| Check Gateway | `ping -c 4 10.0.0.254` |
| Check Internet | `ping -c 4 8.8.8.8` |
| Check DNS | `ping -c 4 google.com` |

## 🐞 Troubleshooting

During setup, network connectivity may require checking after manual IP configuration.

I checked the network adapter, IP address, gateway and DNS settings to identify possible configuration issues.

## 💡 What I Learned

Through this project, I learned how to:

1. Work with VMware Workstation Pro.
2. Set up Kali Linux as a virtual machine.
3. Configure NAT networking.
4. Assign a static IP address.
5. Use basic Linux networking commands.
6. Configure VMware integration features.
7. Create a virtual machine snapshot.

## 🔐 Security & Ethical Use

This lab is for educational purposes and authorized cybersecurity practice only.

## 🔗 Tools & Resources

- 7-Zip: https://www.7-zip.org/
- VMware Workstation: https://www.vmware.com/
- Kali Linux: https://www.kali.org/get-kali/

## 👤 Author

**Zainab Zulfiqar**

Ethical Hacking Intern  
Networkwalks

## 📌 Project Information

- Program: Networkwalks Cybersecurity Internship
- Week: 01
- Project Module: WK1-PM1
- Project: Cybersecurity Lab Setup
- Platform: VMware Workstation Pro
- Operating System: Kali Linux

*Learning and building practical cybersecurity skills through hands-on projects.*
