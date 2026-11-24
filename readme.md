# NSTMS — National School Travel Management and Child Safety System

A static HTML/CSS front-end prototype based on the supplied reference screenshot. The public landing page and authenticated workspaces use a consistent navy, violet, blue, white and pale-lavender design system.

## Included pages

- `index.html` — public landing page with programme overview, priorities, benefits, workflow, FAQ, registration CTA and footer.
- `dashboard.html` — school administrator workspace with overview cards, tour analytics, quick actions, recent activity and trip-readiness checklist.
- `ministry-dashboard.html` — national oversight workspace with review queue, school/transport indicators, inspection coordination and sample trip submissions.
- `login.html` — sign-in interface.
- `register.html` — account-type selection for schools, parents/guardians, drivers/transport providers and authorised government officers.
- `css/styles.css` — shared responsive stylesheet.
- `assets/school-trip-hero.jpg` — local hero photograph extracted from the supplied visual concept asset set.

## Run locally

No build step is needed for this static prototype. Open `index.html` directly in a modern browser, or serve the directory using a local development server. For example:

```bash
npx serve .
```

## Important prototype limitations

This delivery is a front-end visual prototype. It does **not** implement authentication, account creation, database persistence, authorisation decisions, file upload, official document validation, payment collection, parent notifications, GPS tracking, incident dispatch, audit logging or government integrations. Forms are presentation-only and must be connected to secure backend endpoints.

All names, records, counts, trip references, statuses, activity entries, contact details and dates shown in the dashboard are illustrative demo data. They must be replaced with approved live data before any operational use. The interface must not be presented as a live Government of Uganda service or as an official endorsement without formal authorisation.

## Production implementation recommendations

For a production build, use a React + TypeScript application (Vite or an approved enterprise framework), a secured API layer (for example NestJS or Express with strict validation), PostgreSQL, object storage with malware scanning, short-lived authenticated sessions, MFA for privileged users, role-based and school/district-scoped authorisation, immutable security/audit events, encrypted backups, monitoring and tested disaster recovery. Integrations with driver licensing, vehicle registration, insurance, inspection, police and government identity systems require formal agreements and verified APIs; do not treat data entered by a user as official verification.

Apply Uganda's data protection requirements and child-safeguarding practices from the design stage. Minimise learner data, restrict who can access it, define lawful purposes and retention periods, log sensitive access, and complete a privacy/security impact assessment before handling live child records.

## Design system

- Primary navy: `#111b57`
- Primary violet: `#672fe9`
- Primary blue: `#1169ef`
- Teal: `#05a88a`
- Amber: `#f4a300`
- Public canvas: `#f4f5ff`
- Typography: Plus Jakarta Sans with system fallbacks

The stylesheet includes responsive layouts for desktop, tablet and mobile, keyboard focus indicators, reduced-motion support, semantic landmarks and descriptive form labels.
