
**Idea:** Have a central proxy and load balancer (that can themselves be distributed) that routes different requests to the different (micro)services. The goal is to focus each Backend task in a specialized service, and have it all managed by a central service (proxy).
