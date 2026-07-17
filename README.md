# Enterprise Network VLSM and WAN Routing Lab 2

## Overview

This project demonstrates the design, expansion, and implementation of an enterprise network using Cisco Packet Tracer.

Starting from an existing 192.168.1.0/24 addressing scheme, the network was expanded using Variable Length Subnet Masking (VLSM) to efficiently utilize available IP addresses. Additional LAN and WAN segments were created while maintaining full connectivity between all sites and Internet services.

## Objectives

- Extend an existing enterprise network
- Implement VLSM subnetting
- Create additional LAN segments
- Configure point-to-point WAN links using /30 networks
- Configure DHCP services
- Configure routing between all sites
- Verify end-to-end connectivity

## Network Topology

The network consists of:

### Branch Site 1
- Router R1
- Switch1
- DHCP Server
- PC0, PC1, PC2

### Branch Site 2
- Router R2
- Switch2
- DHCP Server
- PC3, PC4, PC5

### Branch Site 3
- Router R4
- Switch3
- DHCP Server
- PC6, PC7, PC8

### Core Network
- Internet Router
- Internet Switch

### Internet Services
- DNS Server (8.8.8.8)
- Cisco.com Server
- Facebook.com Server

## Addressing Plan

### Existing Networks

| Network | Purpose |
|----------|----------|
| 192.168.1.0/26 | Site 1 LAN |
| 192.168.1.128/26 | Site 2 LAN |

### New VLSM Network

The subnet 192.168.1.64/26 was further divided using VLSM.

### LAN Subnet

| Network | Mask |
|----------|----------|
| 192.168.1.64/28 | Site 3 LAN |

### WAN Links

| Network | Mask |
|----------|----------|
| 192.168.1.112/30 | R1 ↔ Internet Router |
| 192.168.1.116/30 | R4 ↔ Internet Router |
| 192.168.1.192/26 | R2 ↔ Internet Router |

## Features Implemented

### VLSM Subnetting
Efficiently divided the available address space to support additional networks while minimizing IP wastage.

### DHCP Configuration
Configured DHCP services for automatic client IP assignment.

### WAN Configuration
Configured serial point-to-point links using /30 networks.

### Routing
Implemented routing between all branch offices and Internet services.

### Connectivity Testing
Verified communication using:
- Ping
- DHCP Lease Verification
- Browser Access

## Verification Results

✅ DHCP addresses assigned successfully

✅ Inter-site communication operational

✅ Branch sites successfully connected through WAN links

✅ Access verified to:

- cisco.com
- facebook.com
- 8.8.8.8

✅ Full network connectivity achieved

## Skills Demonstrated

- Cisco Packet Tracer
- VLSM Subnetting
- IPv4 Address Planning
- DHCP Configuration
- Static Routing
- WAN Technologies
- Point-to-Point Networking
- Network Design
- Network Troubleshooting
- Enterprise Network Deployment

## Technologies Used

- Cisco Packet Tracer
- IPv4 Networking
- VLSM
- DHCP
- Static Routing
- LAN/WAN Networking

## Learning Outcomes

This lab provided practical experience in:

- Designing scalable enterprise networks
- Implementing VLSM subnetting
- Optimizing IP address utilization
- Configuring WAN serial links
- Managing multi-site connectivity
- Troubleshooting routing and addressing issues
- Verifying enterprise-level network communication

## Repository Structure

```
├── Enterprise-Network-VLSM-and-WAN-Routing-Lab.pkt
├── topology.png
└── README.md
```

## Author

**Md. Mostafizur Rahman Zahid**

B.Sc. in Computer Science & Engineering

Cybersecurity | DevSecOps | Networking Enthusiast
