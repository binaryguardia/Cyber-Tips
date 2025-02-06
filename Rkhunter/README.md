# rkhunter: Rootkit Hunter for Linux

**rkhunter** (Rootkit Hunter) is an open-source security tool designed to detect rootkits, backdoors, and other potential vulnerabilities on Linux systems. It is widely used by system administrators and cybersecurity professionals to maintain the integrity of their systems.

---

## Why Use rkhunter?

Rootkits are dangerous malware that can:
- Operate stealthily to avoid detection.
- Modify system files and binaries.
- Grant attackers persistent unauthorized access.

rkhunter is critical in cybersecurity for the following reasons:
- **System Integrity Checks**: Verifies system binaries, configuration files, and permissions.
- **Rootkit Detection**: Scans for known and hidden rootkits.
- **Backdoor Detection**: Identifies suspicious files and unauthorized access points.
- **Regular Security Audits**: Helps ensure compliance with security best practices.

---

## Features

- Scans for over 200 known rootkits.
- Detects:
  - Hidden files and processes.
  - Suspicious entries in configuration files.
  - Weak or unsafe security settings.
- Verifies SHA-256 hashes of critical system files.
- Provides customizable scans and logs.

---

## Installation

Follow these steps to install rkhunter on your Linux system.

### Step 1: Update the Package List
Ensure your system's package list is up-to-date:

    sudo apt update
### Step 2: Install rkhunter

Install rkhunter using the following command:

    sudo apt install rkhunter

### Step 3: Update the rkhunter Database

After installation, update the database for the latest definitions:

    sudo rkhunter --update

## Usage

rkhunter is easy to use and provides a variety of options for scanning and reporting.
## Step 1: Run a Basic Scan

To perform a full system check:

    sudo rkhunter --check
![image](https://github.com/user-attachments/assets/d3fceec1-d9e3-4775-a203-3dadb5d5d59d)

## Step 2: Review Scan Results

The results are logged in:

    /var/log/rkhunter.log

You can review the log using:

    cat /var/log/rkhunter.log

### Step 3: Respond to Warnings

rkhunter may generate warnings for potential threats. Investigate these carefully and take necessary actions.
Advanced Options
**Update rkhunter Database**

Regular updates ensure the latest malware definitions:

    sudo rkhunter --update

Configure Whitelisted Files

To prevent false positives, whitelist trusted files in the configuration file:

    sudo nano /etc/rkhunter.conf

Detailed Logging

Enable verbose mode for more information:

    sudo rkhunter --check --rwo

Perform All Tests

Run all available tests with:

    sudo rkhunter --checkall

