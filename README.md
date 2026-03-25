# 🖧 Day 1 | Basic Network Topology Lab

## 🎯 Objective
Understand how network devices connect and communicate within the same network by building a simple topology in Cisco Packet Tracer.

---

## 🧱 Network Design

![Topology](https://github.com/Pelumi-Johnson/Basic-Network-Topology-Lab/blob/main/Topology.png)

The topology includes:
- 1 Router (1941)
- 1 Switch (2960)
- 2 PCs

### 🔗 Connections
- PC0 → Switch (FastEthernet0 → FastEthernet0/1)
- PC1 → Switch (FastEthernet0 → FastEthernet0/2)
- Switch → Router (FastEthernet0/24 → GigabitEthernet0/0)

All devices were connected using copper straight-through cables.

---

## ⚙️ Configuration

### Router Interface Activation
```
enable
configure terminal
interface gigabitEthernet 0/0
no shutdown
```
---

### IP Addressing

Assigned static IP addresses to both PCs and configured the default gateway.

![IP Configuration](https://github.com/Pelumi-Johnson/Basic-Network-Topology-Lab/blob/main/ipconfiguration.png)

PC0
- IP Address: 192.168.1.10
- Subnet Mask: 255.255.255.0
- Default Gateway: 192.168.1.1

PC1
- IP Address: 192.168.1.11
- Subnet Mask: 255.255.255.0
- Default Gateway: 192.168.1.1

Router
interface gigabitEthernet 0/0
ip address 192.168.1.1 255.255.255.0
no shutdown

---

## 📡 Connectivity Test

Used the ping command to verify communication between devices.

![Ping Test](ping-test.png)

ping 192.168.1.11

---

## 🧠 Key Concepts Learned

- A network allows devices to communicate using IP addressing
- The switch forwards traffic within the local network
- The router acts as a gateway for network communication
- Devices must be in the same subnet to communicate directly
- Ping verifies connectivity between devices

---

## ⚠️ Troubleshooting Insight

- Changed one device to a different IP network
- Communication failed due to subnet mismatch
- Reinforced importance of proper IP addressing

---

## 🔁 Practical Reinforcement

- Rebuilt the entire topology from memory without referencing instructions
- Strengthened understanding of device roles and network structure

---

## ✅ Outcome

- Successfully built and configured a basic network topology
- Verified communication between devices using ping
- Developed foundational understanding of network communication

---

## 📸 Topology

![Network Topology](topology.png)
