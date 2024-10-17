Here’s a comprehensive cheat sheet for **Computer Networks**:

### 1. **OSI Model**
The OSI (Open Systems Interconnection) model is a framework used to understand and design a network architecture in seven layers.

| Layer | Name                  | Function                                                                          | Protocols/Technologies                          |
|-------|-----------------------|-----------------------------------------------------------------------------------|------------------------------------------------|
| 7     | Application            | Interfaces with software, user applications                                       | HTTP, FTP, SMTP, DNS, Telnet                   |
| 6     | Presentation           | Data translation, encryption/decryption, compression                              | SSL, TLS, JPEG, GIF, MPEG                      |
| 5     | Session                | Manages sessions between applications                                             | NetBIOS, PPTP, SIP                             |
| 4     | Transport              | End-to-end communication, reliability, flow control                               | TCP, UDP                                       |
| 3     | Network                | Logical addressing, routing                                                       | IP, ICMP, IPsec, RIP, OSPF, BGP                |
| 2     | Data Link              | Physical addressing, error detection, MAC addressing, frame control               | Ethernet, PPP, MAC addresses, ARP              |
| 1     | Physical               | Physical transmission of data (electrical, optical signals)                       | Hubs, Cables, Fiber optics, Wi-Fi              |

### 2. **TCP/IP Model**
Simplified compared to OSI, TCP/IP is more widely used for real-world networking.

| Layer | Name                  | Function                                                                          | Protocols/Technologies                          |
|-------|-----------------------|-----------------------------------------------------------------------------------|------------------------------------------------|
| 4     | Application            | Combines OSI Application, Presentation, and Session layers                        | HTTP, FTP, SMTP, DNS                           |
| 3     | Transport              | Provides end-to-end communication and error checking                              | TCP, UDP                                       |
| 2     | Internet               | Defines IP addressing and routing                                                 | IP, ICMP, ARP, RARP                            |
| 1     | Network Access         | Physical transmission and data framing                                            | Ethernet, Wi-Fi, Frame Relay                   |

### 3. **Common Networking Protocols**
- **TCP (Transmission Control Protocol):** Reliable, connection-oriented, ensures data delivery (e.g., web browsing, email).
- **UDP (User Datagram Protocol):** Faster, connectionless, used where speed is prioritized over reliability (e.g., video streaming).
- **IP (Internet Protocol):** Provides logical addressing (IPv4: 32-bit, IPv6: 128-bit) and routes packets across networks.
- **ICMP (Internet Control Message Protocol):** Used for error messages and network diagnostics (e.g., ping).
- **DNS (Domain Name System):** Resolves domain names to IP addresses.
- **DHCP (Dynamic Host Configuration Protocol):** Dynamically assigns IP addresses to devices in a network.

### 4. **IP Addressing**
- **IPv4:** 32-bit, divided into 4 octets (e.g., 192.168.1.1).
  - **Classes:**
    - **Class A:** 1.0.0.0 to 126.0.0.0 (Supports ~16M hosts)
    - **Class B:** 128.0.0.0 to 191.255.0.0 (Supports ~65,000 hosts)
    - **Class C:** 192.0.0.0 to 223.255.255.0 (Supports ~256 hosts)
- **IPv6:** 128-bit, provides larger address space (e.g., 2001:0db8:85a3::8a2e:0370:7334).

### 5. **Subnetting**
- Subnetting divides an IP network into smaller subnetworks.
- **Subnet Mask:** Helps identify the network and host portion of an IP address.
  - **Default Subnet Masks:**
    - **Class A:** 255.0.0.0
    - **Class B:** 255.255.0.0
    - **Class C:** 255.255.255.0

**CIDR Notation (Classless Inter-Domain Routing):**
- Example: **192.168.1.0/24** means the first 24 bits are for the network, and the rest for hosts.

### 6. **Routing Protocols**
- **Static Routing:** Manually defined routes.
- **Dynamic Routing:** Routes are automatically updated.
  - **RIP (Routing Information Protocol):** Distance-vector protocol, slow convergence.
  - **OSPF (Open Shortest Path First):** Link-state protocol, faster convergence, uses Dijkstra’s algorithm.
  - **BGP (Border Gateway Protocol):** Used for routing between autonomous systems (Internet).

### 7. **Switching**
- **Circuit Switching:** Dedicated communication path between two endpoints (e.g., telephone networks).
- **Packet Switching:** Data divided into packets, each may take different paths (e.g., internet).
- **Switches (Layer 2):** Direct data based on MAC addresses.

### 8. **VLAN (Virtual LAN)**
- Logical grouping of devices into separate networks within the same physical switch.
- **802.1Q Protocol:** Used to tag VLAN traffic.

### 9. **Network Security Protocols**
- **WPA2 (Wi-Fi Protected Access 2):** Encryption for wireless networks.
- **IPsec (Internet Protocol Security):** Secures IP communications by authenticating and encrypting each IP packet.
- **SSL/TLS (Secure Socket Layer/Transport Layer Security):** Encryption protocols for securing communications on the web.

### 10. **Firewalls & Network Address Translation (NAT)**
- **Firewalls:** Control incoming and outgoing network traffic based on predetermined security rules.
  - **Types:** Packet-filtering, Stateful, Proxy, Next-Gen.
- **NAT (Network Address Translation):** Translates private IP addresses to a public IP address to communicate over the internet.
  - **PAT (Port Address Translation):** Maps multiple private IP addresses to a single public IP using different ports.

### 11. **Wireless Networking (Wi-Fi Standards)**
- **802.11a/b/g/n/ac/ax:** Various Wi-Fi standards.
  - **802.11ac:** Supports up to 1.3 Gbps.
  - **802.11ax (Wi-Fi 6):** Supports up to 10 Gbps, more efficient in crowded areas.

### 12. **VPN (Virtual Private Network)**
- Creates a secure, encrypted connection over a less secure network like the internet.
  - **Types:** Remote-access VPN, Site-to-site VPN.
  - **Protocols:** PPTP, L2TP, OpenVPN.

### 13. **Common Network Devices**
- **Router:** Routes data between different networks.
- **Switch:** Connects devices in a network and filters traffic using MAC addresses.
- **Hub:** Broadcasts data to all connected devices (outdated).
- **Access Point:** Allows wireless devices to connect to a wired network.
- **Modem:** Converts digital data to analog for transmission over telephone lines (and vice versa).

### 14. **Common Network Tools**
- **Ping:** Tests reachability and measures round-trip time.
- **Traceroute:** Shows the path packets take to reach a destination.
- **Netstat:** Displays network connections, routing tables, interface statistics.
- **Wireshark:** Network protocol analyzer to capture and inspect packet data.

### 15. **Network Topologies**
- **Bus:** Single central cable with all devices connected.
- **Star:** Devices connected to a central hub or switch.
- **Ring:** Each device connected to two other devices, forming a ring.
- **Mesh:** Devices are interconnected; provides redundancy.
- **Hybrid:** Combination of multiple topologies (e.g., Star-Bus).

### 16. **Network Cable Types**
- **Twisted Pair (UTP/STP):** Copper wires twisted together; used in Ethernet.
  - **Category 5e (Cat5e):** Up to 1 Gbps.
  - **Category 6 (Cat6):** Up to 10 Gbps (short distances).
- **Coaxial:** Used in older cable networks.
- **Fiber Optic:** High-speed data transmission using light.

This cheat sheet covers core concepts and tools in computer networks that will help with both academic and practical understanding of the field!
