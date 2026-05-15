# LUMINARA Network Design – Cisco Packet Tracer Project

## Overview
This project is a complete Cisco Packet Tracer network implementation for **The Crystal Realm of LUMINARA**. It connects six different LANs using routers, switches, VLSM subnetting, RIP v2, static routing, DHCP relay, DNS, Web, and Email services.

## Project Goals
- Design a scalable multi-site network using VLSM.
- Connect six LANs through routed WAN links.
- Configure RIP v2 and static/floating static routes.
- Configure DHCP for remote LANs using DHCP relay.
- Configure DNS, Web Server, and Email Server.
- Verify full connectivity using ping and Packet Tracer Simulation mode.

## Base Network
Student ID: `22201501`  
Last four digits: `1501`  
Base network: `15.1.0.0/16`

## LAN Subnet Plan

| Location | Subnet | Subnet Mask | Gateway |
|---|---|---|---|
| Granite Borough | 15.1.0.0/19 | 255.255.224.0 | 15.1.0.1 |
| Corsair Isles | 15.1.32.0/21 | 255.255.248.0 | 15.1.32.1 |
| Frostfield Ranch | 15.1.40.0/23 | 255.255.254.0 | 15.1.40.1 |
| Aurora Ridge | 15.1.42.0/24 | 255.255.255.0 | 15.1.42.1 |
| Photon Cove | 15.1.43.0/25 | 255.255.255.128 | 15.1.43.1 |
| Sunspire Palace | 15.1.43.128/26 | 255.255.255.192 | 15.1.43.129 |

## Server IP Addresses

| Server | IP Address | Purpose |
|---|---|---|
| Web Server | 15.1.43.10 | Hosts www.luminara.net |
| DNS Server | 15.1.43.11 | Resolves domain names |
| Email Server | 15.1.43.12 | Handles email service |
| DHCP Server | 15.1.43.13 | Assigns IPs to remote LANs |

## Key Features
- VLSM subnetting
- RIP v2 dynamic routing
- Static and floating static routing
- DHCP relay using `ip helper-address`
- DNS records for web and mail services
- Web service at `www.luminara.net`
- Email service using `luminara.net`
- Full LAN-to-LAN connectivity verification

## Testing and Verification
The project was verified using:
- Successful ping between remote LANs
- DHCP address assignment in Frostfield Ranch and Aurora Ridge
- Web access to `www.luminara.net`
- Email sent from `sun@luminara.net` to `granite@luminara.net`
- Packet path observation using Cisco Packet Tracer Simulation mode

## Tools Used
- Cisco Packet Tracer
- RIP v2
- Static Routing
- DHCP, DNS, HTTP, SMTP, POP3

## Files Included
- `.pkt` Packet Tracer project file
- Final PDF report
- Verification screenshots