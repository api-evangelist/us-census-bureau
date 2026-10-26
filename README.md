# US Census Bureau (us-census-bureau)

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

The U.S. Census Bureau is the federal statistical agency responsible for producing data about the American people and economy. Established in 1902 and part of the U.S. Department of Commerce, the Bureau conducts the constitutionally mandated Decennial Census every ten years and dozens of ongoing surveys including the American Community Survey, Economic Census, Population Estimates, Current Population Survey, and Survey of Income and Program Participation. The Census Bureau exposes its statistics through the Census Data API (over 1,700 datasets), the Microdata API for PUMS tabulation, the TIGERweb geospatial REST services, and the Geocoding Services API — all free, requiring only a free API key for the data endpoints and released into the public domain under CC0.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/apis.yml)

## Scope

- **Position:** Producing
- **Access:** 3rd-Party

## Tags

- Government
- Federal
- Demographics
- Statistics
- Economics
- Geospatial
- Open Data
- Public Sector

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Census Data API

Programmatic access to over 1,700 Census Bureau datasets including the American Community Survey (ACS), Decennial Census, Economic Census, Population Estimates, Annual Business Survey, County Business Patterns, Nonemployer Statistics, Household Pulse Survey, and more. All endpoints follow the pattern `/data/{vintage}/{dataset}` and return a 2D JSON array (header row + value rows). API key required via the `key` query parameter.

