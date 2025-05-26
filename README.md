# cybersecurityinternshipday1
working of nmap and wireshark
# 🔍 Local Network Port Scanning with Nmap & Wireshark

This project demonstrates how to scan a local network for open ports using [Nmap](https://nmap.org/) and optionally analyze network traffic using [Wireshark](https://www.wireshark.org/). The goal is to discover network exposure, identify services, and understand potential security risks.

---

## 🛠 Tools Used

- **Nmap** – Network exploration and security auditing tool
- **Wireshark** *(optional)* – Network protocol analyzer

---

## 📡 Steps Performed

1. **Identified local IP range** using `ipconfig` or `ifconfig`
2. **Ran a TCP SYN scan** across the subnet:
   ```bash
   nmap -sS 192.168.1.0/24
Captured traffic in Wireshark:

Filter used:
wireshark

tcp.port == 80 || tcp.flags.syn == 1
Analyzed scan results to identify:

IP addresses of devices on the network

Open ports and common services (e.g., SSH, HTTP, SMB)

Potential security vulnerabilities

Saved results in:

Text format: nmap.html


