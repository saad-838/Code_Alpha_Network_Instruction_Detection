

# Python Network Intrusion Detection System (NIDS)

A lightweight, single-file NIDS for Windows that detects suspicious network activity in real-time using Python and Scapy.

## Features

- 🚨 **Threat Detection**: Port scans, SYN floods, brute force attempts
- 🔍 **Payload Analysis**: SQLi, XSS, directory traversal patterns
- 📊 **Web Dashboard**: Real-time alerts at `http://localhost:8080`
- ✉️ **Email Alerts**: Optional SMTP notifications
- 📝 **Logging**: All alerts saved to `ids.log`

## Requirements

- Python 3.7+
- Windows 10/11 (Admin privileges)
- [Npcap](https://nmap.org/npcap/) (WinPcap compatible mode)

## Installation

1. Install dependencies:
   ```bash
   pip install scapy pywin32
Download and install Npcap

Usage
Run as Administrator:

bash
Copy
python ids.py
Access dashboard:
http://localhost:8080

Configuration
Edit the CONFIG section in ids.py to:

Set your home network range

Adjust detection thresholds

Enable email alerts

Customize monitored ports

Detection Capabilities
Port Scans (>15 unique ports)

SYN Floods (>100 SYN packets/sec)

Auth Attempts (>10/min on sensitive ports)

Suspicious Payloads (SQLi, XSS, etc.)
