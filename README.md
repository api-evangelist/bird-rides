# Bird

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

Bird is a shared electric scooter and bike micromobility operator headquartered in Miami, Florida and operating as the global anchor brand of Third Lane Mobility, Inc. Founded in 2017 by Travis VanderZanden, Bird pioneered the dockless electric scooter category in Santa Monica, California and rapidly expanded to hundreds of cities across North America, Europe, and the Middle East. After overstating revenue, delisting from the NYSE in September 2023 (ticker BRDS), and filing Chapter 11 bankruptcy in December 2023, Bird emerged in April 2024 under the new private parent company Third Lane Mobility, Inc., which also owns the Spin brand acquired from TIER in September 2023. Bird operates the Bird Three e-scooter and a Bird Bikeshare service, plus the Bird Platform white-label program for independent fleet operators and a Cities partner program that ships "in-depth APIs" and operator dashboards to municipal partners. Bird publishes public General Bikeshare Feed Specification (GBFS) auto-discovery feeds at mds.bird.co for 88+ cities across 12 countries (AT, BE, CA, CH, DE, ES, FI, FR, IL, IT, PT, US), and operates a private city-data portal at city-data.bird.co for credentialed municipal API access. There is no public consumer / 3rd-party developer API or SDK — the consumer surface is the iOS and Android Bird apps, the Bird Three product site, and the Bikeshare site. The undocumented mobile backend at api.birdapp.com / api-auth.prod.birdapp.com is well-documented in the community WoBike project but is not officially sanctioned for third-party use.

**Areas:** Micromobility · Shared Mobility · Electric Scooters · E-Scooter · E-Bikes · Bike Share · Transportation · Urban Mobility · GBFS · General Bikeshare Feed Specification · Mobility Data Specification · MDS

## Bird on APIs.io

Everything profiled for Bird is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/bird-rides/](https://apis.io/providers/bird-rides/)** — or go straight to one of the APIs or properties below.

### APIs (10)

- [Bird City Data Portal](https://apis.io/apis/bird-rides/bird-city-data-portal/) — Credentialed city / municipal data portal at https://city-data.bird.co providing partner cities with access to fleet, trip, and operational data feeds…
- [Bird Platform (Fleet Operator)](https://apis.io/apis/bird-rides/bird-platform-operator/) — Bird Platform is the white-label fleet operator program that lets independent local operators run a Bird-branded e-scooter service in their own market using…
- [Bird Mobile App Backend (Unofficial)](https://apis.io/apis/bird-rides/bird-mobile-app-api/) — The undocumented mobile-app backend that powers the Bird iOS and Android consumer apps. Hosts include api.birdapp.com, api-auth.prod.birdapp.com, and…
- [Bird Discovery API](https://apis.io/apis/bird-rides/bird-rides-discovery-api/) — GBFS auto-discovery and version metadata
- [Bird Geofencing API](https://apis.io/apis/bird-rides/bird-rides-geofencing-api/) — No-ride / no-parking polygon zones
- [Bird Pricing API](https://apis.io/apis/bird-rides/bird-rides-pricing-api/) — Rider-facing pricing plans
- [Bird Realtime API](https://apis.io/apis/bird-rides/bird-rides-realtime-api/) — Real-time feeds with 60-second TTL
- [Bird Stations API](https://apis.io/apis/bird-rides/bird-rides-stations-api/) — Docking-station information (mostly empty for free-floating Bird markets)
- [Bird System API](https://apis.io/apis/bird-rides/bird-rides-system-api/) — System-level information and regions
- [Bird Vehicles API](https://apis.io/apis/bird-rides/bird-rides-vehicles-api/) — Vehicle inventory and real-time availability

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Bird Rides Agentic Access](https://apis.io/agentic-access/bird-rides/bird-rides-agentic-access/)

#### JSON Schema (3)

The data models the API reads and writes.

- [Bird Geofencing Zone](https://apis.io/schemas/bird-rides/bird-geofencing-zone/)
- [Bird System Information](https://apis.io/schemas/bird-rides/bird-system-information/)
- [Bird Vehicle](https://apis.io/schemas/bird-rides/bird-vehicle/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Bird Rides Context](https://apis.io/jsonld/bird-rides/bird-rides-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Bird Vocabulary](https://apis.io/vocabularies/bird-rides/bird-rides-vocabulary/)

#### Examples (2)

Example requests and responses.

- [Bird System Information Example](https://apis.io/examples/bird-rides/bird-system-information-example/)
- [Bird Vehicle Types Example](https://apis.io/examples/bird-rides/bird-vehicle-types-example/)

#### Collections (8)

Postman and Open Collection request collections.

- [Bird GBFS Feed](https://apis.io/collections/bird-rides/open-bird-gbfs/)
- [Bird GBFS Feed Discovery API](https://apis.io/collections/bird-rides/open-bird-rides-discovery-api/)
- [Bird GBFS Feed Discovery Geofencing API](https://apis.io/collections/bird-rides/open-bird-rides-geofencing-api/)
- [Bird GBFS Feed Discovery Pricing API](https://apis.io/collections/bird-rides/open-bird-rides-pricing-api/)
- [Bird GBFS Feed Discovery Realtime API](https://apis.io/collections/bird-rides/open-bird-rides-realtime-api/)
- [Bird GBFS Feed Discovery Stations API](https://apis.io/collections/bird-rides/open-bird-rides-stations-api/)
- [Bird GBFS Feed Discovery System API](https://apis.io/collections/bird-rides/open-bird-rides-system-api/)
- [Bird GBFS Feed Discovery Vehicles API](https://apis.io/collections/bird-rides/open-bird-rides-vehicles-api/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Bird — jsonschema rules](https://apis.io/rules/bird-rides/bird-rides-jsonschema-spectral-rules/)

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Bird Rides Domain Security](https://apis.io/security/bird-rides/bird-rides-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Bird Rides Plans Pricing](https://apis.io/plans/bird-rides/bird-rides-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Bird Rides Rate Limits](https://apis.io/rate-limits/bird-rides/bird-rides-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Bird Rides Finops](https://apis.io/finops/bird-rides/bird-rides-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.bird.co)
- [Documentation](https://www.bird.co/how)
- [Support](https://help.bird.co)
- [Blog](https://www.bird.co/blog)
- [GitHub](https://github.com/birdrides)

## API Evangelist rating

**Kin Score 32.6** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 58.0 |
| Contract quality | 59.9 |
| Contract governance | 23.5 |
| Operational transparency | 2.6 |
| Developer ergonomics | 25.0 |
| Access clarity | 18.4 |

**Agent readiness 19.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | na |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | na |
| Error Semantics | — |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 14.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/bird-rides/](https://apis.io/providers/bird-rides/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Bird: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/bird-rides/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
