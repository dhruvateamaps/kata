# 10. Use of global load balancer


## Status
accepted


## Context
Farmacy foods is targetting to expand across geographies soon.

We could forego the use of a global load balancer and establish a direct interface between user access point and internal services. We could use a global load balancer that interfaces between user access points and internal services.


## Decision

### Design decision
We will use a global load balancer

### Design Justification
Adding a global load balancer would help adhere to the scalability needs of the business.


## Consequences
Additional configurations will be required, charges will be incurred for the use of global load balancer
