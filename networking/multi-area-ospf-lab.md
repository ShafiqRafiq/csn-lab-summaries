# Multi-Area OSPF Lab

This lab shows a multi-area OSPFv2 setup built in Cisco Packet Tracer. I configured three routers across different OSPF areas, assigned router IDs, set passive interfaces where needed, and verified that neighbor relationships and routing were working properly.

## Topology overview

The topology uses three routers connected across multiple OSPF areas.

- **R1** connects Area 1 to Area 0
- **R2** connects Area 0 to Area 3
- **R3** is an internal router in Area 3

This lab helped me understand how OSPF works in a bigger network and not just in a basic single-area setup.

![Topology](./ospf-topology.png)

## What I did

First, I configured the IP addresses on the router interfaces and made sure the interfaces were up and working properly.

**[Insert Screenshot 2 here – show ip interface brief]**

After that, I tested connectivity between the routers to make sure basic Layer 3 communication was working before focusing on OSPF.

**[Insert Screenshot 3 here – Ping verification]**

Then I enabled OSPFv2 on all routers, assigned the correct areas, and configured the loopback interfaces as passive where needed.

**[Insert Screenshot 4 here – show ip protocols]**

Once OSPF was configured, I checked the neighbor adjacencies to make sure the routers were forming OSPF relationships properly.

**[Insert Screenshot 5 here – show ip ospf neighbor]**

I also verified the OSPF interface details like the area, timer values, cost, and network type.

**[Insert Screenshot 6 here – show ip ospf interface]**

## Key concepts shown

- multi-area OSPFv2
- router IDs
- passive interfaces
- OSPF neighbor adjacencies
- OSPF verification
- interface cost and timers
- routing between areas

## Commands used

```bash
show ip interface brief
show ip protocols
show ip ospf neighbor
show ip ospf interface
ping
