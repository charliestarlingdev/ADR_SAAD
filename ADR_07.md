# ADR-07: Separate Notification Handling from Core Logic

## Status: *Accepted*

### Context
The CMS needs to notify users when complaint statuses change, but notification delivery is not part of the system’s core responsibility.

### Decision
I decided to separate notification handling into a dedicated service.

### Consequences
+ This keeps the complaint service focused on its main purpose.
+ Notification mechanisms can be changed or extended without impacting core logic.

- It introduces asynchronous behaviour, which requires additional handling for failures and retries.
