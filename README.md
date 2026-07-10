# SimplePractice (simplepractice)

SimplePractice is a cloud-based practice management platform and EHR for behavioral and mental health, therapy, and wellness practices. It covers scheduling and calendars, client management, telehealth, intake and clinical documentation, insurance and superbill billing, online payments, and a secure client portal (Client Secure Messaging).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/simplepractice/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/simplepractice/refs/heads/main/apis.yml)

## Access Model — No Public Developer API

This entry is an honest, gated stub. As of cataloging (2026-07-10), **SimplePractice does not publish a public, self-serve developer API.** Specifically:

- **No developer portal** and **no published API documentation** (there is no `developers.simplepractice.com` or equivalent).
- **No documented REST endpoints, base URL, authentication scheme, or OpenAPI definition.**
- **No public webhooks** and no supported programmatic integration for third parties. Customers and reviewers repeatedly note there is no way to connect the platform to external tools via official automation (Zapier/Make/webhooks do not have a useful SimplePractice trigger surface).
- The **GitHub organization** ([github.com/simplepractice](https://github.com/simplepractice)) hosts front-end components and internal utilities (Ember/Bootstrap widgets, a Langfuse Ruby SDK, shared RuboCop config) — **not** API specs, OpenAPI, or public API SDKs.

The only programmatic surface is the **SimplePractice Enterprise scheduling integration** (announced September 2022). It connects EAPs and Managed Care Organizations (MCOs) to overlapping SimplePractice provider accounts so members and care coordinators can filter in-network behavioral health providers, view real-time availability, and request appointments. It is delivered through **negotiated enterprise partnerships**, with **no public endpoints, documentation, or developer program** — so no endpoints are asserted here (see `endpointsModeled` in `review.yml`).

> Caution: Several third-party sites advertise a "stable SimplePractice REST API" for clients, appointments, notes, and billing. These are **unofficial** and are **not** backed by any SimplePractice developer program. They were not corroborated by any SimplePractice-owned source and are treated as unreliable.

There is **no** public API for the logical domains a developer would want — Clients, Appointments, Clinical Notes, or Billing. If SimplePractice launches a public developer API, this entry should be upgraded from a stub to a full catalog.

## Tags

- Behavioral Health
- Mental Health
- EHR
- Practice Management
- Healthcare
- Scheduling
- Telehealth
- HIPAA
- Partner API
- No Public API

## Timestamps

- **Created:** 2026-07-10
- **Modified:** 2026-07-10

## APIs

### SimplePractice Enterprise Scheduling API

Partner-only integration (announced September 2022) that connects to overlapping SimplePractice provider accounts so that EAPs, MCOs, members, and care coordinators can filter in-network behavioral health providers by location and specialty, view real-time availability, and request appointments. **No public developer documentation, base URL, authentication, or OpenAPI has been published** — endpoints are modeled/absent, not fabricated.

- **Human URL:** [SimplePractice Enterprise API announcement](https://www.simplepractice.com/press/simplepractice-enterprise-launches-api/)

#### Tags

- Scheduling
- Availability
- Appointments
- Behavioral Health
- Partner API
- Enterprise

## Pricing

SimplePractice is sold as a per-account monthly SaaS subscription (this is application pricing, not API pricing). Standard published monthly rates:

- **Starter:** $49/month
- **Essential:** $79/month
- **Plus:** $99/month (the only tier that supports adding clinicians)

Add-ons and fees:

- **Additional clinicians (Plus only):** $74/mo (2–5), $72/mo (6–15), $69/mo (16+)
- **Practice Managers:** $39/mo each
- **AI Note Taker:** $35/mo per clinician
- **ePrescribe:** $49/mo per clinician plus a one-time $89 setup fee per clinician
- **Card processing:** 3.15% + $0.30 per transaction
- **Claim processing:** from $0.25 per claim
- **CPT licensing:** $20 per clinician per year

SimplePractice frequently runs a 50%-off promotion for the first three months. Verify current numbers on the [pricing page](https://www.simplepractice.com/pricing/).

See [`plans/simplepractice-plans-pricing.yml`](plans/simplepractice-plans-pricing.yml) and [`finops/simplepractice-finops.yml`](finops/simplepractice-finops.yml).

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/simplepractice)
- [Website](https://www.simplepractice.com)
- [GitHub Organization](https://github.com/simplepractice)
- [Documentation](https://www.simplepractice.com/press/simplepractice-enterprise-launches-api/) (Enterprise API announcement — the closest thing to public API docs)
- [Plans](plans/simplepractice-plans-pricing.yml)
- [Fin Ops](finops/simplepractice-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
