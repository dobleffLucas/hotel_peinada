# ARCHITECTURE.md

## Architecture status

Version: Draft 0.1

The final technology stack has not yet been selected.

Do not infer a framework from this document.

## Current architectural constraints

Status: `CONFIRMED`

The initial product is a relatively simple public landing page.

The architecture should favor:

- low operational complexity,
- fast page delivery,
- simple deployment,
- maintainability,
- good SEO,
- responsive frontend implementation,
- minimal backend surface.

## Confirmed non-requirements

The initial architecture does not require:

- relational database,
- NoSQL database,
- authentication,
- user sessions,
- admin dashboard,
- booking backend,
- payment backend,
- CMS.

## Frontend

Status: `PENDING`

Framework / tooling has not been chosen.

Candidate approaches may be evaluated separately.

The implementation should support:
- component reuse,
- responsive design,
- structured content,
- image optimization,
- WhatsApp reservation inquiry form integration.

Do not initialize a final framework until the human owner confirms the stack.

## Backend

Status: `PENDING / MINIMAL`

A traditional backend is not currently required.

The initial WhatsApp inquiry flow can be implemented client-side by generating the configured WhatsApp link and its encoded prefilled message. No server-side delivery mechanism is required.

The hotel's WhatsApp number and final hotel name remain configuration values pending confirmation.

## WhatsApp reservation inquiry architecture

Status: `CONFIRMED AT HIGH LEVEL`

The form constructs the WhatsApp deep link client-side. The final number must be configured outside the message-generation logic. No API credentials are required for this flow.

## Google Reviews architecture

Status: `PENDING`

Initial likely approach:
- manually configured rating,
- manually configured review count,
- external Google Reviews URL.

Optional future approach:
- Google Places API.

No scraping.

## Content model

Status: `CONFIRMED AT HIGH LEVEL`

Even without a database, repeated content should be represented structurally when useful.

Examples:
- room/unit list,
- services list,
- gallery images.

Avoid duplicating repeated markup if the selected stack supports reusable data structures/components.

## Deployment

Status: `PENDING`

Hosting provider has not been selected.

Required characteristics:
- HTTPS,
- custom domain support,
- reliable static/frontend deployment,
- support for the chosen form/email approach.

## Environment variables

Status: `CONFIRMED PRACTICE`

If external services require secrets, they must be stored as environment variables.

Repository should include `.env.example` when environment variables are introduced.

Never commit real secrets.

## Repository structure

Recommended documentation structure:

```text
/
├── AGENTS.md
├── CLAUDE.md
├── README.md
├── docs/
│   ├── README.md
│   ├── PRODUCT.md
│   ├── SPEC.md
│   ├── ARCHITECTURE.md
│   ├── DECISIONS.md
│   └── TASKS.md
└── ... application source files
```

Application-source structure is pending stack selection.

## Engineering principles

- Do not overengineer.
- Avoid unnecessary dependencies.
- Keep the architecture proportional to the project.
- Prefer explicit configuration over hidden behavior.
- Keep product content separate from implementation logic where practical.
- Make future optional features possible without building them prematurely.
