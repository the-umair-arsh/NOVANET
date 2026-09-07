# 🌐 NOVANET INTERNET SERVICE PROVIDER COMPANY (Multi-City Enterprise Network Simulation)

<p align="center">
  <b>A Cisco Packet Tracer-based enterprise network simulation designed with VLAN segmentation, IP addressing, DHCP, DNS, and inter-network connectivity.</b>
</p>

<p align="center">

![Cisco](https://img.shields.io/badge/Cisco%20Packet%20Tracer-1BA0D7?style=for-the-badge\&logo=cisco\&logoColor=white)
![Networking](https://img.shields.io/badge/Computer%20Networking-005571?style=for-the-badge)
![VLAN](https://img.shields.io/badge/VLAN-802.1Q-6A1B9A?style=for-the-badge)
![DHCP](https://img.shields.io/badge/DHCP-Enabled-2E7D32?style=for-the-badge)
![DNS](https://img.shields.io/badge/DNS-Configured-1565C0?style=for-the-badge)

</p>

<p align="center">

![GitHub Repo Size](https://img.shields.io/github/repo-size/the-umair-arsh/NOVANET?style=flat-square)
![GitHub Last Commit](https://img.shields.io/github/last-commit/the-umair-arsh/NOVANET?style=flat-square)
![GitHub Stars](https://img.shields.io/github/stars/the-umair-arsh/NOVANET?style=flat-square)
![GitHub Forks](https://img.shields.io/github/forks/the-umair-arsh/NOVANET?style=flat-square)

</p>

---

## 📌 About the Project

**NOVANET** is a multi-city enterprise network simulation developed in **Cisco Packet Tracer**.

The project demonstrates how a structured enterprise network can be designed by separating different types of users into dedicated **VLANs**, assigning IP addresses dynamically through **DHCP**, providing **DNS services**, and establishing connectivity between different network segments and cities.

The network is designed around three main user groups in each city:

* 👥 **VLAN 10 — Normal Users**
* 🏛️ **VLAN 20 — Government Users**
* 🏢 **VLAN 30 — Company Users**

This segmentation provides logical separation between departments/user groups while allowing the overall network to be managed as an organized enterprise infrastructure.

---

## 🎯 Project Objectives

The main objectives of NOVANET are to:

* Design a structured multi-city enterprise network
* Implement VLAN-based network segmentation
* Separate normal, government, and company users
* Configure IP addressing for different network segments
* Implement DHCP for automatic IP assignment
* Configure DNS services
* Establish communication between network segments
* Demonstrate practical routing and switching concepts
* Simulate a realistic enterprise networking environment using Cisco Packet Tracer

---

## 🏗️ Network Architecture

Each city in the simulated network contains three logical user networks.

```text
                         NOVANET
                            │
              ┌─────────────┼─────────────┐
              │             │             │
           CITY 1         CITY 2        CITY 3
              │             │             │
        ┌─────┼─────┐ ┌─────┼─────┐ ┌─────┼─────┐
        │     │     │ │     │     │ │     │     │
      VLAN10 VLAN20 VLAN30  VLAN10 VLAN20 VLAN30 ...
        │     │     │ │     │     │
      Users   Govt Company Users  Govt Company
```

The same logical VLAN structure is maintained across the different cities to provide consistent network organization.

---

## 🔀 VLAN Segmentation

VLANs are used to logically separate different categories of users within the network.

|   VLAN | User Group       | Purpose                            |
| -----: | ---------------- | ---------------------------------- |
| **10** | Normal Users     | General network users              |
| **20** | Government Users | Government-related network segment |
| **30** | Company Users    | Company/enterprise network segment |

### Why VLANs?

VLAN segmentation helps:

* Reduce unnecessary broadcast traffic
* Separate different user groups
* Improve network organization
* Provide logical isolation between departments
* Make network administration easier
* Provide a scalable structure for an enterprise network

---

## 🌐 IP Addressing

The network uses dedicated IP addressing for its different network segments.

Each VLAN represents a separate logical network, allowing devices belonging to different user groups to be organized into their respective subnets.

The IP addressing structure is designed to support:

```text
City
 ├── VLAN 10 → Normal Users
 ├── VLAN 20 → Government Users
 └── VLAN 30 → Company Users
```

This approach makes the network easier to manage and allows routing between required network segments.

---

## 📡 DHCP Configuration

**DHCP (Dynamic Host Configuration Protocol)** is implemented to automatically provide network configuration to client devices.

Instead of manually configuring every workstation, DHCP can provide the required network information automatically.

Typical DHCP-provided information includes:

* IP address
* Subnet mask
* Default gateway
* DNS server

### Benefits

* Reduces manual configuration
* Prevents common addressing mistakes
* Makes adding new devices easier
* Simplifies network administration

---

## 🌍 DNS Configuration

The project also includes **DNS (Domain Name System)** functionality.

DNS allows network devices to resolve configured domain/host names into IP addresses instead of requiring users to remember numerical IP addresses.

This demonstrates how common enterprise network services can operate alongside VLANs, DHCP, and routing.

---

## 🔄 Inter-Network Connectivity

The network is designed to allow communication between the different network segments where required.

The overall architecture demonstrates connectivity between:

```text
VLAN 10 ─────┐
             │
VLAN 20 ─────┼── Network Infrastructure ── Other VLANs
             │
VLAN 30 ─────┘
                    │
                    ↓
               Other Cities
```

This demonstrates practical concepts such as:

* VLAN-based segmentation
* Routing between different networks
* Gateway configuration
* Multi-network communication
* Inter-city connectivity

---

## 🧩 Core Networking Concepts Demonstrated

The project provides practical implementation of:

| Concept                      | Implementation                            |
| ---------------------------- | ----------------------------------------- |
| **VLANs**                    | User-group network segmentation           |
| **IP Addressing**            | Separate addressing for network segments  |
| **DHCP**                     | Automatic client configuration            |
| **DNS**                      | Name resolution                           |
| **Routing**                  | Communication between different networks  |
| **Switching**                | LAN connectivity                          |
| **Inter-VLAN Communication** | Connectivity between VLANs where required |
| **Multi-City Networking**    | Connecting separate city networks         |
| **Network Design**           | Structured enterprise topology            |

---

## 🗺️ Logical Network Model

```text
                    ┌─────────────────────┐
                    │      NOVANET        │
                    │ Enterprise Network  │
                    └──────────┬──────────┘
                               │
             ┌─────────────────┼─────────────────┐
             │                 │                 │
             ▼                 ▼                 ▼
         ┌────────┐        ┌────────┐        ┌────────┐
         │ CITY 1 │        │ CITY 2 │        │ CITY 3 │
         └───┬────┘        └───┬────┘        └───┬────┘
             │                 │                 │
        ┌────┼────┐       ┌────┼────┐       ┌────┼────┐
        │    │    │       │    │    │       │    │    │
       V10  V20  V30     V10  V20  V30     V10  V20  V30
        │    │    │       │    │    │       │    │    │
      Users Govt Company Users Govt Company Users Govt Company
```

> **Note:** The diagram represents the logical organization of the network. The actual topology and device placement are contained in the Cisco Packet Tracer project file.

---

## 🛠️ Tools & Technologies

| Technology                   | Purpose                                       |
| ---------------------------- | --------------------------------------------- |
| **Cisco Packet Tracer**      | Network simulation and topology design        |
| **Cisco Networking Devices** | Routing and switching infrastructure          |
| **VLAN**                     | Logical network segmentation                  |
| **DHCP**                     | Dynamic IP configuration                      |
| **DNS**                      | Domain/name resolution                        |
| **IP Addressing**            | Network communication and subnet organization |

---

## 📁 Repository Structure

```text
NOVANET/
│
├── NOVANET.pkt
└── README.md
```

### `NOVANET.pkt`

The main Cisco Packet Tracer project file containing the complete simulated network topology, device configurations, VLANs, IP addressing, DHCP/DNS configuration, and network connectivity.

---

## 🚀 How to Run the Project

### Requirements

You need:

* **Cisco Packet Tracer**
* The `NOVANET.pkt` project file

### Steps

1. Download or clone this repository.
2. Open **Cisco Packet Tracer**.
3. Open the following file:

```text
NOVANET.pkt
```

4. Wait for the topology to load.
5. Inspect the configured routers, switches, PCs, servers, and network connections.
6. Use Cisco Packet Tracer's simulation/realtime modes to test network connectivity and services.

---

## 🧪 Suggested Testing

After opening the project, the network can be tested by checking:

### VLAN Connectivity

Verify that devices are assigned to their intended VLANs:

```text
VLAN 10 → Normal Users
VLAN 20 → Government Users
VLAN 30 → Company Users
```

### DHCP

Check whether client devices receive their IP configuration automatically.

### DNS

Verify configured DNS services and name resolution.

### Inter-VLAN Communication

Test communication between devices belonging to different VLANs where communication is intended.

### Inter-City Connectivity

Verify communication between the different city networks.

---

## 🔐 Network Segmentation

One of the important design principles demonstrated in NOVANET is **logical network separation**.

Instead of placing every device into a single large LAN, users are divided according to their organizational role:

```text
                 Enterprise Network
                        │
        ┌───────────────┼───────────────┐
        │               │               │
    Normal Users   Government Users  Company Users
       VLAN 10         VLAN 20          VLAN 30
```

This provides a cleaner and more manageable network architecture.

---

## 📈 Scalability

The VLAN-based design provides a foundation that can be extended as the network grows.

Future additions could include:

* Additional cities
* Additional departments
* More VLANs
* Wireless networks
* Security policies
* Access Control Lists (ACLs)
* Redundant links
* Centralized network services
* Network monitoring

---

## 🔮 Future Improvements

Potential future improvements include:

* 🔐 Advanced security and ACL implementation
* 🛡️ Firewall integration
* 📡 Wireless network integration
* 🔁 Redundant network paths
* 📊 Network monitoring and management
* 🔒 Enhanced inter-VLAN security policies
* 🌐 Additional enterprise services
* 📈 Expansion to more cities and departments
* ⚙️ Improved fault tolerance and redundancy

---

## 🎓 Learning Outcomes

Through this project, the following networking concepts are practically demonstrated:

* Understanding enterprise network architecture
* VLAN creation and segmentation
* IP addressing and subnetting
* DHCP configuration
* DNS configuration
* Routing and switching
* Inter-VLAN communication
* Multi-network connectivity
* Network troubleshooting
* Designing a scalable network topology

---

## 👨‍💻 Author

### Muhammad Umair

**BS Software Engineering Student**

<p>
  <a href="https://github.com/the-umair-arsh">
    <img src="https://img.shields.io/badge/GitHub-the--umair--arsh-181717?style=for-the-badge&logo=github&logoColor=white">
  </a>
  <a href="https://www.linkedin.com/in/muhammad-umair-se">
    <img src="https://img.shields.io/badge/LinkedIn-Muhammad%20Umair-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white">
  </a>
</p>

---

## ⭐ Project

If you find this project useful or interesting, consider giving the repository a ⭐ on GitHub.

<p align="center">
  <b>NOVANET</b><br>
  Multi-City Enterprise Network Simulation<br><br>
  Built with Cisco Packet Tracer
</p>
