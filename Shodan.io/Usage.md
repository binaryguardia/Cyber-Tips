# Shodan.io: The Search Engine for the Internet of Things (IoT)

**Warning: Try to use vpn or proxies before using it and  don't leave your fingerprints anywhere.**

**Shodan.io** is a search engine specifically designed for cybersecurity professionals, allowing users to discover devices, services, and vulnerabilities exposed to the internet. Unlike traditional search engines that index websites, Shodan indexes information about servers, webcams, routers, IoT devices, industrial control systems, and more.

---

## Why Use Shodan?

Shodan is widely used in the field of cybersecurity for the following purposes:

- **Asset Discovery**: Identify devices connected to the internet in specific regions or organizations.
- **Vulnerability Assessment**: Discover devices with outdated software or known vulnerabilities.
- **Penetration Testing**: Analyze the security posture of devices before attempting exploits.
- **Incident Response**: Track exposed systems after data breaches.
- **Threat Intelligence**: Monitor specific devices or organizations for changes or potential attacks.

---

## Key Features of Shodan

1. **Device Discovery**:
   - Search for IoT devices such as webcams, industrial systems, or printers connected to the internet.

2. **Vulnerability Identification**:
   - Identify exposed devices using filters like operating system, software version, or vulnerability tags.

3. **Network Monitoring**:
   - Monitor your network's exposure by tagging IP ranges and reviewing their configurations.

4. **Shodan Alerts**:
   - Set alerts to track devices and receive notifications about configuration changes or new vulnerabilities.

5. **API Integration**:
   - Use Shodan's API to integrate data into applications for automated analysis.

6. **Advanced Filters**:
   - Utilize filters for precise searches, such as geographic location, device type, or specific ports.

---

## Getting Started

### Step 1: Sign Up for Shodan
1. Visit the [Shodan.io website](https://www.shodan.io/).
  ![image](https://github.com/user-attachments/assets/2f5e8bb3-496d-4fc9-a8cb-d12446624218)
 
2. Create an account by clicking **Sign Up**.
3. Verify your email address and log in.

### Step 2: Choose a Subscription
Shodan offers several tiers:
- **Free**: Limited access with basic features.
- **Membership**: Provides advanced filters and enhanced search capabilities.
- **Enterprise**: Designed for large-scale use with API and monitoring tools.

---

## Usage Guide

### Basic Search
To search for connected devices, use the search bar on the Shodan homepage. For example:

    webcam

This query will return a list of webcams exposed to the internet.

## Advanced Search with Filters

Shodan supports various filters for precise searches. Some common filters include:

  country: Filter results by country.

    apache country:"US"

port: Search for devices with specific open ports.

    port:22

os: Filter results by operating system.

    os:"Windows 10"

vuln: Search for devices with specific vulnerabilities.

    vuln:"CVE-2021-44228"

product: Search for specific software or hardware products.

    product:"OpenSSH"

## Shodan CLI

Install the Shodan command-line interface (CLI) for automated queries:

  Install Shodan CLI using pip:

    pip install shodan

Authenticate with your API key:

    shodan init YOUR_API_KEY

Perform searches directly from the command line:

    shodan search webcam

## Shodan Maps

Visualize device locations on a map:

  Go to Shodan Maps.
  Use filters to explore device distributions globally.

## Shodan Alerts

Create alerts to monitor specific IPs or networks:
    Navigate to Alerts on the dashboard.
    Create a new alert by entering the IP range or network to monitor.
    Customize notifications and enable email alerts.

## Practical Use Cases in Cybersecurity

  Assess Network Exposure:
        Search for devices in your organization to identify open ports or misconfigured devices.

    net:"192.168.1.0/24"

### Monitor Critical Systems:

  Track public-facing industrial control systems (ICS) or SCADA devices.

    product:"SCADA"

### Identify Vulnerable Systems:

  Search for systems exposed to the latest vulnerabilities.

        vuln:"CVE-2023-12345"

  Threat Hunting:
        Track malicious actors or compromised devices using specific tags.

## Best Practices

   Use Filters Wisely: Avoid generic searches to reduce noise and focus on relevant results.
   Monitor Regularly: Set up alerts for continuous monitoring of your assets.
   Practice Ethical Usage: Ensure compliance with local laws and regulations when using Shodan.
