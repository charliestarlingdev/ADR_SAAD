# ADR-02: Delegate Authentication to Tenant Systems

## Status: *Accepted*

### Context
I understood that handling user credentials within the CMS would increase risk, complexity, scalability issues and would demand more resources. However, I couldn't find a way to get around these issues. 

### Decision
After spending some time talking with my lecturers, I decided to opt for authenticating the CMS users through the tenant's core system. 

The case study from ABC Ltd explained that the CMS was part of organisations' HelpDesk application, and therefore we could use their login systems to not only set the system context but also ensure user authentication without taking the responsibilty and demand for resources. 

### Consequences
+ Reduction in security risk, and a scalable way of onboarding new tenants. Low cost on resources  therefore, keeping performance high, with an established way of getting and setting system context for the CMS.

+ However, introduces a reliance on external systems for user authentication but if one company loses their login services, atleast other tenants can still utilise the CMS. 
