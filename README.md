# Site-to-Site VPN Lab

## Project Overview

This project demonstrates the design, configuration, validation, and troubleshooting of an IPsec site-to-site VPN between two isolated private networks.

The lab uses Hyper-V to create a virtual network environment and pfSense as the VPN endpoints. The goal is to establish secure communication between Site A and Site B while gaining hands-on experience with IPsec, routing, firewall rules, and VPN troubleshooting.

## Objectives

- Build two isolated private networks in Hyper-V
- Configure pfSense as the VPN gateway for each site
- Configure an IPsec site-to-site VPN
- Verify secure connectivity between the two sites
- Validate VPN status and IPsec security associations
- Perform and document a VPN troubleshooting scenario
- Document the completed architecture and configuration

## Technologies

- Microsoft Hyper-V
- pfSense
- IPsec
- IKE
- TCP/IP
- Virtual Networking

## Network Architecture

![Site-to-Site VPN Architecture](Site-to-Site%20VPN%20Architecture.png)

| Site | Interface | IP Address / Network |
|------|-----------|----------------------|
| Site A | WAN | 172.16.100.10/24 |
| Site A | LAN | 10.10.10.1/24 |
| Site A | LAN Network | 10.10.10.0/24 |
| Site B | WAN | 172.16.100.20/24 |
| Site B | LAN | 10.20.20.1/24 |
| Site B | LAN Network | 10.20.20.0/24 |
| Transit Network | WAN | 172.16.100.0/24 |

## Project Status

**Status:** In Progress
