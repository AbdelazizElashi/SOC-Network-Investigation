# SOC Network Investigation 🔍

 Project Overview

This project simulates a Security Operations Center (SOC) investigation by analyzing devices within a local network using professional tools such as Nmap and Wireshark.

The objective is to identify active hosts, analyze network behavior, and detect potential security risks.

---

 Tools Used

* Nmap (Network Scanning & Enumeration)
* Wireshark (Packet Analysis)
* Kali Linux (Penetration Testing Environment)

---

 Network Discovery

Initial scan of the network to identify active devices:

![Network Scan](images/01-network-scan.png)

---

 Device Analysis

 Device 1 Analysis

* All TCP ports closed
* No exposed services

![Device 1](images/02-device1-scan.png)

---

 Device 2 Analysis (UDP)

* Port 5353 (mDNS) detected
* Indicates local service discovery

![Device 2](images/03-device2-udp.png)

---

 Router / Gateway Analysis

* HTTP & HTTPS services detected
* Potential web interface exposed

![Router](images/04-router-scan.png)

---

 Findings

* Multiple devices identified within the network
* Limited exposed services (good security posture)
* Presence of mDNS service indicates internal communication
* Router exposes web-based services (potential attack surface)

---

 Conclusion

This investigation demonstrates how basic SOC techniques can be used to:

* Map a network
* Identify active devices
* Analyze services and protocols
* Detect potential security risks

---

 Full Report

See full technical report:

📥 [Download PDF](network_device_profiling_report.pdf)
