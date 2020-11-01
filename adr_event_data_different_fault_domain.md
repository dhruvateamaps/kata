# 7. Monitoring and logging data should be stored outside the overall solution


## Status
accepted


## Context
Failure of infrastruture cannot be predicted or controlled. Upon failure, data about the fialure is critical for investigation and analysis. If data about the failure is stored on the same failed system, then this critical data is lost.

We could either store data in the same fault domain or on a different fault domain


## Decision

### Design decision
We will store monitoring and logging data in a different fault domain

### Design Justification
Failure of system should not impact ability to investigate, troubleshoot and diagnose the failure, thus data about the failure should be in a different fault domain


## Consequences
Additional infrastructure will need to be setup on a different fault domain
