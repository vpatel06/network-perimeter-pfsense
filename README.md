# 🛡️ Network Perimeter Security Lab using pfSense + Suricata

This project builds a **virtual perimeter security network lab** using **pfSense** as a firewall/router and **Suricata** as an Intrusion Detection System (IDS) within **VirtualBox** — all 100% free and offline. It simulates a real-world network perimeter and showcases hands-on network security skills, ideal for cybersecurity students and beginners.

---

## 📌 Project Goals

- 🔐 Simulate a secure network perimeter in a virtual environment
- 📦 Learn pfSense firewall configuration (interfaces, NAT, DHCP)
- 🕵️ Deploy and configure Suricata IDS with live rules
- 💻 Inspect and alert on suspicious network activity
- 🧠 Practice hands-on network defense and monitoring

---

## 🧰 Tech Stack

| Component      | Purpose                               |
|----------------|----------------------------------------|
| VirtualBox     | Virtualization platform                |
| pfSense        | Open-source firewall/router            |
| Suricata       | Network Intrusion Detection System     |
| Host-only LAN  | Simulated internal network             |
| ET Open Rules  | Community-maintained IDS ruleset       |

---

## 🖥️ Network Topology

    [Internet]
        |
    [NAT (WAN)]
        |
     pfSense
    (Firewall)
        |
  [Host-only LAN]
        |
 [Host OS or VMs]


---

## 🛠️ Setup Instructions

For detailed step-by-step instructions, see [`docs/setup.md`](docs/setup.md)

1. ✅ Install VirtualBox
2. 🧱 Create pfSense VM with 2 adapters: NAT (WAN) + Host-only (LAN)
3. 🌐 Configure LAN IP (e.g., `192.168.56.2`) and DHCP range
4. 🔧 Access pfSense Web GUI from host browser
5. 📦 Install Suricata package
6. 📄 Enable ET Open rules
7. 📊 Monitor network with Suricata alerts

---

## 🔍 Suricata Rules

- ET Open ruleset enabled and updated inside pfSense
- LAN interface monitored with Suricata in IDS mode
- Alerts triggered by suspicious packets (e.g., scans, signatures)

Details available in [`docs/suricata-rules.md`](docs/suricata-rules.md)

---

## 🧪 Testing & Results

You can simulate and detect:

- Port scans using `nmap`
- EICAR test file download
- Misconfigured devices broadcasting strange traffic

Captured alerts are visible in:


---

## 📸 Screenshots

| pfSense Dashboard            | Suricata Rules Setup         |
|-----------------------------|------------------------------|
| ![](images/dashboard.png)   | ![](images/suricata-config.png) |

---

## 📚 Learning Outcomes

- Understand firewall interfaces, NAT, and IP ranges
- Deploy and tune Suricata in a real-world layout
- Apply ET rules and monitor traffic
- Build foundational skills for Network+ / CCNA / SOC analyst

---

## 🏁 Next Steps

- Add Windows/Linux VM on LAN side to simulate client
- Use port scanning, malware samples, or traffic generators
- Add Snort, pfBlockerNG, or remote logging to SIEM

---

## 📝 License

This project is open-source under the [MIT License](LICENSE).

---

## 🙋‍♂️ Author

**V Patel**  
Cybersecurity Student | Network Security Enthusiast  
[GitHub Profile](https://github.com/vpatel06)



