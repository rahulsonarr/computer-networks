### **Computer Networks Cheat Sheet**

#### **1. OSI Model (7 Layers)**
- **Application (Layer 7):** User interface, provides network services to end-users. (HTTP, FTP, DNS)
- **Presentation (Layer 6):** Data format translation, encryption, and compression. (SSL, JPEG, ASCII)
- **Session (Layer 5):** Manages sessions between applications, establishing, maintaining, and terminating sessions. (RPC, PPTP)
- **Transport (Layer 4):** Ensures end-to-end communication, error handling, and flow control. (TCP, UDP)
- **Network (Layer 3):** Routing of data between devices, logical addressing. (IP, ICMP, ARP)
- **Data Link (Layer 2):** Physical addressing (MAC), error detection. Divided into MAC & LLC. (Ethernet, PPP)
- **Physical (Layer 1):** Transmission of raw bits over the physical medium (cables, radio frequencies). (Ethernet cables, Wi-Fi)

#### **2. TCP/IP Model (4 Layers)**
- **Application (Layer 4):** Combines OSI Application, Presentation, and Session layers. (HTTP, FTP, DNS)
- **Transport (Layer 3):** Reliable data transmission and flow control. (TCP, UDP)
- **Internet (Layer 2):** Logical addressing and routing of packets. (IP, ICMP)
- **Network Interface (Layer 1):** Physical connection and data link protocols. (Ethernet, Wi-Fi)

#### **3. Protocols Overview**
- **HTTP/HTTPS:** HyperText Transfer Protocol (Secure) for web traffic.
- **FTP:** File Transfer Protocol for transferring files between systems.
- **DNS:** Domain Name System, resolves domain names to IP addresses.
- **SMTP:** Simple Mail Transfer Protocol, used for sending emails.
- **TCP (Transmission Control Protocol):** Connection-oriented, reliable transmission (acknowledgment, retransmission).
- **UDP (User Datagram Protocol):** Connectionless, fast, but unreliable (used in streaming, VoIP).

#### **4. IP Addressing**
- **IPv4 Addressing:** 32-bit address (e.g., 192.168.1.1), divided into classes (A, B, C, D, E).
  - **Private IPs:** 192.168.x.x, 10.x.x.x, 172.16.x.x-172.31.x.x
  - **Loopback:** 127.0.0.1 (Local host testing)
- **IPv6 Addressing:** 128-bit address (e.g., 2001:0db8:85a3::8a2e:0370:7334), solving address exhaustion.

#### **5. Subnetting**
- **Subnet Mask:** Defines network and host portions of an IP address.
  - **Common Subnets:** 
    - Class A: 255.0.0.0
    - Class B: 255.255.0.0
    - Class C: 255.255.255.0
- **CIDR (Classless Inter-Domain Routing):** /x notation for subnetting, e.g., /24 means 255.255.255.0

#### **6. Key Network Devices**
- **Router:** Routes data between different networks, works at Layer 3 (Network).
- **Switch:** Connects devices within the same network, works at Layer 2 (Data Link).
- **Hub:** Basic networking device, broadcasts data to all devices.
- **Firewall:** Monitors and controls incoming/outgoing network traffic based on security rules.
- **Modem:** Modulates/demodulates signals between digital devices and analog transmission lines.

#### **7. Network Topologies**
- **Bus:** Single central cable; easy but failure-prone.
- **Star:** Devices connect to a central hub; scalable and fault-tolerant.
- **Mesh:** Devices interconnect with many redundant paths; high reliability but costly.
- **Ring:** Devices form a ring; failure of one device affects the whole network unless dual-ring.

#### **8. Ethernet Standards**
- **Ethernet (802.3):** Standard for wired LAN (10 Mbps to 100 Gbps).
- **Fast Ethernet:** 100 Mbps.
- **Gigabit Ethernet:** 1 Gbps.
- **10G Ethernet:** 10 Gbps, used in high-performance networking.

#### **9. Wireless Networks (Wi-Fi)**
- **802.11 a/b/g/n/ac/ax:** Wi-Fi standards, ranging from 2.4 GHz to 5 GHz, speeds from 11 Mbps (802.11b) to several Gbps (802.11ax or Wi-Fi 6).
- **SSID:** Service Set Identifier, the name of a Wi-Fi network.
- **WPA/WPA2/WPA3:** Wi-Fi security protocols, WPA3 being the most secure.

#### **10. Network Security Concepts**
- **Encryption:** Process of encoding data for confidentiality (e.g., TLS, SSL).
- **Firewalls:** Devices or software to block unauthorized access while permitting outward communication.
- **VPN (Virtual Private Network):** Encrypts internet traffic, providing privacy and secure connections.
- **Intrusion Detection System (IDS):** Monitors network traffic for suspicious activity.
- **Intrusion Prevention System (IPS):** Detects and blocks malicious activity.

#### **11. Common Network Commands**
- **ping:** Tests connectivity by sending ICMP echo requests.
- **tracert (Windows) / traceroute (Linux):** Shows the path packets take to reach a destination.
- **ipconfig (Windows) / ifconfig (Linux):** Displays IP configuration settings.
- **netstat:** Displays active network connections and listening ports.
- **nslookup:** Queries DNS servers for domain name resolution.
- **telnet:** Tests connectivity to remote systems, not secure.
- **ssh:** Secure alternative to telnet, for encrypted remote access.

#### **12. Network Address Translation (NAT)**
- **Purpose:** Translates private IP addresses to public IPs for internet access.
  - **Static NAT:** One-to-one mapping between private and public IPs.
  - **Dynamic NAT:** Private IPs mapped to a pool of public IPs.
  - **PAT (Port Address Translation):** Multiple private IPs mapped to a single public IP with different ports.

#### **13. Network Architectures**
- **Client-Server Model:** Central server provides resources/services to multiple clients.
- **Peer-to-Peer (P2P):** Each device acts as both client and server, sharing resources directly.

#### **14. Network Troubleshooting Steps**
1. **Check physical connections:** Ensure cables, ports, and devices are functioning.
2. **Check IP configuration:** Validate IP address, subnet mask, default gateway.
3. **ping test:** Test connectivity to local network and external network.
4. **tracert/traceroute:** Trace the path packets take to their destination.
5. **DNS issues:** Use `nslookup` to check DNS resolution.
6. **Check firewall and security settings.**

---

This sheet gives an overview of essential concepts in computer networks, which can serve as a quick reference for network protocols, models, devices, and troubleshooting tips.
