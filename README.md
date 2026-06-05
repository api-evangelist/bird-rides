# Bird (bird-rides)

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
