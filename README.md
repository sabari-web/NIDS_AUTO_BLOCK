# NIDS_AUTO_BLOCK
Python based NIDS with automatic IP blocking and GUI
# Python-Based Network Intrusion Detection System (NIDS)

## 🔐 Project Overview
This project is a Python-based Network Intrusion Detection System (NIDS) that detects
malicious network activities such as port scanning and automatically blocks attackers
using iptables. A real-time GUI dashboard displays alerts and blocked IPs.

This project demonstrates hands-on experience in:
- Network security
- Packet analysis
- Intrusion detection
- Firewall automation
- SOC/Blue Team fundamentals

---

## 🚀 Features
- Live packet sniffing using Scapy
- Port scan detection (Nmap SYN & TCP scans)
- Automatic attacker IP blocking using iptables
- Real-time GUI dashboard (Tkinter)
- Alert logging for incident response analysis

---

## 🛠️ Technologies Used
- Python 3
- Scapy
- Tkinter
- iptables
- Kali Linux / Ubuntu
- Nmap (for testing)

---

## ⚙️ How It Works
1. The IDS monitors incoming TCP packets.
2. If a single IP scans multiple ports within a short time window:
   - It is classified as malicious behavior.
3. The attacker IP is automatically blocked using iptables.
4. The GUI dashboard displays alerts in real-time.

---

## 🧪 Testing
The IDS was tested using:
```bash
nmap -sS -p 1-1000 <target-ip>
nmap -sT -p 1-200 <target-ip>
