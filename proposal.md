# Hospital Network Design Proposal

## Departmental Structure

### Main Headquarters:
- Medical Lead Operation & Consultancy Services (MLOCS)  
- Medical Emergency and Reporting (MER)  
- Medical Records Management (MRM)  
- Information Technology (IT)  
- Customer Service (CS)  

### Branch Hospital:
- Nurses & Surgery Operations (NSO)  
- Hospital Labs (HL)  
- Human Resources (HR)  
- Marketing (MK)  
- Finance (FIN)  

Both sites also feature a Guest/Waiting Area (GWA) to accommodate patients and visitors.

---

## Network Infrastructure Requirements

Previously, Nexus Medical Center relied on external vendors for IT support. However, management has now decided to bring all network operations in-house. The new infrastructure will include:

- Local Area Networks (LANs) at both the headquarters and branch  
- Wide Area Network (WAN) connectivity between the two sites  
- A dedicated server area at the headquarters, connected via an access switch to the HQ router  

The server area will host essential services such as:

- DHCP Server  
- DNS Server  
- Web Server  
- Email Server  

---

## Design and Security Considerations

The network must be designed to be cost-effective while strictly adhering to the principles of Confidentiality, Integrity, and Availability (CIA). To ensure efficient and secure operations, the following measures are required:

- **Hierarchical Network Model:** The network will be structured using a hierarchical design for scalability and manageability.  
- **Core Routers:** Each site will utilize a core router (already acquired), with both routers connected to two different ISPs for redundancy.  
- **Segmentation:** Every department will operate on its own VLAN within the local network to enhance security and performance.  
- **Access Control:** Access Control Lists (ACLs) will be implemented to strictly regulate user and departmental access across the network.  
- **VPN Connectivity:** A Virtual Private Network (VPN) will be established between the two sites to ensure secure data transmission over the WAN.  

---

## Security Policy

A comprehensive network security policy will be developed to define user permissions and access at each location, enforced through ACLs. This policy will be designed to protect sensitive data, maintain system integrity, and ensure that critical services always remain available.

As the appointed network security engineer, your role is to design and implement this robust network architecture, ensuring that Nexus Medical Center’s IT infrastructure is secure, reliable, and aligned with industry best practices.
