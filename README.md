# ZDC-Enterprise-Network-Project
Content:
1. Introduction
    ZDC is a medium-sized enterprise with three main facilities:
o	Two wired buildings designed with a 3-Tier Architecture (Core, Distribution, Access).
o	One wireless building for mobile devices and IoT.
o	A centralized Data Center connecting all buildings via high-speed links.
o	The network is connected to the internet through an ISP (WE) using a border router, with advanced protocols for redundancy, security, and efficiency.

Key Components:
o	Core Layer: High-speed routing between buildings and Data Center.
o	Distribution Layer: VLAN routing and traffic control.
o	Access Layer: End-user devices including PCs, IP phones, and printers.
o	Wireless Building: Configured with secure WLAN and DHCP services.
o	Data Center: Hosts critical servers and connects to the ISP.

3. Implemented Protocols & Technologies    
 A. VLANs & Inter-VLAN Routing
    o	Network segmentation was implemented for security and performance optimization, separating departments like HR, Finance, and Guest networks.
    o	Router-on-a-Stick configuration enabled communication between different VLANs.
 B. Redundancy with HSRP
    o	First Hop Redundancy Protocol was deployed to ensure continuous availability of gateway services for all VLANs.
    o	Primary and standby routers were configured with priority values to manage failover.
     
 C. Dynamic Routing with OSPF
    o	OSPF protocol was implemented to automate and optimize path selection between buildings and the data center.
    o	All network segments were placed in OSPF Area 0 for efficient routing.
 D. Loop Prevention with STP
    o	Spanning Tree Protocol in rapid-PVST mode was configured to prevent network loops while maintaining redundancy.
 E. Wireless Network Implementation
    o	A secure wireless network was established with WPA2-PSK encryption.
    o	Dedicated DHCP pool was created to manage IP assignments for wireless clients.
 F. Network Security Measures
    o	NAT Implementation: Network Address Translation was configured to mask internal IP addresses.
    o	Access Control Lists: ACLs were implemented to restrict unauthorized access attempts.
    o	Remote Access Security: Banner messages and VTY line security were configured to protect against unauthorized access.
    
 G. Centralized VLAN Management
    o	VTP protocol was deployed to synchronize VLAN databases across all network switches.
    o	A VTP server was designated to manage VLAN propagation throughout the network.
________________________________________
4. Internet Connectivity
    o	The border router was configured with a default route to the ISP (WE) gateway.
    o	Public IP addressing was properly implemented for external connectivity.
________________________________________


5. Testing & Verification
    o	Comprehensive testing confirmed successful inter-VLAN communication.
    o	Wireless connectivity tests verified proper association and DHCP functionality.
    o	Redundancy tests validated HSRP failover capabilities.
    o	Security measures were tested to ensure proper access restrictions.
________________________________________

6. Server Connectivity
 ISP is connected to three key servers:
    Server    	        Description
    FACEBOOK            Facebook Recognition Server
    YOUTUBE    	        YouTube Streaming Server
    TWITTER	            Twitter Integration Server
