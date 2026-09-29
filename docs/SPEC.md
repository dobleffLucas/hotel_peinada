# SPEC.md

## Specification status

Version: Draft 0.1

This specification contains confirmed requirements and explicitly marked pending items.

AI agents must not treat pending items as requirements.

---

# 1. Page model

## SPEC-001 — Single-page architecture

Status: `CONFIRMED`

The website must operate primarily as a single-page landing page.

Navigation should move the user between sections of the landing page.

Final navigation labels and ordering depend on Figma/content approval.

---

# 2. Responsive behavior

## SPEC-002 — Responsive website

Status: `CONFIRMED`

The website must be usable on:

- desktop,
- tablet,
- mobile.

Exact breakpoints and visual adaptations are `PENDING` until Figma is available.

---

# 3. Hero

## SPEC-003 — Hero section

Status: `CONFIRMED STRUCTURALLY`

The landing page must include a Hero section.

Status: `PENDING`

- copy,
- imagery,
- CTA label,
- CTA destination,
- layout,
- animation.

---

# 4. About / Nosotros

## SPEC-004 — About section

Status: `EXPECTED / PENDING FINAL CONFIRMATION`

The current structure includes an About / Nosotros section.

Final content and layout are pending.

---

# 5. Rooms / Units

## SPEC-005 — Rooms/Units section

Status: `CONFIRMED STRUCTURALLY`

The landing page must include a rooms/units section.

The implementation should support multiple room/unit items without requiring a structural rewrite.

Status: `PENDING`

- number of items,
- fields per item,
- images,
- capacity,
- amenities,
- CTA behavior,
- modal/detail behavior,
- interaction model.

Do not invent these details.

---

# 6. Services

## SPEC-006 — Services section

Status: `CONFIRMED`

The landing page must include a services section.

Status: `PENDING`

- services list,
- icons,
- copy,
- visual presentation.

---

# 7. Gallery

## SPEC-007 — Gallery section

Status: `CONFIRMED`

The landing page must include a gallery.

Status: `PENDING`

The final interaction pattern is defined by Figma.

Possible implementations include cards or carousel, but neither is confirmed.

---

# 8. Google Reviews

## SPEC-008 — Review summary

Status: `CONFIRMED FUNCTIONALLY`

The website must be able to display:

- Google rating value,
- Google review count.

Initial values may be manually configured.

Example presentation only:

`4.7 ★ — 328 reseñas en Google`

This example is not real client data.

## SPEC-009 — Reviews CTA

Status: `CONFIRMED`

The reviews section must include a CTA with wording equivalent to:

`Ver reseñas en Google`

Behavior:

- opens the hotel's Google reviews page,
- opens in a new browser tab.

The final URL is pending.

## SPEC-010 — Review data source

Status: `PENDING`

Initial preferred approach:
- manually configured values.

Optional future approach:
- Google Places API.

Not allowed:
- scraping Google Maps.

---

# 9. Contact

## SPEC-011 — Contact form fields

Status: `CONFIRMED`

The form must contain:

- Name
- Phone
- Email
- Message

## SPEC-012 — Contact delivery

Status: `CONFIRMED FUNCTIONAL INTENT`

Submitting the form must send the inquiry to the hotel by email.

Status: `PENDING TECHNICAL DECISION`

The email delivery mechanism has not been chosen yet.

## SPEC-013 — Database

Status: `OUT OF SCOPE`

The initial contact flow must not require a database.

## SPEC-014 — Form validation

Status: `CONFIRMED AT HIGH LEVEL`

The form must reject obviously invalid or incomplete submissions.

Exact validation rules are pending technical implementation.

At minimum, implementation should consider:
- required fields,
- valid email format,
- sensible message length,
- basic protection against accidental duplicate/spam submissions.

Do not add complex anti-abuse infrastructure unless required.

## SPEC-015 — Form feedback

Status: `CONFIRMED FUNCTIONALLY`

The user must receive visible feedback after attempting to send the form.

States should include:
- sending,
- success,
- error.

Exact visual treatment is defined by Figma.

---

# 10. WhatsApp

## SPEC-016 — WhatsApp

Status: `OUT OF SCOPE`

The initial version does not include:

- floating WhatsApp button,
- WhatsApp CTA,
- automatic WhatsApp message generation.

May be added later with explicit approval.

---

# 11. Booking and payments

## SPEC-017 — Booking engine

Status: `OUT OF SCOPE`

No booking engine is required in the initial version.

## SPEC-018 — Online payments

Status: `OUT OF SCOPE`

No online payment flow is required.

---

# 12. SEO

## SPEC-019 — Basic SEO

Status: `CONFIRMED`

The production site should include basic SEO setup.

Expected items:
- page title,
- meta description,
- semantic heading structure,
- alt text for meaningful images,
- Open Graph metadata where appropriate,
- crawlable public content.

Final metadata values are pending client content.

---

# 13. Performance

## SPEC-020 — Web performance

Status: `CONFIRMED AT HIGH LEVEL`

The site should avoid unnecessary technical weight.

Images should be appropriately optimized for web delivery.

Heavy libraries should not be introduced without a clear need.

No numeric performance target is confirmed yet.

---

# 14. Accessibility

## SPEC-021 — Basic accessibility

Status: `CONFIRMED AT HIGH LEVEL`

Implementation should use:
- semantic HTML,
- keyboard-accessible controls,
- labels for form fields,
- meaningful alt text,
- visible focus states,
- sufficient contrast according to the approved design.

---

# 15. Acceptance criteria

The initial project is functionally complete when:

- all approved sections exist,
- navigation works,
- contact form works,
- email delivery works,
- Google Reviews CTA opens the correct destination,
- responsive behavior is approved,
- implementation matches approved Figma,
- basic SEO is configured,
- production deploy is working,
- no out-of-scope feature has been added without approval.
