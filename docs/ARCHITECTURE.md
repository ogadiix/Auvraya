# Architecture — Proposed, Not Yet Implemented

## Principles
- Inspect existing repository before choosing or changing architecture.
- Separate Flutter presentation, domain logic, and data access.
- Keep mutable content and rules server/CMS-managed; keep stable rendering and security infrastructure in the client.
- Use documented APIs and versioned schemas.
- Make offline behavior and failure states explicit.

## Candidate stack
- Mobile: Flutter and Dart.
- Backend candidate: Supabase (PostgreSQL, Auth, Storage, server-side functions), subject to validation against needs and existing code.
- Admin CMS candidate: a separately deployed web app only if a dedicated CMS is justified.
- AI: server-side calls only, grounded in approved content.
- Weather: provider adapter only after access, coverage, privacy, and terms are reviewed.
- CI: GitHub Actions or the repository's existing CI.

These are candidates, not authorization to install, migrate, or deploy services.

## Logical boundaries
1. Flutter app: UI, navigation, localization, session handling, cache, supported content rendering.
2. API/backend: authentication checks, authorization, input validation, rate limiting, recommendation orchestration, provider integrations.
3. Database: profiles, preferences, versioned content, assessments, recommendations, source records, consent, audit records.
4. CMS: authoring, translation, review, preview, publication, version history, rollback, audit trail.
5. External providers: AI/weather/push, accessed through server-side adapters with timeouts and fallbacks.

## Content delivery
- Use schemas and explicit versions for remote content.
- Support draft, review, approved, published, and archived states.
- Do not run arbitrary downloaded scripts or executable code.
- Retain last-known-good content where safe and appropriate.

## Security
- Server-side authorization is authoritative.
- Apply least privilege and database row-level policies where supported.
- Keep privileged keys server-side.
- Log administrative changes without unnecessarily logging sensitive user content.
