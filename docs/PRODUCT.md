# PRODUCT.md

## Project

Single-page website / landing page for a hotel or accommodation business.

## Project status

Preparation / pre-design implementation phase.

The final Figma design is still pending.

## Primary objective

Present the accommodation, its identity, rooms/units, services and visual content clearly, and convert visitors into direct reservation inquiries through a WhatsApp form flow.

## Product type

Status: `CONFIRMED`

- Single-page landing page.
- Responsive website.
- Public-facing marketing website.
- No authenticated user area.

## Confirmed high-level sections

Status: `CONFIRMED STRUCTURALLY`

1. Hero
2. About / Nosotros
3. Rooms / Units
4. Services
5. Gallery
6. Google Reviews
7. Contact
8. Footer

The final order, visual hierarchy and composition may change based on Figma.

## Primary CTA

Status: `CONFIRMED`

The primary CTA is a reservation inquiry form that redirects the visitor to the hotel's WhatsApp conversation with a prefilled message.

## Reservation inquiry form

Status: `CONFIRMED FUNCTIONALLY`

Fields:

- Name
- Email
- Check-in date
- Check-out date
- Number of adults
- Number of minors
- Preference / assistance request

Expected behavior:

- Visitor completes the form.
- The site opens the hotel's WhatsApp conversation with a message prefilled from the submitted fields.
- The visitor sends the WhatsApp message from WhatsApp.
- No database persistence is currently required.

The hotel's WhatsApp number and the final hotel name used in the message are pending.

## Google Reviews

Status: `CONFIRMED FUNCTIONAL INTENT`

The site should show:

- Google rating.
- Number of Google reviews.
- CTA: `Ver reseñas en Google`.
- CTA opens the Google review page in a new tab.

Status: `PENDING IMPLEMENTATION`

Initial implementation may use manually entered rating/review values.

Google Places API may be added later if the client requests automatic updates.

Do not implement scraping.

## Rooms / Units

Status: `CONFIRMED STRUCTURALLY`

The landing page will contain a section for rooms or accommodation units.

The project currently assumes multiple room/unit types may exist.

Status: `PENDING`

- information shown per unit,
- card structure,
- CTA behavior,
- modal/detail behavior,
- amenities,
- number of units,
- images,
- interaction model.

These details must not be invented before final content and/or Figma.

## Gallery

Status: `CONFIRMED`

A gallery section will exist.

Status: `PENDING`

The presentation format is owned by the design process and may be:

- cards,
- carousel,
- another Figma-defined layout.

## Services

Status: `CONFIRMED`

A services section will exist.

Status: `PENDING`

Specific services and presentation details.

## About / Nosotros

Status: `EXPECTED / PENDING FINAL CONFIRMATION`

An About / Nosotros section is expected.

Keep it in the structural plan unless later removed.

## Current scope

### In scope

- Single-page site.
- Responsive layout.
- Hotel/accommodation presentation.
- Rooms/units section.
- Services section.
- Gallery.
- Google Reviews presentation and external link.
- Reservation inquiry form.
- WhatsApp-based inquiry flow.
- Footer.
- Basic SEO.
- Deployment / production release.

### Out of scope for initial version

Status: `OUT OF SCOPE`

- Database.
- User authentication.
- User accounts.
- Admin dashboard.
- Booking engine.
- Online payments.
- CMS.
- Promotions section.
- Automatic Google Reviews synchronization.

Any of these items require explicit approval before implementation.

## Reference website

Reference concept:

`https://lapedrerapinamar.com.ar`

This reference is for general product direction only.

Do not copy its technical architecture, templates, hidden features, reservation systems or unused functionality.

## Design source of truth

Once received, the approved Figma file is the source of truth for:

- visual hierarchy,
- spacing,
- typography,
- colors,
- component appearance,
- responsive layout,
- image treatment,
- gallery style,
- explicit micro-interactions.

## Product principle

Do not overengineer.

The initial release should implement only the functionality the client needs.
