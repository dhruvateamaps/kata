# 8. Database containing personal and financial information to be secured


## Status
accepted


## Context
Laws about personal data are getting stringent by the day. Users are also wary of organisations that don't take personal data privacy seriously. Non conformance to these legal and social requirements can lead to failure of the business idea.
Security incidents are also on the rise - with data breaches leading to loss of reputation and lawsuits.

We could limit collection of sensitive data leading to no requirement of securing, or we could collect the data and secure it


## Decision

### Design decision
We will use secured database

### Design Justification
Customer service and Sales and Purchase service are holding sensitive information. Access to the data within these servcies has to be secured to ensure confoirmance with laws and social requirements.


## Consequences
Additional administrative and operational overheads. We might experience a marginal adverse impact on the performance.
