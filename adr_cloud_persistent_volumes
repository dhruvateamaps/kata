# 4. Use of persistent volumes on public cloud storage


## Status
accepted


## Context
Containers by nature are ephemereal. But data needs to persist beyond the lifecycle of the container.
This persistence could be accomplished through NFS shares or persistent volume provided by the cloud provider


## Decision



### Design decision
We will be using cloud provided persistent disks


### Design Justification
Cloud provided persistent disks have the added benefit of APIs that can utilised to create, request access as well as use through the entire container lifecyle.


## Consequences
Difficult to later switch back to an NFS based volumes
