# ADR-05: Use an API-First Design

## Status: *Accepted*

### Context
The CMS needed to support a web interface and potentially other clients in the future. Tight coupling between frontend and backend would limit flexibility.

### Decision
I decided to design the CMS using an API-first approach, exposing all functionality through RESTful APIs.

### Consequences
+ This allows the frontend and backend to evolve independently.
+ It supports future integrations and improves testability.

- The trade-off is the extra effort required upfront to design and document stable APIs.
