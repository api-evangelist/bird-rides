# bird-rides

Bird — shared electric scooters and bikes, operating as the global anchor brand of Third Lane Mobility, Inc.

This api-evangelist profile catalogs Bird's public API surface (GBFS feeds for 88+ cities across 12 countries), its credentialed city-data portal, the Bird Platform fleet operator program, and the reverse-engineered consumer mobile backend.

## What is in this repo

- `apis.yml` — APIs.json profile of the four Bird API surfaces (GBFS, City Data Portal, Bird Platform, mobile-app backend) plus company, parent, and sister-brand links.
- `openapi/bird-gbfs-openapi.yml` — OpenAPI 3.1 description of Bird's public GBFS v2.3 surface at `https://mds.bird.co/gbfs/v2/public/{city}`.
- `json-schema/` — JSON Schemas for Bird vehicles, system information, and geofencing zones.
- `json-ld/bird-rides-context.jsonld` — JSON-LD context mapping Bird's GBFS terms to schema.org, GeoJSON, and WGS84 vocabularies.
- `examples/` — Captured GBFS sample responses (system_information, vehicle_types) from the Los Angeles feed.
- `vocabulary/bird-rides-vocabulary.yml` — Operational vocabulary for Bird's micromobility surface.
- `review.yml` — Tier-1 review of Bird's API surface, strengths, and gaps.

## Quick links

- Website: https://www.bird.co
- GBFS auto-discovery (Los Angeles example): https://mds.bird.co/gbfs/v2/public/los-angeles/gbfs.json
- Cities partner program: https://www.bird.co/cities
- City data portal (credentialed): https://city-data.bird.co/login
- Bird Platform (fleet operators): https://www.bird.co/platform
- Parent company: Third Lane Mobility, Inc.
- Sister brand: Spin

## Status

Bird emerged from Chapter 11 bankruptcy in April 2024 under the new private parent Third Lane Mobility, Inc. (which also owns Spin, acquired from TIER in September 2023). Together they form the largest micromobility operator in North America with 200,000+ vehicles in 350+ cities.
