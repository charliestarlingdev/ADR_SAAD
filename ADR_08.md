# ADR-08: Centralise Complaint Lifecycle Rules in the Domain

## Status: *Accepted*

### Context
Complaint statuses must follow defined rules to prevent invalid or inconsistent transitions.

### Decision
I implemented lifecycle rules within a dedicated domain component.

### Consequences
+ This keeps business rules centralised and consistent.
+ It makes the system easier to test and reason about.

- If not carefully managed, the domain layer could become overly complex.
