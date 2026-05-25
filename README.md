# US Census Bureau (us-census-bureau)
The U.S. Census Bureau is the federal statistical agency responsible for producing data about the American people and economy. Established in 1902 and part of the U.S. Department of Commerce, the Bureau conducts the constitutionally mandated Decennial Census every ten years and dozens of ongoing surveys including the American Community Survey, Economic Census, Population Estimates, Current Population Survey, and Survey of Income and Program Participation. The Census Bureau exposes its statistics through the Census Data API (over 1,700 datasets), the Microdata API for PUMS tabulation, the TIGERweb geospatial REST services, and the Geocoding Services API — all free, requiring only a free API key for the data endpoints and released into the public domain under CC0.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=government-api-evangelist&utm_content=repo)

## Tags

 - Government, Federal, Demographics, Statistics, Economics, Geospatial, Open Data, Public Sector

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Census Data API
Programmatic access to over 1,700 datasets including the American Community Survey (ACS), Decennial Census, Economic Census, Population Estimates, County Business Patterns, Nonemployer Statistics, Annual Business Survey, and Household Pulse Survey. Every endpoint follows `/data/{vintage}/{dataset-path}` and returns a 2-D JSON array. Requires a free `key` query parameter.

**Human URL:** [https://www.census.gov/data/developers/data-sets.html](https://www.census.gov/data/developers/data-sets.html)

**Base URL:** `https://api.census.gov/data`

- [Documentation — Datasets](https://www.census.gov/data/developers/data-sets.html)
- [Documentation — API User Guide](https://www.census.gov/data/developers/guidance/api-user-guide.html)
- [APICatalog — api.census.gov/data.json](https://api.census.gov/data.json)
- [OpenAPI](openapi/census-data-api-openapi.yml)
- [JSON Schema — Data Row](json-schema/census-data-row-schema.json)
- [JSON Schema — Dataset Metadata](json-schema/census-dataset-metadata-schema.json)
- [JSON Structure](json-structure/census-data-row-structure.json)
- [JSON-LD](json-ld/us-census-bureau-context.jsonld)
- [Example — ACS5 GET](examples/census-acs5-get-example.json)
- [Example — Discovery list](examples/census-discovery-list-example.json)
- [Spectral Rules](rules/census-data-api-rules.yml)
- [Naftiko Capability — Discovery](capabilities/census-data-api-datasets.yaml)
- [Naftiko Capability — Dataset Query](capabilities/census-data-api-query.yaml)

### Census Microdata API
Tabulate and query Public Use Microdata Sample (PUMS) records from the ACS, CPS, and SIPP using the same endpoint family with the PUMS-specific `tabulate`, `show`, and `recode` parameters.

**Human URL:** [https://www.census.gov/data/developers/guidance/microdata-api-user-guide.html](https://www.census.gov/data/developers/guidance/microdata-api-user-guide.html)

- [OpenAPI](openapi/census-microdata-api-openapi.yml)
- [Example — PUMS tabulate](examples/census-pums-tabulate-example.json)
- [Naftiko Capability — Microdata](capabilities/census-microdata-api-microdata.yaml)

### TIGERweb REST Services
ArcGIS REST services exposing the canonical TIGER/Line geographic boundary layers — states, counties, tracts, block groups, blocks, ZCTAs, congressional districts, school districts, PUMAs, and urban areas. Returns GeoJSON, Esri JSON, KML, or PBF. No API key required.

**Human URL:** [https://tigerweb.geo.census.gov/tigerwebmain/TIGERweb_apps.html](https://tigerweb.geo.census.gov/tigerwebmain/TIGERweb_apps.html)

- [OpenAPI](openapi/census-tigerweb-rest-openapi.yml)
- [Naftiko Capability — Features](capabilities/census-tigerweb-features.yaml)

### Census Geocoding Services API
Free address-to-coordinate and address-to-Census-geography geocoder. Supports one-line, structured, reverse, and batch (10,000 addresses per request). No API key required.

**Human URL:** [https://geocoding.geo.census.gov/geocoder/](https://geocoding.geo.census.gov/geocoder/)

- [OpenAPI](openapi/census-geocoder-api-openapi.yml)
- [Example — One-line address](examples/census-geocoder-onelineaddress-example.json)
- [Naftiko Capability — Geocoding](capabilities/census-geocoder-geocoding.yaml)

### Business Dynamics Statistics API
Annual measures of U.S. establishment births, deaths, expansions, contractions, job creation, and job destruction from 1978 to the latest reference year.

**Human URL:** [https://www.census.gov/data/developers/data-sets/business-dynamics.html](https://www.census.gov/data/developers/data-sets/business-dynamics.html)

- [OpenAPI](openapi/census-bds-api-openapi.yml)
- [Naftiko Capability — Time Series](capabilities/census-bds-timeseries.yaml)

### International Trade API
Monthly U.S. goods trade — imports, exports, balance, HS-coded commodity flows, port-level shipments, country and state-of-origin breakdowns — from 2010 to present.

**Human URL:** [https://www.census.gov/data/developers/data-sets/international-trade.html](https://www.census.gov/data/developers/data-sets/international-trade.html)

- [OpenAPI](openapi/census-international-trade-api-openapi.yml)
- [Naftiko Capability — Time Series](capabilities/census-international-trade-timeseries.yaml)

### Population Clock API
JSON feeds backing the U.S. and world Population Clocks. Public, no key required.

**Human URL:** [https://www.census.gov/popclock/](https://www.census.gov/popclock/)

- [OpenAPI](openapi/census-population-clock-api-openapi.yml)
- [Naftiko Capability — Clock](capabilities/census-population-clock-clock.yaml)

## Common Properties

- [Portal — census.gov](https://www.census.gov)
- [Documentation — Developer Portal](https://www.census.gov/data/developers.html)
- [Documentation — API User Guide](https://www.census.gov/data/developers/guidance/api-user-guide.html)
- [Documentation — Microdata API User Guide](https://www.census.gov/data/developers/guidance/microdata-api-user-guide.html)
- [APICatalog — api.census.gov/data.json](https://api.census.gov/data.json)
- [Documentation — Discovery Tool](https://www.census.gov/data/developers/updates/new-discovery-tool.html)
- [SignUp — Request an API Key](https://api.census.gov/data/key_signup.html)
- [TermsOfService](https://www.census.gov/data/developers/about/terms-of-service.html)
- [PrivacyPolicy](https://www.census.gov/about/policies/privacy.html)
- [GitHubOrganization — uscensusbureau](https://github.com/uscensusbureau)
- [SDK — CitySDK](https://github.com/uscensusbureau/citysdk)
- [Tool — Census Data API MCP Server](https://github.com/uscensusbureau/us-census-bureau-data-api-mcp)
- [Documentation — TIGER/Line](https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html)
- [Documentation — TIGERweb Apps](https://tigerweb.geo.census.gov/tigerwebmain/TIGERweb_apps.html)
- [Documentation — Geocoder Services](https://geocoding.geo.census.gov/geocoder/)
- [Documentation — data.census.gov Search](https://data.census.gov)
- [Documentation — data.gov Catalog Entry](https://catalog.data.gov/organization/census-gov)
- [Support — Ask Census](https://ask.census.gov)
- [Email — cnmp.developers.list@census.gov](mailto:cnmp.developers.list@census.gov)
- [License — Creative Commons CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/)
- [ChangeLog — Developer Updates](https://www.census.gov/data/developers/updates.html)
- [Blog — Director's blog](https://www.census.gov/newsroom/blogs/director.html)

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Census Data API](openapi/census-data-api-openapi.yml)
- [Census Microdata API](openapi/census-microdata-api-openapi.yml)
- [TIGERweb REST Services](openapi/census-tigerweb-rest-openapi.yml)
- [Census Geocoding Services API](openapi/census-geocoder-api-openapi.yml)
- [Business Dynamics Statistics API](openapi/census-bds-api-openapi.yml)
- [International Trade API](openapi/census-international-trade-api-openapi.yml)
- [Population Clock API](openapi/census-population-clock-api-openapi.yml)

### JSON Schema

- [Census Data Row](json-schema/census-data-row-schema.json)
- [Census Dataset Metadata](json-schema/census-dataset-metadata-schema.json)

### JSON Structure

- [Census Data Row](json-structure/census-data-row-structure.json)

### JSON-LD

- [US Census Bureau Context](json-ld/us-census-bureau-context.jsonld)

### Examples

- [ACS5 GET](examples/census-acs5-get-example.json)
- [Discovery list](examples/census-discovery-list-example.json)
- [PUMS tabulate](examples/census-pums-tabulate-example.json)
- [Geocoder one-line](examples/census-geocoder-onelineaddress-example.json)

### Capabilities (Naftiko)

- [Census Data API — Discovery](capabilities/census-data-api-datasets.yaml)
- [Census Data API — Query](capabilities/census-data-api-query.yaml)
- [Microdata — PUMS](capabilities/census-microdata-api-microdata.yaml)
- [TIGERweb — Features](capabilities/census-tigerweb-features.yaml)
- [Geocoder — Geocoding](capabilities/census-geocoder-geocoding.yaml)
- [BDS — Time Series](capabilities/census-bds-timeseries.yaml)
- [International Trade — Time Series](capabilities/census-international-trade-timeseries.yaml)
- [Population Clock](capabilities/census-population-clock-clock.yaml)

### Spectral

- [Census Data API Rules](rules/census-data-api-rules.yml)

### Vocabulary

- [US Census Bureau Vocabulary](vocabulary/us-census-bureau-vocabulary.yml)

### Rate limits

- [US Census Bureau Rate Limits](rate-limits/us-census-bureau-rate-limits.yml)

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
