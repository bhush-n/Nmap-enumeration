# Exploring and Mapping a Local Network Using Nmap on Kali Linux

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
