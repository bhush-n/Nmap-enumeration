# Exploring and Mapping a Local Network Using Nmap on Kali Linux

## Table of contents

[Overview](https://github.com/bhush-n/Nmap-enumeration#overview)

[Requirements](https://github.com/bhush-n/Nmap-enumeration#Requirements)

[Setup and Tools](https://github.com/bhush-n/Nmap-enumeration#setup_and_tools)

[Steps](https://github.com/bhush-n/Nmap-enumeration#steps)

[Resources](https://github.com/bhush-n/Nmap-enumeration#additional_resources)

[Support](https://github.com/bhush-n/Nmap-enumeration#support)

## Overview
In this guide, you will learn to use Nmap, a robust network scanning utility, to detect devices and services operating on a local network. Network scanning and mapping are vital techniques for ethical hackers, aiding in pinpointing potential targets and vulnerabilities within a network. By the conclusion of this guide, you will be proficient in executing basic network scans, identifying open ports, and extracting information about network devices using Kali Linux.

## Requirements
- Fundamental knowledge of networking (IP addresses, ports, etc.).
- Familiarity with the command line interface (CLI).
- Kali Linux installed (either natively, in a virtual machine, or as a live boot).

## Setup and Tools

### Required Tools
- **Kali Linux**: A Debian-based Linux distribution designed for digital forensics and penetration testing.
- **Nmap**: A network exploration tool and security/port scanner (pre-installed on Kali Linux).
- A local network with various connected devices (computers, printers, IoT devices, etc.).

### Verifying Installation
Nmap comes pre-installed on Kali Linux. You can confirm its installation or update it using:
```sh
sudo apt-get update && sudo apt-get install nmap
```
## Steps

### Step 1: Performing a Basic Network Scan
- Launch a terminal on your Kali Linux system.
- Conduct a basic scan on your local network. Replace `192.168.1.0/24` with your network's IP range.
    ```sh
    nmap 192.168.1.0/24
    ```
- Expected Result: A list of network devices, their IP addresses, and open ports.

### Step 2: Scanning Specific Ports
- To scan a specific port (e.g., HTTP port 80), use the `-p` option:
    ```sh
    nmap -p 80 192.168.1.0/24
    ```
- Expected Result: A list of devices with port 80 open.

### Step 3: Detecting Service Versions
- Utilize the `-sV` option to determine the version of services on open ports:
    ```sh
    nmap -sV 192.168.1.0/24
    ```
- Expected Result: A detailed list of open ports and running services with version information.

### Step 4: Identifying Operating Systems
- Use the `-O` option to detect the operating systems of network devices:
    ```sh
    sudo nmap -O 192.168.1.0/24
    ```
- Expected Result: Details about the operating systems of devices on the network.

### Step 5: Executing an Aggressive Scan
- Conduct an aggressive scan using the `-A` option, which encompasses OS detection, version detection, script scanning, and traceroute:
    ```sh
    sudo nmap -A 192.168.1.0/24
    ```
- Expected Result: Comprehensive data about network devices, including open ports, services, versions, operating systems, and traceroute information.

## Additional Resources
- [Nmap Official Documentation](https://nmap.org/docs.html)
- [Nmap Cheat Sheet](https://nmap.org/book/man-briefoptions.html)
- [Online Nmap Course on Udemy](https://www.udemy.com/course/nmap/)

This guide provides a foundational understanding of using Nmap for network scanning and mapping, crucial skills for any ethical hacker.

## Support

For support, email bhushanch45@gmail.com.
