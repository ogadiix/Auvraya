# Backend Rules

- Inspect existing backend before adding services or tables.
- Validate every input and enforce authorization on the server.
- Apply least privilege and row-level access controls where supported.
- Keep privileged keys and AI provider keys server-side.
- Version database migrations and remote content schemas.
- Add rate limits, safe errors, and audit events for privileged CMS changes.
- Do not let AI bypass deterministic safety rules or publish content without review.
