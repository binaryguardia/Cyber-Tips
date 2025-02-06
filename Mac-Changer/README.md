# macchanger Guide

## Overview
This repository provides a comprehensive guide to using the **`macchanger`** tool for managing and spoofing MAC addresses on Linux systems. 

`macchanger` is a powerful utility that allows users to:
- View their current MAC address.
- Temporarily or permanently change the MAC address.
- Randomize the MAC address for anonymity.

---

## Prerequisites
Ensure `macchanger` is installed on your system. Most Linux distributions include it by default. If not, install it using:

### Installation
#### Debian/Ubuntu/Kali:

    sudo apt update
    sudo apt install macchanger
Fedora:

    sudo dnf install macchanger

Arch:

    sudo pacman -S macchanger

##Basic Usage

**Help**

    sudo macchanger --help
![image](https://github.com/user-attachments/assets/d8930468-567d-4ce1-acb5-12c09e88ce8a)
    
**1. Check Current MAC Address**

    sudo macchanger -s <interface>

Example:

    sudo macchanger -s eth0

**2. Assign a Random MAC Address**

    sudo macchanger -r <interface>

**3. Change to a Specific MAC Address**

    sudo macchanger -m <new_mac_address> <interface>

Example:

    sudo macchanger -m 00:11:22:33:44:55 eth0

**4. Restore Original MAC Address**

    sudo macchanger -p <interface>
