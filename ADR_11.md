# ADR-11: Use the Repository Pattern for Data Access

## Status: *Accepted*

### Context
Direct database access within business logic tightly couples the system to persistence details.

### Decision
I used repositories to abstract data access.

### Consequences
+ Improves testability and separation of concerns.
+ Allows database changes with minimal impact.

- Introduces additional abstraction and some boilerplate code.
