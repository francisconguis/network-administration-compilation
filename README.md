# 🌐 Network Administration Lab Compilation

![Platform](https://img.shields.io/badge/Platform-Cisco%20Packet%20Tracer-005073.svg)
![Domain](https://img.shields.io/badge/Domain-Computer%20Networking-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Coursework-Completed-success.svg)

A repository of network simulation projects, topology designs, and protocol configuration labs built using **Cisco Packet Tracer**. This collection demonstrates hands-on implementation of switching, routing, network security, and enterprise infrastructure services.

---

## 📌 Lab Directory & Topology Overview

| Lab File | Topic Title | Content |
| :--- | :--- | :--- |
| `Activity 1_Conguis.pkt` | Basic LAN Topologies & Multi-Subnet Switching | Configures two independent star-topology local networks (10.10.10.0 and 20.20.20.0) on Cisco Catalyst 2960 switches to test static IPv4 host addressing, intra-switch packet delivery, and broadcast domain isolation without a router. |
| `Activity 2_Conguis.pkt` | Multi-Switch Star Topology & Switch Uplink Interconnection | Demonstrates inter-switch expansion using two Cisco Catalyst 2950-24 switches (S1 and S2) interconnected via an Ethernet crossover link, connecting end devices (PC0 through PC3) within a unified flat subnet (10.10.10.0) to verify Layer 2 frame forwarding across uplinks. |
| `Activity 3_Conguis.pkt` | Basic Switch Configuration, SVI Management & Line Security | Focuses on configuring Cisco Catalyst 2960 switches with Switch Virtual Interface (SVI VLAN 1) management IP addresses (192.168.1.253 and .254), establishing switch-to-switch trunk/crossover links, and securing console/VTY administrative logins using password authentication. |
| `Activity 4_Conguis.pkt` | VLAN Segmentation & Access Ports | IEEE 802.1Q encapsulation, VLAN tagging, Access mode configs |
| `Activity 5_Conguis.pkt` | Trunking & Inter-VLAN Routing | Router-on-a-Stick (ROAS), Sub-interfaces, Trunk mode links |
| `Activity 6_Conguis.pkt` | Inter-VLAN Routing (ROAS) with Wireless LAN Extension | Implements Router-on-a-Stick using a Cisco 2811 router and 2960 switch to route traffic between multi-floor VLANs (10, 20, 30) across an 802.1Q trunk, integrating an access point for wireless end-device connectivity. |
| `Activity 7_Conguis.pkt` | Network Services (DHCP & DNS) | Dedicated & router-hosted DHCP pools, DNS resolution |
| `Activity 8_Conguis.pkt` | Traffic Filtering & Security (ACLs) | Standard and Extended Access Control Lists (ACLs) |
| `Activity 10_Conguis.pkt` | Multi-Subnet Corporate Infrastructure | Multi-switch uplink architecture, perimeter defense |
| `Activity1(Finals)_Conguis.pkt` | Enterprise Capstone Network | Redundant links, multi-VLAN enterprise campus design |

---

## 🛠️ Key Technical Competencies Demonstrated

* **Layer 2 Switching:** VLAN provisioning, 802.1Q trunking negotiation, Spanning Tree Protocol (STP) verification, and switchport port-security policies.
* **Layer 3 Routing:** Inter-VLAN routing using sub-interfaces (Router-on-a-Stick), static route fallbacks, and dynamic routing convergence.
* **IP Addressing & Planning:** Subnetting with VLSM, CIDR prefix optimization, gateway assignment, and IPv4 address conservation.
* **Network Services & Hardening:** DHCP server configuration, DNS name binding, standard/extended Access Control Lists (ACLs) for ingress/egress filtering, and SSH/console administrative credentials.

---

## 🚀 How to Open and Inspect Labs

1. **Prerequisites:** Install [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer) (version 8.0 or newer recommended).
2. **Clone the repository:**
   ```bash
   git clone [https://github.com/francisconguis/network-administration-compilation.git](https://github.com/francisconguis/network-administration-compilation.git)
