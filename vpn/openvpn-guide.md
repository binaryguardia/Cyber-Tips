# VPNBook OpenVPN Setup Guide for Kali Linux

This guide will show you how to set up and use OpenVPN on Kali Linux using free VPN credentials from VPNBook.

## Step 1: Install OpenVPN

If OpenVPN is not already installed on your system, you can install it with the following command:

    sudo apt update
    sudo apt install -y openvpn

## Step 2: Download Free VPN Configuration from VPNBook

  Go to VPNBook Free OpenVPN and download the latest OpenVPN Certificate Bundle. This bundle will be a .zip file (e.g., vpnbook.zip) with configuration files for various servers.

  Extract the .zip file to access the .ovpn configuration files. You can do this with the following command:

    unzip vpnbook.zip -d vpnbook
  You should now have a folder called vpnbook with multiple .ovpn files, each corresponding to a VPN server (e.g., vpnbook-euro1-tcp443.ovpn).
  
## Step 3: Get VPNBook Username and Password

VPNBook[https://www.vpnbook.com/freevpn] provides free usernames and passwords on their website. Go to VPNBook Free OpenVPN and note down the current username and password.
## Step 3: Activate vpn 
    openvpn vpnfile.ovpn
