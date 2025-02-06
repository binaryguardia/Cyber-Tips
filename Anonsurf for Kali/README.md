# Anonsurf Setup and Usage Guide for Kali Linux

Anonsurf is a tool for anonymizing network activity on Kali Linux using TOR and iptables. This guide provides setup instructions and common commands.

## Installation

1. **Create a Directory and Clone Repository:**

   ```bash
   mkdir Anonsurf && cd Anonsurf
   git clone https://github.com/Und3rf10w/kali-anonsurf.git
   cd kali-anonsurf
   
2. **Run the installer script**
   
   
   ```bash
   sudo ./installer.sh
## Usage

Here are some commands for using Anonsurf after installation:

1. **Start Anonsurf:**
   ```
   sudo anonsurf
 ![image](https://github.com/user-attachments/assets/5b7d2995-a36f-48c5-823c-97fd4ca35308)
![image](https://github.com/user-attachments/assets/6250cd6a-a65e-42d7-a0e4-e16faba4c5fc)

2. **Stop Anonsurf:**
   ```
   anonsurf stop
![image](https://github.com/user-attachments/assets/ed43f866-a74a-4486-8283-3d059d7c7e71)

3. ***Restart Anonsurf:**
   ```
   anonsurf restart
![image](https://github.com/user-attachments/assets/21e29e52-08a6-48dc-80b0-b5f9ea569dca)

4. ***Change IP Address:***
   ```
   anonsurf change
![image](https://github.com/user-attachments/assets/e4f867b1-9af8-48b1-8cf6-e3de6abe5d02)

5. ***Check Current IP Address:***
   ```
   anonsurf myip

6. ***Check Anonsurf Status:***
   ```
   anonsurf status
![image](https://github.com/user-attachments/assets/6be82120-d64c-48bb-a0d8-89da04c19be7)


Reference: 
https://github.com/Und3rf10w/kali-anonsurf
