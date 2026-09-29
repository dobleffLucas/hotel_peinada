# AGENTS.md

## Purpose

This is the main entry point for AI coding agents working on this repository.

Before planning or coding, read the project documentation in this order:

1. `docs/PRODUCT.md`
2. `docs/SPEC.md`
3. `docs/ARCHITECTURE.md`
4. `docs/DECISIONS.md`
5. `docs/TASKS.md`

## Core rules

- Do not invent product requirements.
- Do not add features that are not present in `docs/SPEC.md`.
- Do not treat pending decisions as confirmed decisions.
- If a requirement is marked as `PENDING`, preserve that uncertainty.
- Do not change approved architecture decisions without documenting the reason in `docs/DECISIONS.md`.
- Prefer small, reversible changes.
- Work on one task at a time.
- Before finishing a task, verify that the implementation matches the relevant acceptance criteria.
- Do not add a database, authentication, booking engine, CMS, WhatsApp integration, payment system, or Google Places API unless explicitly approved.
- Figma is the source of truth for visual implementation once the final design is received.
- `docs/SPEC.md` is the source of truth for functional behavior.

## Current project status

The project is in the preparation phase.

The final Figma design has not been received yet.

Do not implement final UI layouts, spacing systems, typography, colors, gallery behavior, or room-card behavior until those details are available.

## AI handoff protocol

When starting work:

1. Read the documentation.
2. Identify the relevant task in `docs/TASKS.md`.
3. State what you are going to change.
4. Make only the changes needed for that task.
5. Verify the result.
6. Report:
   - files changed,
   - functionality implemented,
   - tests/checks performed,
   - unresolved questions.

## Conflict resolution

If documents appear to conflict, use this priority:

1. Latest explicit human instruction.
2. `docs/DECISIONS.md`
3. `docs/SPEC.md`
4. `docs/PRODUCT.md`
5. `docs/ARCHITECTURE.md`
6. `docs/TASKS.md`

If uncertainty remains, do not guess.
