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
```bash
cd ~/Downloads
sudo dpkg -i Nessus-#.##.#-debian6_amd64.deb
