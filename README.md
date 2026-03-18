# Corporate Network Infrastructure with Inter-VLAN Routing

This project demonstrates a secure corporate network architecture designed in **Cisco Packet Tracer**. It features multiple departments segmented into VLANs, providing improved security, performance, and manageability.

## 🚀 Key Features
* **Network Segmentation:** Divided the organization into 5 functional VLANs (IT, Wireless, Voice, Server, and Management).
* **Inter-VLAN Routing:** Implemented using the **Router-on-a-Stick** topology with sub-interfaces.
* **Wireless Connectivity:** Integrated Access Points for mobile users.
* **Management Security:** Dedicated Management VLAN (VLAN 99) for switch configuration access.
* **Hierarchical Design:** Uses a Core Switch to aggregate traffic from multiple Access Switches.

## 🏗️ Topology Details
| Department | VLAN ID | IP Subnet |
| :--- | :---: | :--- |
| IT / PCs | 10 | 192.168.10.0/24 |
| Wireless | 20 | 192.168.20.0/24 |
| Voice (VoIP) | 30 | 192.168.30.0/24 |
| Servers | 40 | 10.0.0.0/24 |
| Management | 99 | 192.168.99.0/24 |

## 🛠️ Configuration Highlights
* **Encapsulation:** 802.1Q dot1Q used for sub-interfaces on the 2911 Router.
* **Trunking:** Configured 802.1Q trunks between all switches and the router.
* **DHCP:** Configured DHCP pools for automated IP assignment.

## 📸 Network Diagram
*(Insert your Packet Tracer screenshot here)*

## 📂 How to use
1. Download the `.pkt` file from this repository.
2. Open it in **Cisco Packet Tracer (v8.0 or higher)**.
3. Test connectivity by pinging between different VLANs.
