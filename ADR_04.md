# ADR-04: Implement Role-Based Access Control (RBAC)

## Status: *Accepted*

### Context
The CMS supports several different user roles, each with very different responsibilities. Without a clear access control strategy, there was a risk that users could access data or actions they should not be allowed to.

### Decision
I decided to implement role-based access control, where permissions are defined by both the user’s role and their tenant.

### Consequences
+ This makes permissions much clearer and easier to reason about across the system.
+ It improves security by ensuring users only see and perform actions relevant to their role.

- The downside is that permission checks must be applied consistently across services, which adds complexity if not carefully managed.
