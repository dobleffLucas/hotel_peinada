# TASKS.md

## Usage

Tasks should move through:

`TODO → IN PROGRESS → REVIEW → DONE`

AI agents should work on one task at a time unless explicitly instructed otherwise.

Do not mark a task `DONE` without verification.

---

# Phase 0 — Project preparation

## TODO

- [ ] T0.1 Confirm frontend stack.
- [ ] T0.2 Initialize application project.
- [ ] T0.3 Configure repository conventions.
- [ ] T0.4 Add project documentation.
- [ ] T0.5 Configure `.gitignore`.
- [ ] T0.6 Add `.env.example` if/when environment variables are required.
- [ ] T0.7 Decide deployment provider.
- [ ] T0.8 Configure hotel WhatsApp number and final hotel name for reservation inquiries.
- [ ] T0.9 Create initial README for developers.

---

# Phase 1 — Design handoff

Blocked until Figma is received.

- [ ] T1.1 Review complete Figma file.
- [ ] T1.2 Confirm landing section order.
- [ ] T1.3 Identify reusable components.
- [ ] T1.4 Confirm desktop behavior.
- [ ] T1.5 Confirm tablet behavior.
- [ ] T1.6 Confirm mobile behavior.
- [ ] T1.7 Extract typography.
- [ ] T1.8 Extract color tokens.
- [ ] T1.9 Extract spacing/layout rules.
- [ ] T1.10 Export/obtain approved assets.
- [ ] T1.11 Confirm gallery behavior.
- [ ] T1.12 Confirm room/unit card behavior.
- [ ] T1.13 Confirm animations/interactions.
- [ ] T1.14 Update `SPEC.md` with approved design behavior.
- [ ] T1.15 Update `DECISIONS.md` with newly approved decisions.

---

# Phase 2 — Core UI

Blocked until design handoff is complete.

- [ ] T2.1 Implement global layout.
- [ ] T2.2 Implement responsive navigation/header.
- [ ] T2.3 Implement Hero.
- [ ] T2.4 Implement About / Nosotros.
- [ ] T2.5 Implement Rooms / Units.
- [ ] T2.6 Implement Services.
- [ ] T2.7 Implement Gallery.
- [ ] T2.8 Implement Google Reviews section.
- [ ] T2.9 Implement Contact section.
- [ ] T2.10 Implement Footer.

---

# Phase 3 — Functional behavior

- [ ] T3.1 Implement navigation between landing sections.
- [ ] T3.2 Implement reservation inquiry form field validation.
- [ ] T3.3 Implement WhatsApp prefilled-message generation and redirect.
- [ ] T3.4 Implement redirecting state.
- [ ] T3.5 Implement validation feedback.
- [ ] T3.6 Verify malformed or missing WhatsApp configuration is handled safely.
- [ ] T3.7 Configure Google rating/review values.
- [ ] T3.8 Configure Google Reviews external URL.
- [ ] T3.9 Ensure external reviews link opens in new tab.

---

# Phase 4 — Content integration

- [ ] T4.1 Add final hotel copy.
- [ ] T4.2 Add final room/unit content.
- [ ] T4.3 Add final services content.
- [ ] T4.4 Add final gallery images.
- [ ] T4.5 Add final review count/rating.
- [ ] T4.6 Add final contact details.
- [ ] T4.7 Add approved legal/footer information if applicable.

---

# Phase 5 — QA

## Functional QA

- [ ] T5.1 Verify all navigation.
- [ ] T5.2 Verify reservation inquiry validation.
- [ ] T5.3 Verify WhatsApp message generation and destination.
- [ ] T5.4 Verify redirecting/error states.
- [ ] T5.5 Verify Google Reviews link.
- [ ] T5.6 Verify all external links.

## Visual QA

- [ ] T5.7 Compare desktop implementation against Figma.
- [ ] T5.8 Compare tablet implementation against Figma.
- [ ] T5.9 Compare mobile implementation against Figma.
- [ ] T5.10 Verify typography.
- [ ] T5.11 Verify spacing.
- [ ] T5.12 Verify image crops/aspect ratios.
- [ ] T5.13 Verify interaction states.

## Technical QA

- [ ] T5.14 Run build.
- [ ] T5.15 Run lint if configured.
- [ ] T5.16 Run automated tests if configured.
- [ ] T5.17 Check console for errors.
- [ ] T5.18 Verify no secrets are exposed.
- [ ] T5.19 Verify image optimization.
- [ ] T5.20 Basic keyboard accessibility review.
- [ ] T5.21 Basic metadata/SEO review.

---

# Phase 6 — Production

- [ ] T6.1 Configure production environment.
- [ ] T6.2 Configure page title.
- [ ] T6.3 Configure meta description.
- [ ] T6.4 Configure favicon.
- [ ] T6.5 Configure Open Graph metadata.
- [ ] T6.6 Deploy production build.
- [ ] T6.7 Connect domain.
- [ ] T6.8 Verify HTTPS.
- [ ] T6.9 Test production WhatsApp reservation inquiry flow.
- [ ] T6.10 Test production external links.
- [ ] T6.11 Final client review.
- [ ] T6.12 Resolve approved final issues.
- [ ] T6.13 Deliver project.

---

# Definition of Done — Task

A task is done when:

- implementation matches the relevant `SPEC.md` requirement,
- implementation does not contradict `DECISIONS.md`,
- visual work matches Figma where applicable,
- relevant responsive states work,
- no obvious regression is introduced,
- required build/lint/test checks pass,
- unresolved issues are reported.

# Definition of Done — Project

The initial project is done when:

- approved sections are implemented,
- WhatsApp reservation inquiry form works in production,
- Google Reviews link is correct,
- responsive behavior is approved,
- implementation matches approved Figma,
- basic SEO is configured,
- production deployment works,
- final client review is complete.
