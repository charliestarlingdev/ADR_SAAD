# ADR-06: Introduce an API Gateway

## Status: *Accepted*

### Context
While designing the container model, I noticed that routing and authentication checks were being repeated across services.

### Decision
I introduced an API Gateway to act as a single entry point into the CMS.

### Consequences
+ This centralises common concerns such as routing and security checks.
+ It results in cleaner and simpler downstream services.

- However, it introduces an additional component that must be monitored and maintained.
