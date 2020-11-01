# 5. Use of Column-Family store for services that log events


## Status
accepted


## Context
Analysis of events typically requires related data about the event to be accessed together, for example, information about the event like time of the event, application impacted, feature impacted, user impacted etc.
We could utilise file stores. Or we could use any one of relational, document or column based database


## Decision

### Design decision
We will use column family stores for the Monitoring service and the centralized logging service

### Design Justification
Column family stores ease access to related data as an aggregate.


## Consequences
Column family stores will have a higher latency while trying to update existing rows
