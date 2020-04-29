# Static Routing and Dynamic Routing for Private IP
comparison between them

* Router:

![r](https://camo.githubusercontent.com/416623c866865f8b8d0faebe8793da71271df2cd/68747470733a2f2f73636f6e74656e742e66747065382d322e666e612e666263646e2e6e65742f762f74312e302d392f39353232343138325f343233363838363238323939313831345f333238343432333930313432303937383137365f6f2e706e673f5f6e635f6361743d313031265f6e635f7369643d313130343734265f6e635f6f68633d41316c544d44703632686b4158384172584b68265f6e635f68743d73636f6e74656e742e66747065382d322e666e61266f683d6237653861363230613561393034386635316331373333366665646131636436266f653d3545434430394335)

# Static

https://github.com/QueenieCplusplus/Static_Routing

![static](https://scontent.ftpe8-2.fna.fbcdn.net/v/t1.0-9/95553683_4236886296325146_7089570363658469376_o.png?_nc_cat=101&_nc_sid=110474&_nc_ohc=avBRyMZq-mwAX-8ZPsI&_nc_ht=scontent.ftpe8-2.fna&oh=335968e6bfdf6b46cd125e456424ce6c&oe=5ED06155)

Static Routes are config on a router. They don't react to network outages. 

The one exception is when the static route specifies the outbound interface: If the interface goes down, the static route is removed from the routing table.

Because static routes are unidirectional, they must be configed for each outging interface the router will use.

the benefit of Static Routing Protocol is that a router generates no routing protocol overheads, due to no bandwidth consumption for advertisements between network devices (Router-Router or Router-SW).

# Suitable Circumstance (Hub & Spoke Mode) for Statics

軸輻式設計

it is recommended for a hub-and-spoke topology with low-speed remote connection. A default static route is configed at each remote side because the hub is the only route used to each other sites.

![hub and spoke](https://transportgeography.org/wp-content/uploads/2017/10/point_hub_network.png)

Point-to-point and hub-and-spoke networks are at the opposite ends of the connectivity spectrum. A point-to-point network connects directly a set of locations without any interruption of services (e.g. pick up or drop off) even if the route itself may not be direct.

A (pure) hub-and-spoke network connects every location through a single intermediary location called a hub. Hub-and-spoke, as a network structure, allows for greater flexibility within the transport system through a concentration of flows.

On the above figure, a point-to-point network involves 16 independent connections, each to be serviced by vehicles and infrastructures. By using a hub-and-spoke structure, only 8 connections are required. 

# Dynamic (Routing Protocols)

However the size of today's network makes it impossible to manually config and maintain all he routes in all the routers in a timely manner.

But human config can involve many mistakes, which is why dynamic routing protocol exists.

They use algorithm to advertise and learn about changes in the network topology.

Dynamic Routing Protocols:

RIP (Interior, distance vetor) https://github.com/QueenieCplusplus/RIP

IGRP (Interior, distance vector)

EIGRP (Interior, distance vector)

OSPF (Interior, LSA) https://github.com/QueenieCplusplus/OSPF

IS-IS (Interior, LSA) https://github.com/QueenieCplusplus/IS_IS

BGP (Exterior) https://github.com/QueenieCplusplus/BGP

EGP (Exterior)





















