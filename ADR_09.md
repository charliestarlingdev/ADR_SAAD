# ADR-09: Keep the API Layer Lightweight

## Status: *Accepted*

### Context
Placing business logic directly in controllers can lead to poor separation of concerns.

### Decision
I restricted the API layer to request handling and delegation.

### Consequences
+ Controllers remain clean and readable.
+ Business logic is easier to test.

- This places more responsibility on the service layer design.
