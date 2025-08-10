# ZDC Enterprise Network Project

## 1. Introduction
ZDC is a medium-sized enterprise with three main facilities:
- **Two wired buildings** designed with **3-Tier Architecture** (Core, Distribution, Access)
- **One wireless building** for mobile devices and IoT
- **Centralized Data Center** connecting all buildings via high-speed links
- Network connected to the internet through **ISP (WE)** using border router with advanced protocols for redundancy, security, and efficiency

## 2. Key Components
- **Core Layer**: High-speed routing between buildings and Data Center
- **Distribution Layer**: VLAN routing and traffic control
- **Access Layer**: End-user devices (PCs, IP phones, printers)
- **Wireless Building**: Secure WLAN with DHCP services
- **Data Center**: Hosts critical servers and ISP connection

## 3. Implemented Protocols & Technologies

### A. VLANs & Inter-VLAN Routing
- Network segmentation for security/performance (HR, Finance, Guest networks)
- Router-on-a-Stick configuration for inter-VLAN communication

### B. Redundancy with HSRP
- First Hop Redundancy Protocol for gateway availability
- Priority-based failover between primary/standby routers

### C. Dynamic Routing with OSPF
- Automated path selection between buildings/data center
- All segments in OSPF Area 0 for efficient routing

### D. Loop Prevention with STP
- Rapid-PVST mode to prevent loops while maintaining redundancy

### E. Wireless Network Implementation
- Secure WPA2-PSK encryption
- Dedicated DHCP pool for wireless clients

### F. Network Security Measures
- **NAT**: Masks internal IP addresses
- **ACLs**: Restrict unauthorized access
- **Remote Access Security**: Banner messages + VTY line protection

### G. Centralized VLAN Management
- VTP protocol for VLAN database synchronization
- Designated VTP server for VLAN propagation

## 4. Internet Connectivity
- Border router configured with default route to ISP (WE) gateway
- Proper public IP addressing implementation

## 5. Testing & Verification
✔ Inter-VLAN communication  
✔ Wireless connectivity & DHCP  
✔ HSRP failover capabilities  
✔ Access restriction validation  

## 6. Server Connectivity
| Server       | Description                     |
|--------------|---------------------------------|
| FACEBOOK     | Facebook Recognition Server     |
| YOUTUBE      | YouTube Streaming Server        |
| TWITTER      | Twitter Integration Server      |
