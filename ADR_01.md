# ADR-01: Adopt a Multi-Tenant Architecture

## Status: *Accepted*

### Context
From the start, the CMS was intended to be used by multiple organisations rather than built as a single-company system. This meant that the system needed to support shared infrastructure while still keeping each organisation's data and users separate (separate environments of context). 

### Decision
A multi-tenant architecture was chosen, where all organisations use the same system but operate within their own tenant context. 

### Consequences
+ This approach seems easier to scale on the surface and avoids duplicating infrastructure for each tenant.

- However, it also means that tenant context needs to be handled carefully throughout the system to retain data privacy across different organisations. 