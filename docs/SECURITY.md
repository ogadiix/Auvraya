# Security and Privacy Checklist

## Before implementation
- [ ] Identify personal data collected and why.
- [ ] Define consent, retention, export, and deletion behavior.
- [ ] Define threat model and trust boundaries.
- [ ] Confirm environment separation for local, staging, and production.
- [ ] Confirm applicable app-store and privacy requirements.

## Implementation controls
- [ ] No secrets in source control, mobile bundles, logs, or client-visible configuration.
- [ ] Server-side authorization for every protected operation.
- [ ] Least privilege and row-level access controls where supported.
- [ ] Input validation, output encoding, rate limiting, and abuse protections.
- [ ] Secure token/session storage and expiry behavior.
- [ ] Dependency review and supported versions.
- [ ] Safe logging; avoid unnecessary sensitive data.
- [ ] Account deletion and associated data deletion workflow.
- [ ] Backups, recovery, and migration safety reviewed.
- [ ] AI prompts, retrieved content, and model outputs treated as untrusted input.
- [ ] No medical diagnosis, prescription, or unsupported cure claims.
- [ ] Audit log for CMS publication and safety-rule changes.

## Release gate
Do not release while critical/high-risk findings remain unresolved. Document accepted residual risks and obtain explicit approval before production deployment.
