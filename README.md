# TheFork (thefork)

TheFork is a leading European restaurant reservations marketplace, part of Tripadvisor, connecting diners with tens of thousands of restaurants across Europe and beyond. Through its developers portal, TheFork exposes a public REST API surface for restaurants, point-of-sale systems, and third-party partners to integrate with TheFork Management platform. The API enables partners to build custom booking flows, create and manage reservations with full detail such as meal date, party size, and customer data, surface preset menus and curated dining experiences, and access personalized guest data including allergies, dietary restrictions, and seating preferences. Offerings include a B2B API for restaurants and a POS API for point-of-sale providers.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Restaurant
- Reservations
- Booking
- Dining
- Point Of Sale
- Marketplace

## Timestamps

- **Created:** 2026-06-02
- **Modified:** 2026-06-03

## APIs

### TheFork B2B API

TheFork B2B API lets restaurants and groups integrate with TheFork Management platform. It supports designing custom booking flows, creating reservations with meal date, party size, and customer data, presenting preset menus, accessing personalized guest data such as allergies, dietary restrictions, and seating preferences, and retrieving guest reviews. The API is fronted by a Kong gateway and documented with OpenAPI 3. Authentication uses the Auth0 OAuth 2.0 client credentials flow to obtain a bearer access token.

- **Human URL:** [https://docs.thefork.io/B2B-API/introduction](https://docs.thefork.io/B2B-API/introduction)
- **Base URL:** `https://api.thefork.io`

#### Tags

- Reservations
- Booking
- Menus
- Guests
- Reviews

#### Properties

- [Documentation](https://docs.thefork.io/B2B-API/introduction)
- [API Reference](https://docs.thefork.io/B2B-API/API%20specifications/post-v-1-restaurants-id-reservations)
- [Getting Started](https://docs.thefork.io/getting-started)
- [Authentication](https://docs.thefork.io/B2B-API/authentication)
- [OpenAPI](openapi/thefork-b2b-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/thefork-b2b.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thefork-b2b.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/thefork-b2b-reservation-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/thefork-b2b-customer-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/thefork-b2b-review-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/thefork-b2b-reservation-structure.json)
- [J S O N- L D](json-ld/thefork-b2b-context.jsonld)
- [Example](examples/thefork-b2b-create-reservation-example.json)
- [Example](examples/thefork-b2b-get-reservation-example.json)
- [Example](examples/thefork-b2b-find-customer-by-phone-example.json)
- [Example](examples/thefork-b2b-get-review-example.json)

### TheFork POS API

TheFork POS API enables point-of-sale providers to integrate their systems with TheFork Management platform, synchronizing reservations and restaurant operations data. TheFork calls the POS provider's configured webhook endpoints (for example a receipt opening URL) to open orders when a diner is seated, then receives final order details such as total amount and currency back, marking reservations as left when payment completes. Authentication uses an API key supplied in the X-Api-Key header for requests to TheFork, and a bearer token for callbacks.

- **Human URL:** [https://docs.thefork.io/POS-API/how-it-works](https://docs.thefork.io/POS-API/how-it-works)

#### Tags

- Point Of Sale
- Reservations
- Orders

#### Properties

- [Documentation](https://docs.thefork.io/POS-API/how-it-works)
- [API Reference](https://docs.thefork.io/POS-API/Flow/create-order)
- [Getting Started](https://docs.thefork.io/getting-started)
- [Authentication](https://docs.thefork.io/preliminary-steps)
- [OpenAPI](openapi/thefork-pos-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/thefork-pos.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thefork-pos.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/thefork-pos-order-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/thefork-pos-order-structure.json)
- [Example](examples/thefork-pos-create-order-example.json)

## Common Properties

- [Website](https://www.thefork.com)
- [Documentation](https://docs.thefork.io/)
- [Portal](https://docs.thefork.io/)
- [Getting Started](https://docs.thefork.io/getting-started)
- [Sign Up](https://docs.thefork.io/preliminary-steps)
- [Terms of Service](https://docs.thefork.io/pdf/LaFourchette-Partners-API-Licence-2.pdf)
- [Blog](https://medium.com/thefork)
- [GitHub Organization](https://github.com/lafourchette)
- [Spectral Rules](rules/thefork-rules.yml)
- [Vocabulary](vocabulary/thefork-vocabulary.yml)
- [J S O N- L D](json-ld/thefork-context.jsonld)
- [Plans](plans/thefork-plans-pricing.yml)
- [Rate Limits](rate-limits/thefork-rate-limits.yml)
- [Fin Ops](finops/thefork-finops.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
