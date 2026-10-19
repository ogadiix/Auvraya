# Test Plan

Update this plan as the architecture and implementation become known.

## Each task
- [ ] Format code using the project's standard formatter.
- [ ] Run static analysis/lint/type checks available for changed code.
- [ ] Run relevant unit tests.
- [ ] Run integration tests for affected boundaries.
- [ ] Run app/web build where applicable.
- [ ] Inspect logs and failure output.
- [ ] Inspect Git diff and status.

## Product test areas
- English/Hindi switching and missing translation fallback
- Authentication, session expiry, authorization, and account deletion
- CMS draft/review/publish/archive and rollback
- Content schema validation and version compatibility
- Assessment scoring edge cases, mixed/uncertain outcomes, and versioning
- Recommendation explanation and safety-rule enforcement
- Offline, stale cache, timeout, provider failure, and retry behavior
- Accessibility, font scaling, screen reader labels, contrast, and touch targets
- Privacy consent, data minimization, retention, and deletion
- Security: access control, secrets, input validation, rate limiting, dependency checks
- Android release build and representative device testing

Do not mark tests as passed unless they were actually executed successfully.
