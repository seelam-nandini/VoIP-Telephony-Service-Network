# VoIP-Telephony-Service-Networking Project with Dial Peering
Designing and implementing a network infrastructure by interconnecting four departments, which are as follows:
Finance: 20 phones, 20 PCs, and 1 printer
Sales: 20 phones, 20 PCs, and 1 printer
HR: 20 phones, 20 PCs, and 1 printer
ICT: 20 phones, 20 PCs, and 1 printer
All desktops have an associated telephone set (each PC is connecting directly to a Phone, not a switch). The network consists of four servers located at the server-side site and is fully configured for operations; all servers are shared between all users. The four servers are HTTP,DNS,Email, and DHCP.

## Requirements:

To emphasize scalability and availability, we are required to provide a complete network infrastructure design and implementation. We will be using the following IP addresses: 192.168.100.0/24 for Data, 172.16.100.0/24 for Voice, and 10.10.10.0/24 between the routers.

1. Designing a networked system.We use packet tracer software to design your network.
2. **Routers:** Each department is to have a VoIP-enabled router with a server-side LAN attached to the ICT department router. Use a Cisco 2811 router.
3. **Switches:** Each department has an access layer switch. Use the Cisco 2960 switch.
4. **Connections:** Use serial connections between a router and a router, then a straight-through cable between the router and the switches, the switches and the hosts, and phones to PCs.
5. **Subnets:** Each department will be accessing two subnetworks, for example, data and voice subnets.
6. **Basic settings:** Configure basic device settings such as hostnames, console passwords, enabling passwords, banner messages, encrypting all passwords, and disabling IP domain lookup.
7. **DHCP Server:** For voice (VoIP), use the respective router as the DHCP server, while for data, use the DHCP server device at the server-side site.
   **VLANs:** Each department will have two VLANs. One for data and another for voice. All IP phones in the network should be in VLAN 100.
9. **Inter-VLAN Routing:** Use a router-on-a-stick to enable inter-VLAN routing on the network. Create subinterfaces for both data and voice VLANs.
10. **IP Addressing:** All devices in the network are expected to obtain an IP address dynamically from the respective DHCP servers, while the devices in the server room are to be allocated IP addresses statically.
11. **Routing protocol:** Use OSPF as the routing protocol to advertise routes on the routers.
12. **Remote Access:** Configure SSH on all the routers for remote login.
13. **Telephony service:** Configure VoIP on the routers and allocate dial numbers in this format for the departments Finance (1..), HR (2..), Sales (3..), and ICT (4..), where 1.. can be 101 to 199, and so on.
14. **Routing for VoIP:** Configure dial-peering on the routers to allow IP phones from different routers to communicate.
15. **Finalize:** Test communication and ensure everything configured is working as expected.
