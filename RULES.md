# Project Rules

1. Inspect the repository, Git status, existing code, dependencies, and docs before making changes.
2. Work on one explicitly scoped task at a time. State the plan, files to change, and acceptance criteria first.
3. Preserve existing user work. Do not overwrite, delete, reset, force-push, or reformat unrelated files.
4. Do not create duplicate app, backend, database, authentication, or CMS layers if an equivalent already exists.
5. Do not create empty placeholder files or directories just to match a proposed architecture.
6. Run relevant formatters, analyzers, tests, and builds when available. Report exactly what ran and what did not.
7. Review `git diff` and `git status` before finishing. Never claim a check passed unless it was run.
8. Update `TASKS.md`, `docs/MEMORY.md`, and relevant documentation when decisions or progress change.
9. Never hardcode secrets, tokens, credentials, private keys, or production endpoints containing secrets.
10. Do not deploy, publish, spend money, change billing, or modify production data without explicit approval.
11. Keep mutable copy, translations, approved wellness content, assessment configuration, recommendation rules, and notification templates backend/CMS-managed.
12. Do not download or execute arbitrary code from the backend. Use versioned, schema-validated content and supported app components.
13. English and Hindi are first-class languages. Plan for translation review and missing-translation fallbacks.
14. Keep wellness guidance educational, non-diagnostic, transparent about sources, and reviewed by appropriately qualified people before publication.
15. Treat Prakriti self-reflection as unvalidated until its method and scoring have appropriate evidence and qualified review. Allow uncertain or mixed results.
16. Use AI only through a secured server-side boundary where appropriate. Never ship provider API keys in the app.
17. Apply least privilege, server-side authorization, secure session handling, input validation, rate limits, privacy protections, and data deletion support.
18. Use accessible, responsive, performant UI. Use 3D selectively and provide a lightweight fallback.
19. Prefer small, focused changes and readable code over speculative abstraction.
20. If requirements or evidence are unclear, document the uncertainty and ask before making consequential assumptions.
