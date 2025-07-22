# 🛡️ Virtual Network Perimeter Lab with pfSense + Suricata + Kali + Ubuntu

## 📌 Overview

This project simulates a virtual **network perimeter defense system** using open-source tools within **VirtualBox**. It features a realistic lab setup using:

- `pfSense` firewall + router  
- `Suricata` IDS to detect and log threats  
- `Ubuntu` (internal host)  
- `Kali Linux` (simulated attacker)

The goal was to understand how network security works in practice, including how firewalls and IDS tools detect suspicious activity such as port scanning, malware downloads, and reconnaissance. A Python script was written to parse alerts from Suricata’s `eve.json` log for threat intelligence.

This project also helped reinforce concepts from the **CCNA**, especially around network segmentation, interfaces, and security zones.

---

## 🧠 Skills Practiced

- pfSense installation and LAN/WAN interface setup  
- Suricata configuration and rule tuning  
- Network alert logging and testing  
- Simulating attacks from Kali Linux (e.g., `nmap`)  
- Parsing Suricata alerts using Python  
- Working with VirtualBox virtual networks (NAT, Host-only)

---

## 🖼️ Lab Architecture
<pre> ┌────────────┐ │ Internet │ └────┬───────┘ │ [NAT] │ ┌──────▼───────┐ │ pfSense │ │ Firewall + │ │ Suricata IDS│ └────┬────┬────┘ │ │ em0 (WAN) em1 (LAN) 10.0.2.15/24 192.168.56.1/24 │ ┌────────┴────────┐ │ │ ┌────────────┐ ┌────────────┐ │ Ubuntu │ │ Kali │ │ 192.168. │ │ 192.168. │ │ 56.2 │ │ 56.3 │ └────────────┘ └────────────┘ </pre>
