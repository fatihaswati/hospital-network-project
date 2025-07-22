# Hospital Network Design - Nexus Medical Center

## Project Overview  
This project implements a robust and secure network design for Nexus Medical Center's headquarters and branch using Cisco Packet Tracer. The network supports departmental segmentation, reliable WAN connectivity, and strong security policies.

## Features  
- VLAN segmentation per department  
- Site-to-site IPsec VPN  
- Redundant ISP connections  
- Dynamic routing with OSPF  
- Secure remote management via SSH  
- Port Security implementation

## Network Design  
The network uses a hierarchical model with core routers, multilayer switches, access switches, and dedicated wireless networks. Each department operates within its own VLAN and subnet to improve security and network management.

## IP Addressing  
Starting with 192.168.100.0/24, subnetted per department according to user count, with static addresses for servers and dynamic DHCP allocation for end devices.

## Setup Instructions  
Open the Cisco Packet Tracer file included in this repository to simulate the network. Device configurations can be viewed and modified as needed.

## Testing and Validation  
All configurations have been validated for connectivity, routing, access control enforcement, and VPN tunnel stability.

## Technologies  
- Cisco Packet Tracer  
- VLANs, DHCP, OSPF, ACLs  
- IPsec VPN  
- SSH, NAT (PAT)

## Author  
Fateha Rashid
