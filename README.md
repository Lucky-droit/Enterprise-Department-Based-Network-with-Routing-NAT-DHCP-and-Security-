# Enterprise Department-Based Network with Routing, NAT, DHCP and Security

## 📌 Project Overview
This project demonstrates the design, implementation, and troubleshooting of a department-based enterprise network using Cisco Packet Tracer. The network is segmented using VLANs and secured using ACLs and port security, with inter-VLAN routing, centralized DHCP, and NAT providing internet access to internal users.

The lab is designed to simulate real-world enterprise networking and NOC-level troubleshooting scenarios.

---

## 🏢 Network Design
The enterprise network is divided into multiple departments, each mapped to a dedicated VLAN and IP subnet:

| Department | VLAN | Network |
|----------|------|---------|
| HR | VLAN 10 | 192.168.10.0/24 |
| IT | VLAN 20 | 192.168.20.0/24 |
| Admin | VLAN 30 | 192.168.30.0/24 |
| Management | VLAN 40 | 192.168.40.0/24 |

- A Layer 2 switch provides access-layer connectivity.
- A router is used for inter-VLAN routing (Router-on-a-Stick).
- An 802.1Q trunk connects the switch and router.
- Internet access is simulated using a cloud connection.

---

## ⚙️ Technologies Used
- Cisco Packet Tracer  
- VLANs and Access Ports  
- 802.1Q Trunking  
- Inter-VLAN Routing (Router-on-a-Stick)  
- DHCP (Router-Based)  
- NAT Overload (PAT)  
- Standard and Extended ACLs  
- Switch Port Security (Sticky MAC)  
- Cisco IOS Diagnostic Commands  

---

## 🔐 Key Configurations
- VLAN creation and department-based segmentation
- Router subinterfaces configured as default gateways
- DHCP pools created per VLAN with excluded gateway addresses
- NAT overload configured for internet access
- Standard and extended ACLs applied to enforce security policies
- Port security enabled on access ports to restrict unauthorized devices

---

## 🧪 Verification & Testing
The following checks were performed:
- DHCP IP assignment and gateway verification
- Inter-VLAN connectivity testing using `ping`
- NAT translation verification using `show ip nat translations`
- ACL behavior verification using `show access-lists`
- Port security validation using `show port-security`

---

## 🛠️ Troubleshooting Scenarios Covered
- Hosts not receiving IP addresses from DHCP
- Inter-VLAN routing failures
- NAT translation issues blocking internet access
- ACLs unintentionally blocking traffic
- Port security violations due to unknown MAC addresses

---

## 🎯 Learning Outcomes
- Practical understanding of enterprise VLAN architecture
- Hands-on experience with DHCP, NAT, and routing
- Real-world application of ACLs and port security
- Improved troubleshooting and fault-isolation skills
- Exposure to enterprise network design best practices

---

## 👤 Author
**Lucky Prajapati**   
