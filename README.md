# Holidu

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Holidu is a Munich-based vacation-rental search engine and short-term-rental technology company that helps travellers find and book holiday homes and helps property owners and managers distribute their inventory. Holidu exposes a public Developer Hub with two production REST APIs: the Affiliate API, for searching offers, retrieving property details, checking real-time availability and syncing changes; and the Connectivity (provider) API, a v2 property-management surface of ~50 operations covering apartments, multi-unit listings, descriptions, photos, facilities, reviews, rates, length-of-stay pricing, availability, extra costs, discounts, booking terms, payment and cancellation configuration, and bookings. Authentication is via per-partner API keys (with an OAuth 2.0 security service and Bearer-JWT callbacks), sandbox and production hosts are separated, and Holidu runs a HackerOne bug-bounty program. Holidu is backed by EQT Ventures, HV Capital and Northzone.

**Areas:** Company · Travel And Leisure · Vacation Rentals · Short-Term Rental · Hospitality · Property Management · Booking · Channel Manager · Connectivity · Affiliates

## Holidu on APIs.io

Everything profiled for Holidu is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/holidu/](https://apis.io/providers/holidu/)** — or go straight to one of the APIs or properties below.

### APIs (23)

- [Holidu Apartment API](https://apis.io/apis/holidu/holidu-apartment-api/) — The Apartment API from Holidu — 5 operation(s) for apartment.
- [Holidu Availabilities API](https://apis.io/apis/holidu/holidu-availabilities-api/) — The Availabilities API from Holidu — 1 operation(s) for availabilities.
- [Holidu Availability API](https://apis.io/apis/holidu/holidu-availability-api/) — The Availability API from Holidu — 1 operation(s) for availability.
- [Holidu Booking Terms API](https://apis.io/apis/holidu/holidu-booking-terms-api/) — The Booking Terms API from Holidu — 5 operation(s) for booking terms.
- [Holidu Bookings API](https://apis.io/apis/holidu/holidu-bookings-api/) — The Bookings API from Holidu — 3 operation(s) for bookings.
- [Holidu Changed API](https://apis.io/apis/holidu/holidu-changed-api/) — The Changed API from Holidu — 1 operation(s) for changed.
- [Holidu Descriptions API](https://apis.io/apis/holidu/holidu-descriptions-api/) — The Descriptions API from Holidu — 1 operation(s) for descriptions.
- [Holidu Details API](https://apis.io/apis/holidu/holidu-details-api/) — The Details API from Holidu — 1 operation(s) for details.
- [Holidu Discounts API](https://apis.io/apis/holidu/holidu-discounts-api/) — The Discounts API from Holidu — 2 operation(s) for discounts.
- [Holidu Extra Costs API](https://apis.io/apis/holidu/holidu-extra-costs-api/) — The Extra Costs API from Holidu — 1 operation(s) for extra costs.
- [Holidu Facilities API](https://apis.io/apis/holidu/holidu-facilities-api/) — The Facilities API from Holidu — 3 operation(s) for facilities.
- [Holidu LOS API](https://apis.io/apis/holidu/holidu-los-api/) — The LOS API from Holidu — 2 operation(s) for los.
- [Holidu LOS Push API](https://apis.io/apis/holidu/holidu-los-push-api-api/) — Length of Stay pricing push operations.
- [Holidu MultiUnit API](https://apis.io/apis/holidu/holidu-multiunit-api/) — The MultiUnit API from Holidu — 1 operation(s) for multiunit.
- [Holidu MultiUnit Facility API](https://apis.io/apis/holidu/holidu-multiunit-facility-api/) — The MultiUnit Facility API from Holidu — 1 operation(s) for multiunit facility.
- [Holidu MultiUnit Localization API](https://apis.io/apis/holidu/holidu-multiunit-localization-api/) — The MultiUnit Localization API from Holidu — 1 operation(s) for multiunit localization.
- [Holidu MultiUnit Photo API](https://apis.io/apis/holidu/holidu-multiunit-photo-api/) — The MultiUnit Photo API from Holidu — 1 operation(s) for multiunit photo.
- [Holidu Photos API](https://apis.io/apis/holidu/holidu-photos-api/) — The Photos API from Holidu — 1 operation(s) for photos.
- [Holidu Rates API](https://apis.io/apis/holidu/holidu-rates-api/) — The Rates API from Holidu — 1 operation(s) for rates.
- [Holidu Reviews API](https://apis.io/apis/holidu/holidu-reviews-api/) — The Reviews API from Holidu — 1 operation(s) for reviews.
- [Holidu Search API](https://apis.io/apis/holidu/holidu-search-api/) — The Search API from Holidu — 1 operation(s) for search.
- [Holidu Test API](https://apis.io/apis/holidu/holidu-test-api/) — The Test API from Holidu — 1 operation(s) for test.
- [Holidu Testa API](https://apis.io/apis/holidu/holidu-testa-api/) — The Testa API from Holidu — 1 operation(s) for testa.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Holidu Webhooks](https://apis.io/asyncapis/holidu/holidu-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [holidu](https://apis.io/servers/holidu/holidu/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Holidu Agentic Access](https://apis.io/agentic-access/holidu/holidu-agentic-access/)

#### Collections (22)

Postman and Open Collection request collections.

- [Affiliate Apartment API](https://apis.io/collections/holidu/open-holidu-apartment-api/)
- [Affiliate Apartment Availabilities API](https://apis.io/collections/holidu/open-holidu-availabilities-api/)
- [Affiliate Apartment Availability API](https://apis.io/collections/holidu/open-holidu-availability-api/)
- [Affiliate Apartment Booking Terms API](https://apis.io/collections/holidu/open-holidu-booking-terms-api/)
- [Affiliate Apartment Bookings API](https://apis.io/collections/holidu/open-holidu-bookings-api/)
- [Affiliate Apartment Changed API](https://apis.io/collections/holidu/open-holidu-changed-api/)
- [Affiliate Apartment Descriptions API](https://apis.io/collections/holidu/open-holidu-descriptions-api/)
- [Affiliate Apartment Details API](https://apis.io/collections/holidu/open-holidu-details-api/)
- [Affiliate Apartment Discounts API](https://apis.io/collections/holidu/open-holidu-discounts-api/)
- [Affiliate Apartment Extra Costs API](https://apis.io/collections/holidu/open-holidu-extra-costs-api/)
- [Affiliate Apartment Facilities API](https://apis.io/collections/holidu/open-holidu-facilities-api/)
- [Affiliate Apartment LOS API](https://apis.io/collections/holidu/open-holidu-los-api/)
- [Affiliate Apartment LOS Push API API](https://apis.io/collections/holidu/open-holidu-los-push-api-api/)
- [Affiliate Apartment MultiUnit API](https://apis.io/collections/holidu/open-holidu-multiunit-api/)
- [Affiliate Apartment MultiUnit Facility API](https://apis.io/collections/holidu/open-holidu-multiunit-facility-api/)
- [Affiliate Apartment MultiUnit Localization API](https://apis.io/collections/holidu/open-holidu-multiunit-localization-api/)
- [Affiliate Apartment MultiUnit Photo API](https://apis.io/collections/holidu/open-holidu-multiunit-photo-api/)
- [Affiliate Apartment Photos API](https://apis.io/collections/holidu/open-holidu-photos-api/)
- [Affiliate Apartment Rates API](https://apis.io/collections/holidu/open-holidu-rates-api/)
- [Affiliate Apartment Search API](https://apis.io/collections/holidu/open-holidu-search-api/)
- [Affiliate Apartment Test API](https://apis.io/collections/holidu/open-holidu-test-api/)
- [Affiliate Apartment Testa API](https://apis.io/collections/holidu/open-holidu-testa-api/)

#### Overlays (2)

OpenAPI overlays, including conversational phrasing for each operation.

- [Holidu Affiliate Api Overlay](https://apis.io/overlays/holidu/holidu-affiliate-api-overlay/)
- [Holidu Connectivity Api Overlay](https://apis.io/overlays/holidu/holidu-connectivity-api-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Holidu Authentication](https://apis.io/security/holidu/holidu-authentication/)
- [Holidu Domain Security](https://apis.io/security/holidu/holidu-domain-security/)
- [Holidu Vulnerability Disclosure](https://apis.io/security/holidu/holidu-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Holidu Scopes](https://apis.io/scopes/holidu/holidu-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.holidu.com/)
- [Documentation](https://developer.holidu.com/docs)
- [Getting started](https://developer.holidu.com/reference/how-to-integrate-with-holidu-capabilities-use-cases)
- [API reference](https://developer.holidu.com/reference)
- [Sign up](https://partner.holidu.com/)
- [Support](https://developer.holidu.com/discuss)
- [Changelog](https://developer.holidu.com/changelog)
- [Security](https://www.holidu.com/.well-known/security.txt)
- [GitHub](https://github.com/holidu)
- [Status](https://status.holidu.com/)

## API Evangelist rating

**Kin Score 42.6** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 56.9 |
| Contract governance | 4.5 |
| Operational transparency | 48.7 |
| Developer ergonomics | 42.3 |
| Access clarity | 0.0 |

**Agent readiness 40.6** — agent-native

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | verified |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 32.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/holidu/](https://apis.io/providers/holidu/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Holidu: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/holidu/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
