# Static_and_Dynamic
comparison between them

Static Routes are config on a router. They don't react to network outages. 

The one exception is when the static route specifies the outbound interface: If the interface goes down, the static route is removed from the routing table.

Because static routes are unidirectional, they must be configed for each outging interface the router will use.



