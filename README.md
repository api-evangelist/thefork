# TheFork (thefork)
TheFork is a leading European restaurant reservations marketplace, part of Tripadvisor, connecting diners with tens of thousands of restaurants across Europe and beyond. Through its developers portal, TheFork exposes a public REST API surface for restaurants, point-of-sale systems, and third-party partners to integrate with TheFork Management platform. The API enables partners to build custom booking flows, create and manage reservations with full detail such as meal date, party size, and customer data, surface preset menus and curated dining experiences, and access personalized guest data including allergies, dietary restrictions, and seating preferences. Offerings include a B2B API for restaurants and a POS API for point-of-sale providers.

**URL:** [Visit APIs.json URL](https://docs.thefork.io/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Restaurant, Reservations, Booking, Dining, Point Of Sale, Marketplace

## Timestamps

- **Created:** 2026-06-02
- **Modified:** 2026-06-03

## APIs

### TheFork B2B API
TheFork B2B API lets restaurants and groups integrate with TheFork Management platform. It supports designing custom booking flows, creating reservations with meal date, party size, and customer data, presenting preset menus, accessing personalized guest data such as allergies, dietary restrictions, and seating preferences, and retrieving guest reviews. The API is fronted by a Kong gateway and documented with OpenAPI 3. Authentication uses the Auth0 OAuth 2.0 client credentials flow to obtain a bearer access token.

**Human URL:** [https://docs.thefork.io/B2B-API/introduction](https://docs.thefork.io/B2B-API/introduction)

#### Tags:

 - Reservations, Booking, Menus, Guests, Reviews

#### Properties

- [Documentation](https://docs.thefork.io/B2B-API/introduction)
- [APIReference](https://docs.thefork.io/B2B-API/API%20specifications/post-v-1-restaurants-id-reservations)
- [GettingStarted](https://docs.thefork.io/getting-started)
- [Authentication](https://docs.thefork.io/B2B-API/authentication)
- [OpenAPI](openapi/thefork-b2b-openapi.yml)
- [JSONSchema](json-schema/thefork-b2b-reservation-schema.json)
- [JSONSchema](json-schema/thefork-b2b-customer-schema.json)
- [JSONSchema](json-schema/thefork-b2b-review-schema.json)
- [JSONStructure](json-structure/thefork-b2b-reservation-structure.json)
- [JSON-LD](json-ld/thefork-b2b-context.jsonld)
- [Example](examples/thefork-b2b-create-reservation-example.json)
- [Example](examples/thefork-b2b-get-reservation-example.json)
- [Example](examples/thefork-b2b-find-customer-by-phone-example.json)
- [Example](examples/thefork-b2b-get-review-example.json)

### TheFork POS API
TheFork POS API enables point-of-sale providers to integrate their systems with TheFork Management platform, synchronizing reservations and restaurant operations data. TheFork calls the POS provider's configured webhook endpoints (for example a receipt opening URL) to open orders when a diner is seated, then receives final order details such as total amount and currency back, marking reservations as left when payment completes. Authentication uses an API key supplied in the X-Api-Key header for requests to TheFork, and a bearer token for callbacks.

**Human URL:** [https://docs.thefork.io/POS-API/how-it-works](https://docs.thefork.io/POS-API/how-it-works)

#### Tags:

 - Point Of Sale, Reservations, Orders

#### Properties

- [Documentation](https://docs.thefork.io/POS-API/how-it-works)
- [APIReference](https://docs.thefork.io/POS-API/Flow/create-order)
- [GettingStarted](https://docs.thefork.io/getting-started)
- [Authentication](https://docs.thefork.io/preliminary-steps)
- [OpenAPI](openapi/thefork-pos-openapi.yml)
- [JSONSchema](json-schema/thefork-pos-order-schema.json)
- [JSONStructure](json-structure/thefork-pos-order-structure.json)
- [Example](examples/thefork-pos-create-order-example.json)

## Common Properties

- [Website](https://www.thefork.com)
- [Documentation](https://docs.thefork.io/)
- [Portal](https://docs.thefork.io/)
- [GettingStarted](https://docs.thefork.io/getting-started)
- [SignUp](https://docs.thefork.io/preliminary-steps)
- [TermsOfService](https://docs.thefork.io/pdf/LaFourchette-Partners-API-Licence-2.pdf)
- [Blog](https://medium.com/thefork)
- [GitHubOrganization](https://github.com/lafourchette)
- [SpectralRules](rules/thefork-rules.yml)
- [Vocabulary](vocabulary/thefork-vocabulary.yml)
- [JSON-LD](json-ld/thefork-context.jsonld)
- [Plans](plans/thefork-plans-pricing.yml)
- [RateLimits](rate-limits/thefork-rate-limits.yml)
- [FinOps](finops/thefork-finops.yml)

## Features

| Name | Description |
|------|-------------|
| Custom Booking Funnel | Build a custom booking flow with real-time availability, offers, and preset menus, then create reservations directly against a restaurant. |
| Reservation Management | Create, retrieve, and update reservations including meal date, party size, and customer data. |
| Guest Profiles | Access personalized guest data such as allergies, intolerances, dietary restrictions, and seating preferences. |
| Customer Lookup | Find customer details by phone number for a given restaurant. |
| Reviews | Retrieve guest review details by review UUID. |
| Asynchronous Data Sync | Synchronize data without requiring real-time updates, using webhooks for reservation created and updated events. |
| POS Order Sync | Open and close point-of-sale orders tied to reservations and sync final amounts back to TheFork Management. |

## Use Cases

| Name | Description |
|------|-------------|
| Restaurant Booking Integration | Restaurants and groups embed TheFork availability and booking into their own websites and apps. |
| POS Integration | Point-of-sale vendors connect their systems to reflect seated guests, open tickets, and reconcile spend with reservations. |
| Guest Personalization | Use allergy, dietary, and seating preferences to personalize the dining experience and pre-service preparation. |
| Review Aggregation | Pull guest reviews into restaurant CRM and reputation tooling. |

## Integrations

| Name | Description |
|------|-------------|
| TheFork Management (TFM) | The restaurant management platform the APIs synchronize with. |
| Tripadvisor | Parent company; TheFork is part of the Tripadvisor group. |
| Auth0 | Identity provider issuing OAuth 2.0 client credentials tokens. |
| Kong | API gateway fronting the public API with auth, rate limiting, and IP allowlisting. |

## Solutions

| Name | Description |
|------|-------------|
| For Restaurants | B2B API for restaurants and groups to manage bookings and guests. |
| For POS Providers | POS API for point-of-sale vendors to sync orders and reservations. |
| For Partners | Partner API for third-party partners (announced as available soon). |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [TheFork B2B API](openapi/thefork-b2b-openapi.yml)
- [TheFork POS API](openapi/thefork-pos-openapi.yml)

### JSON Schema

- 15 schema files in [json-schema/](json-schema/) covering reservations, customers, reviews, orders, and supporting types.

### JSON Structure

- [TheFork B2B Reservation](json-structure/thefork-b2b-reservation-structure.json)
- [TheFork POS Order](json-structure/thefork-pos-order-structure.json)

### JSON-LD

- [TheFork Context](json-ld/thefork-context.jsonld)
- [TheFork B2B Context](json-ld/thefork-b2b-context.jsonld)
- [TheFork POS Context](json-ld/thefork-pos-context.jsonld)

### Examples

- 5 request/response examples in [examples/](examples/).

## Capabilities

Naftiko capabilities organized as self-contained per-tag definitions, each exposing both a REST and an MCP adapter.

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Reservations](capabilities/b2b-reservations.yaml) | TheFork B2B API | 3 | Restaurant Integrator |
| [Customers](capabilities/b2b-customers.yaml) | TheFork B2B API | 2 | Restaurant Integrator |
| [Reviews](capabilities/b2b-reviews.yaml) | TheFork B2B API | 1 | Restaurant Integrator |
| [Orders](capabilities/pos-orders.yaml) | TheFork POS API | 2 | POS Provider |

## Vocabulary

- [TheFork Vocabulary](vocabulary/thefork-vocabulary.yml) — Unified taxonomy mapping 4 resources, 7 actions, 4 workflows, and 2 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [TheFork Spectral Rules](rules/thefork-rules.yml) — 11 rules enforcing TheFork API conventions (HTTPS hosts, kebab-case paths, camelCase properties, Title Case tags and summaries, security schemes)

## Commercial

- [Plans & Pricing](plans/thefork-plans-pricing.yml) — Contract-based partner access model
- [Rate Limits](rate-limits/thefork-rate-limits.yml) — Kong gateway, contract-defined per-partner limits
- [FinOps](finops/thefork-finops.yml) — FOCUS-aligned billing view

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
