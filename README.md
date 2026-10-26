# Bird (bird-rides)

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

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/bird-rides/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/bird-rides/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- Micromobility
- Shared Mobility
- Electric Scooters
- E-Scooters
- E-Bikes
- Bikeshare
- Transportation
- Urban Mobility
- GBFS
- General Bikeshare Feed Specification
- Mobility Data Specification
- MDS
- Geofencing
- Cities
- Smart Cities
- Fleet Management
- Third Lane Mobility

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Bird GBFS Feed

Bird's public General Bikeshare Feed Specification (GBFS) v2.3 auto-discovery feeds. Each city has its own auto-discovery document at https://mds.bird.co/gbfs/v2/public/{city}/gbfs.json that links to nine sub-feeds — system_information, vehicle_types, free_bike_status, station_information, station_status, geofencing_zones, system_pricing_plans, system_regions, and gbfs_versions — with a 60-second TTL. As of this profile Bird publishes feeds for 88 cities across Austria, Belgium, Canada, Switzerland, Germany, Spain, Finland, France, Israel, Italy, Portugal, and the United States. The feeds are free to consume under the GBFS Data License Agreement at https://www.bird.co/wp-content/uploads/2019/03/GBFS-Data-License-Agreement-2018-09-25.pdf, and they expose real-time vehicle locations, battery levels, vehicle types (scooter and electric-assist bicycle), no-ride and no-parking geofencing polygons, pricing plans, and service regions for every Bird market.

- **Human URL:** [https://github.com/MobilityData/gbfs](https://github.com/MobilityData/gbfs)
- **Base URL:** `https://mds.bird.co/gbfs/v2/public/{city}`

#### Tags

- GBFS
- Micromobility
- Real-time
- Geofencing
- Vehicle Locations

#### Properties

- [Documentation](https://github.com/MobilityData/gbfs/blob/master/gbfs.md)
- [Discovery](https://mds.bird.co/gbfs/v2/public/los-angeles/gbfs.json)
- [License](https://www.bird.co/wp-content/uploads/2019/03/GBFS-Data-License-Agreement-2018-09-25.pdf)
- [OpenAPI](openapi/bird-gbfs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bird-gbfs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bird-gbfs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/bird-vehicle-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/bird-system-information-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/bird-geofencing-zone-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/bird-rides-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/bird-system-information-example.json)
- [Examples](examples/bird-vehicle-types-example.json)
- [Vocabulary](vocabulary/bird-rides-vocabulary.yml)

### Bird City Data Portal

Credentialed city / municipal data portal at https://city-data.bird.co providing partner cities with access to fleet, trip, and operational data feeds beyond the public GBFS surface. Access is granted to municipal staff and authorized researchers under a data-sharing agreement; credentials are requested directly from Bird's government partnerships team (city@bird.co; benelux@bird.co for EMEA). Bird markets this surface as the "in-depth APIs" that let cities analyze micromobility trends and measure infrastructure impact. The portal is not a public developer API and there is no published OpenAPI definition.

- **Human URL:** [https://city-data.bird.co/login](https://city-data.bird.co/login)

#### Tags

- Cities
- Government
- Municipal
- MDS
- Compliance
- Trip Data

#### Properties

- [Portal](https://city-data.bird.co/login)
- [Documentation](https://www.bird.co/cities)
- [Contact](mailto:city@bird.co)
- [Contact](mailto:benelux@bird.co)
- [Postman Collection](collections/bird-gbfs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bird-gbfs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bird Platform (Fleet Operator)

Bird Platform is the white-label fleet operator program that lets independent local operators run a Bird-branded e-scooter service in their own market using Bird vehicles, the Bird consumer app, and a Bird-hosted real-time data dashboard with geospatial tooling, historic analytics, and GovTech compliance features. Vehicles are sold at cost with a minimum order of 50 units, and Bird charges a revenue-share service fee per ride. The platform is invitation / qualification based and does not publish a developer API surface — operators interact via the hosted dashboard.

- **Human URL:** [https://www.bird.co/platform](https://www.bird.co/platform)

#### Tags

- Fleet Operator
- White Label
- Dashboard
- Operations

#### Properties

- [Portal](https://www.bird.co/platform)
- [Documentation](https://www.bird.co/us-fm)
- [Documentation](https://www.bird.co/us-op)
- [Postman Collection](collections/bird-gbfs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bird-gbfs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bird Mobile App Backend (Unofficial)

The undocumented mobile-app backend that powers the Bird iOS and Android consumer apps. Hosts include api.birdapp.com, api-auth.prod.birdapp.com, and api-bird.prod.birdapp.com. The surface is email + magic-link authentication, JWT access / refresh tokens (24-hour TTL), and endpoints for nearby vehicles, configuration, and ride lifecycle. The surface is reverse-engineered and documented in the community-maintained WoBike project but is NOT a sanctioned third-party API — there is no developer portal, no rate-limit documentation, no terms of service for programmatic use, and access can change without notice. Listed here for completeness and transparency, not as a recommended integration target.

- **Human URL:** [https://github.com/ubahnverleih/WoBike/blob/master/Bird.md](https://github.com/ubahnverleih/WoBike/blob/master/Bird.md)
- **Base URL:** `https://api.birdapp.com`

#### Tags

- Mobile
- Unofficial
- Reverse Engineered
- Consumer

#### Properties

- [Documentation](https://github.com/ubahnverleih/WoBike/blob/master/Bird.md)
- [Documentation](https://sharedmobility.github.io/Bird.html)
- [Postman Collection](collections/bird-gbfs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bird-gbfs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.bird.co)
- [Product](https://three.bird.co)
- [Product](https://bikeshare.bird.co)
- [Documentation](https://www.bird.co/how)
- [Map](https://www.bird.co/map)
- [Safety](https://www.bird.co/safety)
- [Sustainability](https://www.bird.co/sustainability)
- [Support](https://help.bird.co)
- [Cities](https://www.bird.co/cities)
- [Platform](https://www.bird.co/platform)
- [Fleet Manager](https://www.bird.co/us-fm)
- [Operator Partner](https://www.bird.co/us-op)
- [About](https://www.bird.co/about)
- [Careers](https://www.bird.co/careers)
- [Contact](https://www.bird.co/contact-us)
- [Press](https://www.bird.co/press)
- [Blog](https://www.bird.co/blog)
- [Investor Relations](https://ir.bird.co)
- [Terms](https://www.bird.co/terms)
- [Privacy](https://www.bird.co/privacy)
- [License](https://www.bird.co/wp-content/uploads/2019/03/GBFS-Data-License-Agreement-2018-09-25.pdf)
- [App Store](https://apps.apple.com/us/app/bird-be-free-enjoy-the-ride/id1260842311)
- [Play Store](https://play.google.com/store/apps/details?id=co.bird.android)
- [GitHub Organization](https://github.com/birdrides)
- [GitHub Organization](https://github.com/thirdlanemobility)
- [Parent Company](https://www.thirdlanemobility.com)
- [Sister Brand](https://www.spin.app)
- [Twitter](https://twitter.com/birdride)
- [Instagram](https://www.instagram.com/bird)
- [LinkedIn](https://www.linkedin.com/company/bird-rides)
- [Wikipedia](https://en.wikipedia.org/wiki/Bird_Global)
- [Plans](plans/bird-rides-plans-pricing.yml)
- [Rate Limits](rate-limits/bird-rides-rate-limits.yml)
- [Fin Ops](finops/bird-rides-finops.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
**URL:** https://apievangelist.com
