# ProxyChains Setup and Usage Guide

ProxyChains is a tool that forces applications to route their network traffic through proxy servers. This guide explains how to set up and configure ProxyChains on Linux.

## Step 1: Install ProxyChains

If ProxyChains is not already installed, you can install it with:

    sudo apt update
    sudo apt install proxychains4 -y
## Step 2: Edit ProxyChains Configuration

 **Open the Configuration File:**
    
    sudo nano /etc/proxychains4.conf
 **Remove the hashes**
 #dynamic_chain
 #Proxy DNS requests - no leak for DNS data
![image](https://github.com/user-attachments/assets/7e012611-7bdf-4507-a49f-82f984437c24)

save it by by ctrl + s and exit by ctrl + x
## Step 3: Usage Examples

Run applications through ProxyChains using the following syntax:
   
proxychains4 [application] [arguments]
```
   proxychains4 firefox
