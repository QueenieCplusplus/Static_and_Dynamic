# Static_and_Dynamic
comparison between them

# Static 

Static Routes are config on a router. They don't react to network outages. 

The one exception is when the static route specifies the outbound interface: If the interface goes down, the static route is removed from the routing table.

Because static routes are unidirectional, they must be configed for each outging interface the router will use.

the benefit of Static Routing Protocol is that a router generates no routing protocol overheads, due to no bandwidth consumption for advertisements between network devices (Router-Router or Router-SW).

# Suitable Circumstance (Hub) for Statics

it is recommended for a hub-and-spoke topology with low-speed remote connection. A default static route is configed at each remote side because the hub is the only route used to each other sites.

![hub and spoke](https://www.researchgate.net/publication/297600508/figure/fig2/AS:337841608511489@1457559124395/Point-to-Point-vs-Hub-and-Spoke-Systems.png)

# Dynamic (Routing Protocols)

However the size of today's network makes it impossible to manually config and maintain all he routes in all the routers in a timely manner.

But human config can involve many mistakes, which is why dynamic routing protocol exists.

They use algorithm to advertise and learn about changes in the network topology.




