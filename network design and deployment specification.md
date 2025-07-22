# Network Design & Deployment Specifications

## Simulation Environment  
Develop and simulate the network architecture using Cisco Packet Tracer.

## Structured Topology  
Employ a hierarchical network structure that incorporates redundancy to minimize downtime.

## WAN Connectivity  
Establish a serial link between the core routers at the main site and the branch office.

## Core Infrastructure  
Each location should utilize a single core router, two multilayer switches, and multiple access switches to interconnect departmental areas, optimizing both cost and performance.

## Wireless Access  
Ensure that every department is equipped with its own wireless network to support user mobility.

## User Estimates  
Plan for approximately 60 users per department at headquarters and about 30 users per department at the branch.

## VLAN Segmentation  
Assign a unique VLAN and subnet to each department for improved security and traffic management.

## IP Addressing  
Starting with the 192.168.100.0 network, perform subnetting to allocate appropriate address ranges based on departmental size.

## Internet Connectivity  
Connect the organization’s network to the internet using the static public IP ranges 195.136.17.0/30, 195.136.17.4/30, 195.136.17.8/30, and 195.136.17.12/30, distributed across two different ISPs for redundancy.

## Device Configuration  
Set up essential device parameters such as hostnames, console and enable passwords, login banners, and disable unnecessary services like IP domain lookup.

## Inter-Department Communication  
Enable inter-VLAN routing on multilayer switches to allow seamless communication between departments.

## Switching & Routing  
Configure multilayer switches to handle both Layer 2 and Layer 3 operations, assigning them appropriate IP addresses.

## Dynamic Addressing  
All end-user devices should receive IP addresses automatically from the DHCP servers located in the server area.

## Static Assignments  
Devices within the server room must be configured with static IP addresses for stability and ease of management.

## Routing Protocol  
Implement OSPF on both routers and multilayer switches to dynamically share routing information throughout the network.

## Default Routing  
Set up default static routes on routers and multilayer switches, using next-hop IP addresses to forward any unmatched traffic.

## Secure Remote Access  
Enable SSH on all routers and Layer 3 switches to facilitate secure remote management.

## Port Security  
On the server room’s access switch, restrict each port to a single device using sticky MAC address learning, and set the violation mode to shut down.

## Secure Site Interconnect  
Deploy extended ACLs alongside an IPSec VPN tunnel to encrypt and secure communications between headquarters and the branch.

## NAT Configuration  
Implement Port Address Translation (PAT) using the outgoing router interface’s IPv4 address and apply the necessary access control rules.

## Verification  
Conduct comprehensive testing to ensure all configurations function correctly and meet the specified requirements.

---

# Technologies Utilized

- **Network Topology Design:** Developed the entire network structure using Cisco Packet Tracer.  
- **Hierarchical Architecture:** Applied a layered network design for scalability and resilience.  
- **Proper Device Interconnection:** Utilized appropriate cabling to link all networking hardware.  
- **Initial Device Setup:** Configured essential settings such as hostnames, passwords, and banners on all devices.  
- **VLAN Configuration:** Established Virtual LANs and assigned ports to specific VLAN IDs for departmental segmentation.  
- **IP Address Management:** Performed subnetting and assigned IP addresses to all network segments.  
- **Inter-VLAN Routing:** Enabled routing between VLANs on multilayer switches using Switch Virtual Interfaces (SVIs).  
- **Dynamic IP Assignment:** Set up dedicated DHCP servers to automatically allocate IP addresses to devices.  
- **Secured Remote Administration:** Implemented SSH to allow encrypted remote access to network devices.  
- **Dynamic Routing:** Configured OSPF as the primary routing protocol for efficient path selection.  
- **Network Address Translation:** Deployed PAT (Port Address Translation) to enable multiple devices to share a single public IP.  
- **Secure Site Connectivity:** Established a site-to-site IPsec VPN for encrypted communication between locations.  
- **Access Control:** Applied both standard and extended ACLs to manage and restrict network traffic.  
- **Port Security:** Enabled switchport security features to control device access on switch ports.  
- **Wireless Networking:** Configured Cisco Access Points to provide wireless connectivity for users.  
- **End Device Setup:** Completed configuration of host devices for network access.  
- **ISP Router Configuration:** Set up routers to connect the internal network to external Internet Service Providers.  
- **Network Testing & Validation:** Verified all connections and configurations to ensure seamless communication.  
- **Network Interface Management:** Managed network adapters and ensured compatibility within Packet Tracer.
