# 6. Use of Document Database for services that could have changing schemas


## Status
accepted


## Context
Startups require new features leading to a situation where the schema cannot be decided upon upfront or where the schema could require a change. Further, the database will need to scale as per demand as well as handle variety of data like images, new types of health information, device and appliance information etc.

We could use relational, document or column based database


## Decision

### Design decision
We will use Document Database for the Diet Advisor service, User Interface service and Fridge Communicator service

### Design Justification
Enables new types of diet suggestions by letting flexibility of schema


## Consequences
Considerable effort will need to be expended to ensure a good, static aggregate design