- **Human URL:** [https://www.census.gov/data/developers/data-sets.html](https://www.census.gov/data/developers/data-sets.html)
- **Base URL:** `https://api.census.gov/data`

#### Tags

- Government
- Demographics
- Statistics
- Open Data

#### Properties

- [Documentation](https://www.census.gov/data/developers/data-sets.html)
- [Documentation](https://www.census.gov/data/developers/guidance/api-user-guide.html)
- [A P I Catalog](https://api.census.gov/data.json)
- [Documentation](https://api.census.gov/data.html)
- [OpenAPI](openapi/census-data-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/census-data-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/census-data-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/census-data-row-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/census-dataset-metadata-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/census-data-row-structure.json)
- [JSON-LD](json-ld/us-census-bureau-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Example](examples/census-acs5-get-example.json)
- [Example](examples/census-discovery-list-example.json)
- [Spectral Rules](rules/census-data-api-rules.yml) — [Spectral](https://docs.stoplight.io/docs/spectral)

### Census Microdata API

Tabulate and query Public Use Microdata Sample (PUMS) records across the American Community Survey, Current Population Survey, and Survey of Income and Program Participation. Supports custom tabulations across record-level person and household data using the same `/data/{vintage}/{dataset}` endpoint family with PUMS-specific `tabulate=`, `show=`, and recoding parameters.

- **Human URL:** [https://www.census.gov/data/developers/guidance/microdata-api-user-guide.html](https://www.census.gov/data/developers/guidance/microdata-api-user-guide.html)
- **Base URL:** `https://api.census.gov/data`

#### Tags

- Government
- Microdata
- Statistics
- PUMS

#### Properties

- [Documentation](https://www.census.gov/data/developers/guidance/microdata-api-user-guide.html)
- [OpenAPI](openapi/census-microdata-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/census-microdata-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/census-microdata-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/census-pums-tabulate-example.json)

### TIGERweb REST Services

ArcGIS REST services exposing the canonical Census TIGER/Line geographic boundary layers — states, counties, tracts, block groups, blocks, ZIP Code Tabulation Areas, congressional districts, school districts, Public Use Microdata Areas, urban areas, and more. Returns GeoJSON, Esri JSON, KML, and PBF. No API key required.

- **Human URL:** [https://tigerweb.geo.census.gov/tigerwebmain/TIGERweb_apps.html](https://tigerweb.geo.census.gov/tigerwebmain/TIGERweb_apps.html)
- **Base URL:** `https://tigerweb.geo.census.gov/arcgis/rest/services`

#### Tags

- Government
- Geospatial
- GIS
- Boundaries
- Mapping

#### Properties

- [Documentation](https://tigerweb.geo.census.gov/tigerwebmain/TIGERweb_apps.html)
- [Portal](https://tigerweb.geo.census.gov/arcgis/rest/services)
- [OpenAPI](openapi/census-tigerweb-rest-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/census-tigerweb-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/census-tigerweb-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Census Geocoding Services API

Free geocoding service that turns addresses into geographic coordinates and Census geographies (state, county, tract, block, congressional district, school district). Supports one-line address parsing, structured address parsing, address batch geocoding, coordinate reverse geocoding, and benchmark selection (current, 2020, 2010). No API key required.

- **Human URL:** [https://geocoding.geo.census.gov/geocoder/](https://geocoding.geo.census.gov/geocoder/)
- **Base URL:** `https://geocoding.geo.census.gov/geocoder`

#### Tags

- Government
- Geocoding
- Addresses
- GIS

#### Properties

- [Portal](https://geocoding.geo.census.gov/geocoder/)
- [Documentation](https://geocoding.geo.census.gov/geocoder/Geocoding_Services_API.html)
- [OpenAPI](openapi/census-geocoder-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/census-geocoder-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/census-geocoder-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/census-geocoder-onelineaddress-example.json)

### Business Dynamics Statistics API

Time series API covering U.S. business establishment births, deaths, job creation, and job destruction from 1978 to the latest reference year. Supports breakdowns by firm age, firm size, sector, state, and metro area via the `/data/timeseries/bds` endpoint.

- **Human URL:** [https://www.census.gov/data/developers/data-sets/business-dynamics.html](https://www.census.gov/data/developers/data-sets/business-dynamics.html)
- **Base URL:** `https://api.census.gov/data/timeseries/bds`

#### Tags

- Government
- Economics
- Business
- Employment

#### Properties

- [Documentation](https://www.census.gov/data/developers/data-sets/business-dynamics.html)
- [OpenAPI](openapi/census-bds-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/census-bds-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/census-bds-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### International Trade API

Monthly U.S. international goods trade — imports, exports, balance of trade, port-level shipments, HS-coded commodity flows, country-of-origin/destination — from 2010 to present. Endpoint family `/data/timeseries/intltrade/{exports|imports}/{hs|porths|stateports|...}`.

- **Human URL:** [https://www.census.gov/data/developers/data-sets/international-trade.html](https://www.census.gov/data/developers/data-sets/international-trade.html)
- **Base URL:** `https://api.census.gov/data/timeseries/intltrade`

#### Tags

- Government
- Trade
- Economics
- Imports
- Exports

#### Properties

- [Documentation](https://www.census.gov/data/developers/data-sets/international-trade.html)
- [OpenAPI](openapi/census-international-trade-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/census-international-trade-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/census-international-trade-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Population Clock API

JSON-feed driving the U.S. and world Population Clock — current population estimates plus estimated time intervals for births, deaths, and net international migration. Public, no key required.

- **Human URL:** [https://www.census.gov/popclock/](https://www.census.gov/popclock/)
- **Base URL:** `https://www.census.gov/popclock/data`

#### Tags

- Government
- Demographics
- Real Time

#### Properties

- [Portal](https://www.census.gov/popclock/)
- [OpenAPI](openapi/census-population-clock-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/census-population-clock-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/census-population-clock-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://www.census.gov)
- [Documentation](https://www.census.gov/data/developers.html)
- [Documentation](https://www.census.gov/data/developers/about.html)
- [Documentation](https://www.census.gov/data/developers/guidance/api-user-guide.html)
- [Documentation](https://www.census.gov/data/developers/guidance/microdata-api-user-guide.html)
- [A P I Catalog](https://api.census.gov/data.json)
- [Documentation](https://www.census.gov/data/developers/updates/new-discovery-tool.html)
- [Sign Up](https://api.census.gov/data/key_signup.html)
- [Sign Up](https://www.census.gov/data/developers/api-key.html)
- [Terms of Service](https://www.census.gov/data/developers/about/terms-of-service.html)
- [Privacy Policy](https://www.census.gov/about/policies/privacy.html)
- [Blog](https://www.census.gov/newsroom/blogs/director.html)
- [Changelog](https://www.census.gov/data/developers/updates.html)
- [GitHub Organization](https://github.com/uscensusbureau)
- [SDK](https://github.com/uscensusbureau/citysdk)
- [Tool](https://github.com/uscensusbureau/us-census-bureau-data-api-mcp)
- [Tool](https://api.census.gov/data.html)
- [Documentation](https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html)
- [Documentation](https://tigerweb.geo.census.gov/tigerwebmain/TIGERweb_apps.html)
- [Documentation](https://geocoding.geo.census.gov/geocoder/)
- [Documentation](https://data.census.gov)
- [Forum](https://www.data.gov/)
- [Documentation](https://catalog.data.gov/organization/census-gov)
- [Support](https://ask.census.gov)
- [Contact Form](https://ask.census.gov/prweb/PRServletCustom/app/ECORRAsk/YACFBFye-rFIz_FoGtyvDRUGg1Uzu5Mn*/!STANDARD)
- [Email](mailto:cnmp.developers.list@census.gov)
- [License](https://creativecommons.org/publicdomain/zero/1.0/)
- [Rate Limits](rate-limits/us-census-bureau-rate-limits.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
