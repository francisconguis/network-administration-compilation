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
| `Activity 4_Conguis.pkt` | VLAN Segmentation & Router-on-a-Stick (ROAS) Routing | Configures VLAN 10 (1st floor) and VLAN 20 (2nd floor) on a Catalyst 2960 switch with designated access ports, routing cross-VLAN traffic through an 802.1Q trunk link to sub-interfaces on a Cisco 2811 router. |
| `Activity 5_Conguis.pkt` | Multilayer Switch Inter-VLAN Routing (Layer 3 SVI) & Secure WLAN Integration | Implements Inter-VLAN routing directly on a Cisco Catalyst 3560 multilayer switch using Switched Virtual Interfaces (SVIs) for VLAN 10 (Main: 50.50.50.0) and VLAN 20 (Annex: 70.70.70.0), integrating a WPA/WPA2-secured wireless Access Point (SSID: LAB1) to serve wireless hosts alongside wired clients without an external router. |
| `Activity 6_Conguis.pkt` | Multi-Floor Inter-VLAN Routing (ROAS) & Wireless Access | Configures Router-on-a-Stick using a Cisco 2811 router and 2960 switch to route traffic between multi-floor segments (VLAN 10 1st-floor, VLAN 20 2nd-floor, VLAN 30 3rd-floor) over an 802.1Q trunk, integrating an access point to extend Layer 3 connectivity to wireless clients. |
| `Activity 7_Conguis.pkt` | VLAN Isolation & Centralized Server-Based DHCP Service | Configures access VLANs on a Cisco Catalyst 2960 switch to enforce strict broadcast containment between segmented hosts, integrating a dedicated network server running DHCP services (192.168.1.0/24) to automate host IP address provisioning across the subnet. |
| `Activity 8_Conguis.pkt` | Multi-Router Interface Routing & Router-Based Multi-VLAN DHCP Services | Utilizes a Cisco 2811 router with multiple routed physical interfaces (Fa 0/0 at 10.10.10.1 and Fa 0/1 at 20.20.20.1) connected to separate Catalyst 2960 switches, configuring native router DHCP pools to dynamically lease IP addresses to hosts in VLAN 10 (B1) and VLAN 20 (B2) while enabling full inter-VLAN routing. |
| `Activity 10_Conguis.pkt` | Multi-Segment Routed Enterprise Network with Integrated WLAN | Deploys a Cisco 2911 ISR router interconnecting three distinct switched subnets across routed GigabitEthernet interfaces (g0/0 for VLAN 10 10.10.10.0, g0/1 for VLAN 20 192.168.1.0, and g0/2 for VLAN 30 172.10.10.0), featuring WPA-secured wireless AP integration (SSID: LAB2) to facilitate full inter-subnet routing across wired and wireless hosts. |
| `Activity 11_Conguis.pkt` | Spanning Tree Protocol (STP) Topology Convergence & Port Role Election | Configures a redundant three-switch Layer 2 mesh using Cisco Catalyst 2960s to analyze Spanning Tree Protocol (STP) operations, evaluating Bridge ID (MAC: SW1, SW2, SW3) election of the Root Bridge, Root Ports (RP), Designated Ports (DP), and Non-Designated/Alternate blocking ports (NDP) to prevent switching loops. |
| `Activity1(Finals)_Conguis.pkt` | Layer 2 Security: DHCP Snooping & Rogue DHCP Server Mitigation | Implements Layer 2 network hardening on a Cisco Catalyst 2960 switch using DHCP Snooping on VLAN 10 (IT), establishing trusted uplinks (Fa0/1 to Router0, Fa0/2 to Main Server) and untrusted access ports to block unauthorized leases from a rogue/fake hacker DHCP server. |
| `Activity2(Finals)_Conguis.pkt` | Site-to-Site Wireless Bridge & SOHO Gateway Interconnection | Connects a Main Office and Annex building across a wireless bridge between two HomeRouter devices, distributing connectivity through downstream Catalyst 2960 switches to end workstations with customized local DHCP address pooling (192.168.1.1, starting IP: .200). |
| `Activity3(Finals)_Conguis.pkt` | Dual-LAN Architecture with Multi-Band Wireless & SOHO Routing | Designs two isolated networks (LAN1 and LAN2): LAN1 pairs a gateway router (192.168.1.1, start IP: .20) with a 2960 switch and an AP (SSID: LAB1) serving mobile clients; LAN2 demonstrates dual-band SOHO wireless routing across distinct 2.4 GHz (SSID: Main1) and 5.0 GHz (SSID: Main2) bands with integrated switched host distribution. |
| `Assignment 1_Conguis.pkt` | Multi-LAN Routing & Inter-Switch Uplink Expansion | Configures a Cisco 2911 router to route between two primary subnets (10.10.0.0/24 via G 0/0 and 192.168.0.0/24 via G 0/1), demonstrating Layer 2 switch expansion across an Ethernet crossover link (Switch0 to Switch1) to extend LAN1/LAN2 across a shared default gateway (10.10.0.254) while enabling routed reachability to LAN3 (PC2). |
| `MA1_Conguis.pkt` | Multi-Switch VLAN Trunking & Router-on-a-Stick (ROAS) | Configures VLAN 14 (172.100.20.0) and VLAN 15 (172.100.10.0) across two Catalyst 2960 switches connected via an 802.1Q trunk link (fa0/3 to fa0/3), routing inter-VLAN traffic through an upstream router (Router0) via sub-interfaces with shared gateways (.254). |
| `` |  |  |
| `` |  |  |
| `` |  |  |
| `` |  |  |
| `` |  |  |
| `` |  |  |

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
