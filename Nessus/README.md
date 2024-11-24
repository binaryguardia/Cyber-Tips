# Nessus Installation and Usage Guide for Cybersecurity

Nessus is a powerful vulnerability scanner developed by Tenable, used extensively in cybersecurity for assessing vulnerabilities in systems, networks, and applications. This guide provides a step-by-step walkthrough to help you install, set up, and use Nessus for your penetration testing or vulnerability management needs.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
4. [Initial Setup](#initial-setup)
5. [Using Nessus for Cybersecurity](#using-nessus-for-cybersecurity)
6. [Common Nessus Scans](#common-nessus-scans)
7. [FAQs](#faqs)
8. [Resources](#resources)

---

## Introduction
Nessus Essentials is a free version of the Nessus vulnerability scanner, designed for small-scale environments. It allows users to scan up to 16 IP addresses, making it ideal for personal or educational use. This guide covers:
- Installing Nessus on a Debian-based OS.
- Setting up and activating Nessus.
- Conducting vulnerability scans.

---

## Prerequisites
Before starting, ensure you have the following:
- A Debian-based operating system (e.g., Ubuntu).
- Administrative (root) access to the terminal.
- A valid email address to register for Nessus Essentials.

---

## Installation

### Step 1: Register for Nessus Essentials
1. Visit [Tenable's Nessus Essentials Registration Page](https://www.tenable.com/products/nessus/nessus-essentials).  
2. Create an account and provide your email to receive an **activation code**.

### Step 2: Download the Nessus Package
1. Go to the [Nessus Downloads Page](https://www.tenable.com/downloads/nessus).
2. Download the `Nessus-#.##.#-debian6_amd64.deb` package suitable for Debian-based systems.
3. Save the file to your `/Downloads/` folder.

### Step 3: Install Nessus
Navigate to the folder containing the downloaded file and install it using the following command:

    cd ~/Downloads
    sudo dpkg -i Nessus-#.##.#-debian6_amd64.deb
### Step 4: Start the Nessus Service

Start the Nessus service with the command:

    sudo /bin/systemctl start nessusd.service

### Step 5: Access the Web Interface

  Open your browser (e.g., Firefox) and navigate to:

  **https://localhost:8834/**

  If prompted with a security risk alert, click: Advanced... -> Accept the Risk and Continue.
 
## Initial Setup
### Step 6: Configure Nessus

   Select Nessus Essentials during the setup.
    Enter the activation code you received via email.

### Step 7: Create a User Account

  Set up a username and a strong password for Nessus access.
    Proceed to the next step.

### Step 8: Install Plugins

Nessus will now download and install the required plugins. This step may take some time depending on your internet speed and hardware capabilities.
### Step 9: Log In

   Once the installation is complete, log in using the credentials you created earlier.
    You are now ready to use Nessus!

## Using Nessus for Cybersecurity
### Step 1: Launch a New Scan
![image](https://github.com/user-attachments/assets/e5dc9abd-109d-4aed-84e5-dce7b4369f7c)

   Log into the Nessus web interface.
    Click on Scans in the left-hand menu.
    Choose a scan template based on your needs (e.g., Basic Network Scan, Web Application Scan, or Malware Scan).

### Step 2: Configure the Scan

  Provide a name for the scan.
    Enter the target(s) (e.g., IP address or domain).
    Adjust additional settings, such as scan schedule or credentials.

### Step 3: Run the Scan

  Click Save to save your scan configuration.
    Start the scan by clicking Launch.

### Step 4: Review Scan Results

   Once the scan is complete, view the results to identify vulnerabilities.
    Export the report in your preferred format (e.g., PDF, CSV).

## Common Nessus Scans
1. Basic Network Scan

    Identifies vulnerabilities in network devices and servers.
    Ideal for general network assessments.

2. Web Application Scans

    Checks for vulnerabilities in web applications (e.g., SQL injection, XSS).
    Ensures web apps are secure against common attacks.

3. Compliance Checks

    Ensures systems meet security standards like PCI-DSS, HIPAA, or ISO 27001.
    Useful for regulatory compliance.

4. Credentialed Scans

    Uses system credentials for deeper vulnerability analysis.
    Provides detailed insights into system misconfigurations.
