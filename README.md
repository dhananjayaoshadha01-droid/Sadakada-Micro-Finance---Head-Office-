# 📂 Sadakada Micro Finance - Head Office Network Infrastructure

### 📝 Project Overview
This project involves the design and implementation of a secure, scalable, and high-performance network infrastructure for the **Sadakada Micro Finance Head Office** using **Cisco Packet Tracer**. The primary objective is to demonstrate enterprise-level **Network Segmentation** and **Inter-VLAN Routing** to ensure secure data flow between financial departments.

### 📸 Network Diagram
![Network Diagram](main%20branch.png)

### 🚀 Key Features
* **Network Segmentation:** Divided the organization into 5 functional VLANs to reduce broadcast domains and enhance security.
* **Inter-VLAN Routing:** Implemented using the **Router-on-a-Stick** topology with 802.1Q encapsulation on a Cisco 2911 Router.
* **Wireless Connectivity:** Integrated Access Points for seamless WiFi connectivity for staff laptops.
* **VoIP Integration:** Configured IP Phones with dedicated extensions for internal communication.
* **Hierarchical Design:** Uses a central Core Switch to aggregate traffic from multiple Access Switches.

### 🏗️ Topology Details (VLAN Table)
| Department | VLAN ID | IP Subnet |
| :--- | :---: | :--- |
| IT / Admin | 10 | 192.168.10.0/24 |
| Wireless (Staff) | 20 | 192.168.20.0/24 |
| Voice (VoIP) | 30 | 192.168.30.0/24 |
| Servers / Database | 40 | 10.0.0.0/24 |
| Management (Native) | 99 | 192.168.99.0/24 |

### 🛠️ Configuration Highlights
* **Encapsulation:** `dot1Q` used for sub-interfaces on the gateway.
* **Trunking:** Configured 802.1Q trunks between all switches and the router.
* **DHCP:** Configured DHCP pools for automated IP assignment across all departments.

### 📂 How to use
1. Download the `main branch.pkt` file from this repository.
2. Open it in **Cisco Packet Tracer (v8.0 or higher)**.
3. Test connectivity by pinging between different VLANs (e.g., IT PC to Server).

---
**Designed by:** Oshadha Dhananjaya  
**Role:** Cybersecurity Engineer / IT Student at Rajarata University of Sri Lanka
