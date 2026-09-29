# Project Documentation

This folder contains the source of truth for the project.

## Documents

### `PRODUCT.md`
Defines what the product is, its objective, scope, exclusions, and current assumptions.

### `SPEC.md`
Defines functional behavior and acceptance criteria.

### `ARCHITECTURE.md`
Defines technical structure and constraints. Unconfirmed technical choices remain pending.

### `TASKS.md`
Tracks implementation work in execution order.

### `DECISIONS.md`
Records approved decisions so different AI agents do not repeatedly reopen the same topics.

## Recommended workflow

### Planning AI
- updates PRODUCT, SPEC, ARCHITECTURE and TASKS.
- does not implement code unless explicitly requested.

### Implementation AI
- reads all project documents.
- selects one task from TASKS.
- implements only that task.
- verifies it before marking it complete.

### Review AI
- compares implementation against SPEC, DECISIONS and Figma.
- distinguishes bugs/spec deviations from optional improvements.

### Human review
- approves relevant changes before merging or delivering.

## Status labels

Use these labels consistently:

- `CONFIRMED`
- `CONFIRMED STRUCTURALLY`
- `CONFIRMED FUNCTIONALLY`
- `PENDING`
- `EXPECTED / PENDING FINAL CONFIRMATION`
- `OUT OF SCOPE`
- `OPTIONAL FUTURE`
