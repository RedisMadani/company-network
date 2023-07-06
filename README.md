# HTL Shkodra 22/23 NWTK 4 Project Description

![network](https://github.com/RedisMadani/company-network/assets/136177376/6479bac7-d08a-4c7f-a1cc-413a362920c2)

This repository contains the project files for the HTL Shkodra 22/23 NWTK 4 Project, which focuses on building an advanced company network using PacketTracer. The project involves setting up an extensive network infrastructure with multiple locations and various networking elements.

## Project Objectives

1. Standort 1: 
   - Implement subnetting/VLSM with the network range 10.<KN>.<T>.0/21.
   - Design a hierarchical LAN architecture using Access, Distribution, and Core layers. Utilize the Switch 3650 for this purpose.
   - Configure redundant connections between switches using Link-EtherChannel with LACP.
   - Assign appropriate VLANs (Admins, Management, Native, Raum1 to Raum4) and distribute them effectively using VTP.
   - Connect and configure at least two hosts in each VLAN on the Access layer switches.
   - Implement Port Security, PortFast, BPDUGuard, RootGuard, and UplinkFast features on the Access switches.
   - Enable routing on the switches in the Core layer.
   - Set up DHCP for one VLAN (excluding Management-VLAN).
   - Connect a router to the Core switches (using RIPv2) to establish a connection to the "Internet" router via PAT. The router will also act as a DHCP server.
   - Apply Zone-based Policy Firewall (ZPF) to protect Standort 1. Only clients from Standort 1 will be allowed internet access, while all incoming requests from the internet will be blocked.
   - Limit VTY-line access to only the Admins network for configuring switches and routers from Standort 1.

2. Standort 2:
   - Assign the network range 200.<GM>.<GT>.0/24.
   - Set up an email server, a switch, a router (4331), and two hosts.
   - Configure redundant gateways, with the last IP address as the standard gateway for the hosts.

3. Standort 3:
   - Assign the network range 172.16.<GT+GM>.0/24.
   - Set up a web server, a router with static NAT for ports 80 and 443, and a DNS server (www.[VornameNachname].al).
   - Allow access only to HTTP, HTTPS, and DNS services using Extended Access Control Lists (ACLs).

4. "Internet":
   - Implement subnetting/VLSM with the network range <KN>.<GM>.<GT>.0/23.
   - Connect routers to establish connectivity between different locations.
   - Configure a loopback interface on one of the routers.

5. General:
   - Assign the last available host IP address to all router interfaces and SVIs.
   - Assign ascending IP addresses to all hosts and switch management interfaces.
   - Utilize OSPF for routing in the "Internet" network.
   - Use static default routes or RIPv2 for routing in other locations as required.
   - Ensure all switches and routers have basic configurations including hostname, password settings, enable password encryption, banners, disabling domain lookup, enabling SSH access, and encrypting all passwords.

## Project Structure

The project is divided into five parts:

1. Overview Plan (Sketch): Create a clear hand-drawn plan showcasing devices, VLANs, and IP networks.
2. Setup and Configuration in Packet Tracer: Standort 1. This part includes IP addressing, access/trunk ports, VTP, and STP.
3. Configuration of Standort 1: Configure SVIs, routing, DHCP, PAT, and LACP.
4. Setup and Configuration of Remaining Locations + Internet + Testing.
5. Switch/Router Password and SSH Configuration + Documentation.

Please refer to the provided PDF document for detailed documentation, including IP address plans, interface configurations, protocol configurations, and overall project explanations.

Note: This project is designed for educational purposes as part of the HTL Shkodra NWTK 4 curriculum and does not represent an actual company network.
