# Enterprise Campus Network Simulation

[![Cisco Packet Tracer](https://img.shields.io/badge/Cisco-Packet_Tracer-blue?logo=cisco&logoColor=white)](https://www.netacad.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An enterprise multi-floor campus network infrastructure designed and simulated using **Cisco Packet Tracer** and **Cisco IOS CLI**. This project demonstrates scalable network architecture, dynamic interior gateway routing (OSPF), hierarchical IP addressing using Variable Length Subnet Masking (VLSM), and perimeter security filtering via Access Control Lists (ACLs).

---

## 🏗️ Architecture & Topology Highlights

* **Multi-Floor Campus Design:** 3-floor enterprise office structure segmented into 4 dedicated departments (Engineering, Operations, Administration, and Management).
* **High Availability Backbone:** Multi-router mesh topology interconnected across redundant router links.
* **Efficient Address Allocation (VLSM):** Implemented CIDR-based Variable Length Subnet Masking to eliminate IP address waste across 3,500+ host endpoints and point-to-point /30 inter-router links.
* **Dynamic Routing Protocol (OSPF Area 5):** Configured Single-Area OSPF with automated path convergence, fast neighbor adjacencies, and dynamic route redistribution.
* **Access Control & Security (Standard & Extended ACL):** Granular traffic filtering policies to restrict unauthorized inter-VLAN / inter-departmental communication while permitting business-critical application traffic (HTTP, DNS, ICMP).

---

## 📁 Repository Structure

```text
├── campus_network_simulation.pkt   # Main Cisco Packet Tracer project file
├── lat1.pkt                         # Original lab configuration file
├── configs/                         # IOS CLI startup & running configurations
└── README.md                        # Documentation & architecture breakdown
```

---

## 🚀 How to Open & Inspect

1. Download and install **[Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer)** (Version 8.0 or newer recommended).
2. Clone this repository:
   ```bash
   git clone https://github.com/farrelwidjaja/cisco-network-topology-simulation.git
   ```
3. Open `campus_network_simulation.pkt` or `lat1.pkt` inside Cisco Packet Tracer.
4. Test reachability across departments using the command line:
   ```bash
   ping <destination-ip>
   traceroute <destination-ip>
   ```

---

## 👨‍💻 Author
**Farrel Widjaja**  
*Computer Science Student at BINUS University (Cloud Computing & Network Engineering)*  
* [Portfolio Website](https://farrelwidjaja.vercel.app/)
* [LinkedIn Profile](https://linkedin.com/in/farrelwidjaja)
* [GitHub Profile](https://github.com/farrelwidjaja)
