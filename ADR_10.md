# ADR-10: Use a Service Layer for Coordination

## Status: *Accepted*

### Context
Handling complaints requires coordination between permissions, domain logic, and persistence.

### Decision
I introduced a central service to coordinate complaint-related operations.

### Consequences
+ This makes request flows easier to understand.
+ It reduces duplicated logic.

- There is a risk of the service becoming too large if not controlled.
