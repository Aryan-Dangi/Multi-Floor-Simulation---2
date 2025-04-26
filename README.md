Alpha Infotech Office Network Design
Project Overview
This project involves the design and simulation of a scalable, efficient network for Alpha Infotech, a mid-sized enterprise operating across a 5-floor office building. The network was modeled using Cisco Packet Tracer with an emphasis on topology planning, IP addressing, dynamic/static routing, server deployment, and DNS management to enable seamless internal communication.

Network Topology
Topology Types:

Ring Topology: Floors 1 to 3

Bus Topology: Floors 4 and 5

Interconnection:

Each floor uses a dedicated 2960 switch.

Each floor’s switch connects to a 2911 router.

Routers of each floor are connected in a bus structure.

IP Addressing Scheme
Floors 1 & 2: Class A Private IP addresses (10.x.x.x)

Floors 3, 4 & 5: Class A Public IP addresses (8.x.x.x)

Addressing Method: VLSM (Variable Length Subnet Masking) applied to efficiently allocate IP addresses based on host requirements.

Server Setup
Email Server: Floor 1 (IP: 10.0.0.2, Domain: alphainfotech.com)

DNS Server: Floor 2

HTTP Server: Floor 3 (IP: 8.0.0.2, Domain: www.alphainfotech.com)

FTP Server: Floor 5 (IP: 8.0.132.3, Domain: ftp.alphainfotech.com)

DHCP Server: Floor 5

Routing Configuration
Routing Type: Static Routing (configured manually between all routers).

Static routes are defined on each router to ensure seamless communication across floors.

Each router knows the exact paths to reach networks from other floors.

DNS Configuration
A DNS server was configured to resolve domain names internally.

Mappings include:

alphainfotech.com → 10.0.0.2

ftp.alphainfotech.com → 8.0.132.3

www.alphainfotech.com → 8.0.0.2

Additional Information
Subnets were carefully designed using VLSM calculations.

The project ensures future scalability, reliability, and high-speed communication between departments.

Testing was conducted through successful ping tests and domain name resolution.

