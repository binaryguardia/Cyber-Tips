# BeeLogger

**BeeLogger** is an open-source keylogger generator built in Python, designed for ethical hacking and cybersecurity education. It allows users to create Windows-compatible keylogger payloads that can monitor keystrokes and send logs via email.

---
# This is not the official Beelogger repo.
**If you face any issue kindly visit it's official website  [BeeLogger GitHub Repository](https://github.com/4w4k3/beelogger).**
---
## ⚠️ **Disclaimer**

This tool is for educational purposes only. Any unauthorized use of this software to compromise systems, invade privacy, or other unethical purposes is illegal. Use BeeLogger only on systems you own or have explicit permission to test. The creator and contributors of BeeLogger are not responsible for any misuse of this tool.

---

## Features
- Generate Windows-compatible keylogger payloads.
- Send keylogging data via Gmail.
- Easy-to-use CLI interface.
- Works on Linux and Windows with the help of Wine.

---

## Requirements
- **Operating System**: Linux (Parrot, Kali) or Windows.
- **Python**: Python 2.7.
- **Dependencies**:
  - `wine`
  - `PyCrypto`
  - `pynput`

---

## Installation and Setup

### 1. Clone the Repository
    
    git clone https://github.com/4w4k3/BeeLogger.git
    cd BeeLogger
### 2. Install Required Dependencies

## HOW TO INSTALL:

Video: https://www.youtube.com/watch?v=ifOGkOTS5zk

    sudo chmod +x install.sh
    sudo ./install.sh
    python2.7 bee.py

### 3. Configure Gmail
   Use a Gmail account to send logs.
   Enable "Less Secure App Access" in your Gmail account settings.
        Go to Google Account Settings.
        Enable "Allow less secure apps."
        Use a dedicated Gmail account for security reasons.

## How to Use
### 1. Generate a Keylogger Payload

Run the main script:

    python2.7 bee.py
![image](https://github.com/user-attachments/assets/619a11f0-c1bd-4e0b-96fc-2402580a9a62)

Follow the prompts to:
    Enter your Gmail address and password (used to send logs).
    Customize the payload (file name, settings).

### 2. Test the Payload
  Transfer the generated .exe file to the target Windows system.
    Logs will be sent to the configured Gmail.

## Troubleshooting
Common Issues

  **Wine Errors:**
        Ensure Wine is properly installed:

        sudo apt install wine

  Reconfigure Wine if issues persist.

  **Logs Not Sent:**
        Check Gmail account credentials.
        Ensure "Less Secure App Access" is enabled.

   **Missing Files:**
        Verify all dependencies are installed.
        Clone a stable version of the repository.


## 🌐 Additional Resources
   
  [BeeLogger GitHub Repository](https://github.com/4w4k3/beelogger)
  
 [How to Install Wine](https://forums.kali.org/archived/showthread.php?25175-install-wine-on-kali-64bit-with-no-problems)

