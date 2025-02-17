# Cisco Packet Tracer Lab - Configuring Static Routes

## Description
This lab is a network simulation created in **Cisco Packet Tracer**, focusing on configuring static routes on routers to enable end-to-end communication between PCs. The topology includes multiple routers and subnets that require manual route configuration.

### Devices Used:
- **Cisco 2911 Routers** (R1, R2)
- **Cisco 2960 Switches** (SW1, SW2)
- **PCs** (PC1, PC2)

### Network Structure:
- **Subnet 1:** 192.168.1.0/24 (PC1 and SW1)
- **Subnet 2:** 192.168.12.0/24 (Link between R1 and R2)
- **Subnet 3:** 192.168.13.0/24 (R2 interface connection)
- **Subnet 4:** 192.168.3.0/24 (PC2 and SW2)

## Objectives
- Configure the **hostname** of R1 and R2.
- Assign and configure the **correct IPv4 addresses** on all router interfaces.
- Enable the interfaces and set **interface descriptions**.
- Configure **static routes** on both routers to ensure full network connectivity.
- Assign **IP addresses** and **default gateways** to PC1 and PC2.
- Test network connectivity using **ping** between PCs.

## Setup Instructions
1. Open the **.pkt** file in Cisco Packet Tracer.
2. Configure the **hostname** for both routers (R1 and R2).
3. Assign the correct **IPv4 addresses** to all interfaces as per the network topology.
4. Use `no shutdown` to enable each interface.
5. Verify the interface configuration using `show ip interface brief`.
6. Configure **static routes** on R1 and R2:
   - On R1, add a static route to reach 192.168.3.0/24 via R2.
   - On R2, add a static route to reach 192.168.1.0/24 via R1.
7. Configure the **default gateway** on PC1 and PC2.
8. Test connectivity by **pinging PC2 from PC1**.

## Screenshot
![Network Topology](/mnt/data/image.png)

## Notes
- Ensure that each PC’s **gateway is set correctly**.
- If pings fail, check **route configurations and subnet masks**.
- Use `show ip route` to verify static routes.

## Author
Created for educational purposes in **Cisco Networking Labs**.

