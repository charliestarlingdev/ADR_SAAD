# ADR-03: Using a Separate Database Per Tenant

## Status: *Rejected*

### Context
With each tenant bringing their own consumers, staff and complaints, I thought it would be a good start to give each tenant their own database. However, after careful review, I decided not to go through with this decision.

### Decision
I originally decided to appoint each tenant their own database to handle their information in isolation from one another. Later, I came back to this decision and rejected it. 

### Consequences
+ Isolation is maintained as data would be stored entirely spearate from other tenants using the CMS.

+ As a business point of view, ABC Ltd can better monitor and charge accordingly to tenants that are scaling up in terms of users and complaints (needing a larger database).

+ However, the cost on resources and complexity involved in setting up the system would prove difficult, add to that, it would be inefficient for the system to connect to multiple different databases at any single time without having an impact on performance (bad for scaling). 

