# 11. Application internal communication specs


## Status
accepted


## Context
Components within the application will need to communicate with one another. 

This communication can be synchronous or asynchronous (based on component function).


## Decision

### Design decision
All communication to Sales and Purchase service will be synchronous. All other communications will be asynchronous.

### Design Justification
Synchronous communication shall be used to preserve data integrity and avoid split brain scenario
Asynchronous communication shall be used to ensure speed and agility of the data communication


## Consequences
Payment system communication may have negligible lag
