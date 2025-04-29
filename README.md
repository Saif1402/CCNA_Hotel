# CCNA_Hotel
Hotel Network Design & Implementation

📘 Project Overview:
This project involves designing and implementing a multi-floor hotel network infrastructure using Cisco Packet Tracer. The hotel has three floors, each containing multiple departments, and uses advanced routing, VLANs, wireless connectivity, and security features to provide both internet access and internal communication.

🧱 Hotel Floor Plan and Department Layout
🟩 First Floor:
Reception – VLAN 80 – 192.168.8.0/24

Store – VLAN 70 – 192.168.7.0/24

Logistics – VLAN 60 – 192.168.6.0/24

🟦 Second Floor:
Sales & Marketing – VLAN 30 – 192.168.3.0/24

Human Resource (HR) – VLAN 40 – 192.168.4.0/24

Finance – VLAN 50 – 192.168.5.0/24

🟨 Third Floor:
IT Department – VLAN 10 – 192.168.1.0/24

Admin Department – VLAN 20 – 192.168.2.0/24

🧩 Network Devices and Topology
Routers: 3 routers (one for each floor) located in the server room.

Switches: 1 per floor (3 total).

Wireless Routers/Access Points: 1 per floor for guest/staff Wi-Fi.

Printers: 1 per department.

End Devices: PCs, laptops, smartphones.

Servers: Central DHCP, Web, and SSH access.

🔗 Network Configuration Summary
1. Routing:
OSPF (Open Shortest Path First) used for dynamic routing between VLANs and networks.

Router Interconnections:

10.10.10.0/30 – Router 1 ↔ Router 2

10.10.10.4/30 – Router 1 ↔ Router 3

10.10.10.8/30 – Router 2 ↔ Router 3

2. VLAN Setup:
8 VLANs created (VLAN 10 to VLAN 80).

Each department is isolated in its own VLAN for security and organization.

3. DHCP Configuration:
Each router acts as a DHCP server for its connected VLANs.

All devices get dynamic IP addresses via DHCP.

4. WiFi Configuration:
Wireless routers on each floor provide internet access to mobile devices and laptops.

Connected to core network via switches.

5. SSH Configuration:
SSH enabled on all routers for secure remote management using Test-PC in IT department.

6. Port Security:
Port fa0/1 on IT switch is restricted to Test-PC only.

Sticky MAC address learning used.

Violation mode set to shutdown for unauthorized access.

🔐 Security Measures Implemented
VLANs ensure data separation between departments.

SSH for secure router access.

Port Security restricts unauthorized device access.

DHCP prevents IP conflicts with centralized control.

📊 Project Benefits
Scalability: Easy to add more departments/floors in future.

Security: Strong isolation using VLANs and access controls.

Efficiency: Centralized management with OSPF and DHCP.

Mobility: Wireless coverage per floor for staff and guests.

💡 Key Skills Applied in the Project

Skill Area	Description
Network Design	Planning multi-floor topology with routers, switches, VLANs
Routing Protocols	Configured and implemented OSPF for inter-router communication
VLAN Configuration	Isolated departments using VLANs on switches
DHCP Configuration	Enabled automatic IP distribution via DHCP on routers
Wireless Networking	Provided Wi-Fi access using wireless routers per floor
Remote Access (SSH)	Enabled secure login to routers via SSH
Port Security	Restricted unauthorized access using sticky MAC and shutdown violation mode
Troubleshooting	Used ping, show commands, packet simulation to test connectivity and fix issues
Documentation	Created network diagrams, IP tables, and security notes
