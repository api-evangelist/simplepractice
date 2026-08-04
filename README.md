# SimplePractice (simplepractice)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
