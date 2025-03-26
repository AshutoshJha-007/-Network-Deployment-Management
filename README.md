# ISP Network Deployment & Management

## Overview
This project documents the setup and management of a high-speed **ISP network infrastructure**, covering **OLT, ONU, Ethernet, TCP/IP, Fiber Optic, Routers, and Switches** for seamless broadband service.

## Features
- **High-Speed ISP Network:** Designed and deployed for residential and commercial users.
- **OLT & ONU Deployment:** Configured Fiber Optic connectivity for last-mile distribution.
- **Router & Switch Configuration:** Optimized traffic flow, VLAN segmentation, and firewall rules.
- **Fiber Optic & Ethernet Deployment:** Ensured reliable and scalable data transmission.
- **TCP/IP Network Design:** Implemented subnetting, DHCP, and DNS services for efficient connectivity.
- **Network Monitoring & Troubleshooting:** Utilized Wireshark, Ping, and Traceroute to diagnose issues.

## Network Architecture
```
[Internet] → [OLT] → [ONU] → [Main Router] → [Core Switch] → [Access Switches] → [End Users]
```
- **OLT (Optical Line Terminal):** Distributes fiber connections to multiple ONUs.
- **ONU (Optical Network Unit):** Converts fiber optic signals for end-user connectivity.
- **Main Router:** Handles WAN connectivity and firewall configurations.
- **Core Switch:** Manages VLANs and high-speed internal routing.
- **Access Switches:** Distributes connections to customers.
- **DHCP & DNS Servers:** Automate IP address allocation and domain resolution.

## Tools & Technologies
- **Networking:** TCP/IP, Ethernet, VLAN, DHCP, DNS
- **Fiber Infrastructure:** OLT, ONU, Fiber Optic Cables
- **Hardware:** Routers, Managed Switches
- **Security:** Firewall Rules, VLAN Segmentation, Access Control Lists
- **Troubleshooting:** Wireshark, Ping, Traceroute

## Deployment Steps
1. **Setup OLT & ONU** for fiber network distribution.
2. **Configure Main Router** with WAN settings and security policies.
3. **Install and configure Core Switch** for VLANs and internal routing.
4. **Deploy Access Switches** for distribution to end users.
5. **Lay Fiber Optic & Ethernet Cabling** for high-speed data transmission.
6. **Configure DHCP and DNS Servers** for seamless connectivity.
7. **Monitor and troubleshoot network** using diagnostic tools.

## Project Files
- **network_topology.png** - Diagram of the network architecture.
- **router_config.txt** - Sample router configuration file.
- **switch_config.txt** - Sample switch configuration file.
- **dhcp_dns_setup.sh** - Script for setting up DHCP and DNS servers.
- **troubleshooting_guide.md** - Common network issues and resolutions.

## Future Enhancements
- Implement **BGP routing** for better traffic control.
- Set up **redundant network paths** for improved uptime.

---
**Maintained by:** [Ashutosh Kumar Jha](https://github.com/AshutoshJha-007)
