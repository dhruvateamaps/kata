# 12. Application internal communication message specs


## Status
accepted


## Context
Components within the application will need to communicate with one another. 

This communication could utilise point to point queues or pub/sub messaging systems.


## Decision

### Design decision
The inventory system will uitilise a pub/sub messaging to get inventory data from the network of fridges.
Sales and purchase system will utilise a point-to-point queue to communicate with the network of fridges.

### Design Justification
Inventory system can utilise a pub/sub messaging as it does not have synchronous communication.
Sales and Purchase system has synchronous communication requirement, thus it will utilise a point to point queue to communicate with the fridge.


## Consequences
There will be additional administrative overheads of multiple queues
