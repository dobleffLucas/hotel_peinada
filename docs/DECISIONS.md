# DECISIONS.md

This document records approved project decisions.

Do not reopen an accepted decision unless:
- the client changes requirements,
- new technical information invalidates it,
- a human explicitly asks to reconsider it.

---

## DEC-001 — Single-page landing page

Status: `ACCEPTED`

Decision:
The initial website will be a single-page landing page.

Reason:
Current project needs do not justify a multi-page application.

---

## DEC-002 — Primary conversion through WhatsApp reservation inquiry form

Status: `ACCEPTED`

Decision:
The primary CTA will be a reservation inquiry form that opens the hotel's WhatsApp conversation with a prefilled message. The visitor sends the message from WhatsApp.

Form fields:
- Name
- Email
- Check-in date
- Check-out date
- Number of adults
- Number of minors
- Preference / assistance request

---

## DEC-003 — No database in initial version

Status: `ACCEPTED`

Decision:
The initial website will not persist contact submissions in a database.

Reason:
Current requirement is only to send inquiries to the hotel by email.

---

## DEC-004 — Scoped WhatsApp reservation inquiry flow

Status: `ACCEPTED`

Decision:
Include only the WhatsApp reservation inquiry flow defined in DEC-002.

Do not add a floating WhatsApp button or any other WhatsApp flow in the initial version.

---

## DEC-005 — No booking engine

Status: `ACCEPTED`

Decision:
The initial website will not implement booking functionality.

---

## DEC-006 — Google review summary

Status: `ACCEPTED FUNCTIONAL INTENT`

Decision:
The website should show Google rating and review count and offer a `Ver reseñas en Google` CTA that opens the review destination in a new tab.

Implementation detail:
Data may initially be entered manually.

Automatic API synchronization remains unapproved.

---

## DEC-007 — Do not scrape Google Maps

Status: `ACCEPTED`

Decision:
Google review/rating data must not be collected through scraping.

If automatic synchronization is later required, evaluate the official Google Places API.

---

## DEC-008 — Figma owns final visual decisions

Status: `ACCEPTED`

Decision:
The approved Figma design is the visual source of truth.

Do not invent:
- colors,
- typography,
- spacing,
- card behavior,
- gallery interaction,
- final responsive composition.

---

## DEC-009 — AI agents must not invent requirements

Status: `ACCEPTED`

Decision:
All AI agents must preserve uncertainty in unresolved areas.

A `PENDING` item is not permission to choose an implementation silently.

---

# Pending decisions

The following have not been approved yet:

- final frontend stack,
- hosting provider,
- final room/unit content model,
- gallery interaction,
- exact breakpoint strategy,
- final Google Reviews implementation,
- analytics,
- final domain configuration,
- exact SEO metadata,
- animation/motion strategy.
- hotel WhatsApp number,
- final hotel name for the WhatsApp message.
