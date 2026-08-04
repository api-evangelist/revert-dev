# Revert (revert-dev)

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

Revert is an open-source unified API for building product integrations. A single normalized interface fronts many third-party SaaS providers across categories like CRM, with managed OAuth connections, a unified data model (contacts, leads, deals, companies, notes, tasks, events, users), a passthrough proxy for provider-specific calls, and webhooks. Revert is AGPL-3.0 licensed and self-hostable, with a hosted cloud offering.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/revert-dev/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/revert-dev/refs/heads/main/apis.yml)

## Authentication

- `x-revert-api-token` — your Revert API key (private token, used from your backend).
- `x-revert-t-id` — the unique customer/tenant id captured when a customer links their tool through Revert's managed OAuth flow.
- `x-api-version` — optional; the latest API version is used when omitted.

Base URL: `https://api.revert.dev` (unified CRM calls are under `https://api.revert.dev/crm`).

## Tags

- Unified API
- Integrations
- CRM
- iPaaS
- Open Source
- OAuth

## Timestamps

- **Created:** 2026-07-01
- **Modified:** 2026-07-01

## APIs

### Revert Connection API

Manage the connections a customer establishes to third-party tools through Revert's managed OAuth flow. Look up, list, and revoke connections keyed by tenant id (x-revert-t-id).

- **Human URL:** [https://docs.revert.dev/api-reference/api-reference/connection](https://docs.revert.dev/api-reference/api-reference/connection)
- **Base URL:** `https://api.revert.dev`

#### Tags

- Connections
- OAuth
- Integrations

#### Properties

- [Documentation](https://docs.revert.dev/api-reference/api-reference/connection)
- [API Reference](https://docs.revert.dev/api-reference/api-reference/connection)
- [OpenAPI](openapi/revert-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/revert-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/revert-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Revert Unified CRM Contacts API

Read, list, create, update, and search contacts across any connected CRM (Salesforce, HubSpot, Zoho, Pipedrive, Close, and more) using one normalized contact model.

- **Human URL:** [https://docs.revert.dev/api-reference/api-reference/crm/contact](https://docs.revert.dev/api-reference/api-reference/crm/contact)
- **Base URL:** `https://api.revert.dev/crm`

#### Tags

- CRM
- Contacts
- Unified API

#### Properties

- [Documentation](https://docs.revert.dev/api-reference/api-reference/crm/contact)
- [OpenAPI](openapi/revert-dev-openapi.yml)
- [Postman Collection](collections/revert-dev.postman_collection.json)
- [Open Collection](collections/revert-dev.opencollection.json)

### Revert Unified CRM Leads API

Read, list, create, update, and search leads across connected CRMs using Revert's unified lead schema.

- **Human URL:** [https://docs.revert.dev/api-reference/api-reference/crm/lead](https://docs.revert.dev/api-reference/api-reference/crm/lead)
- **Base URL:** `https://api.revert.dev/crm`

#### Tags

- CRM
- Leads
- Unified API

### Revert Unified CRM Deals API

Read, list, create, update, and search deals (opportunities) across connected CRMs using one normalized deal model.

- **Human URL:** [https://docs.revert.dev/api-reference/api-reference/crm/deal](https://docs.revert.dev/api-reference/api-reference/crm/deal)
- **Base URL:** `https://api.revert.dev/crm`

#### Tags

- CRM
- Deals
- Unified API

### Revert Unified CRM Companies API

Read, list, create, update, and search companies (accounts) across connected CRMs using Revert's unified company schema.

- **Human URL:** [https://docs.revert.dev/api-reference/api-reference/crm/company](https://docs.revert.dev/api-reference/api-reference/crm/company)
- **Base URL:** `https://api.revert.dev/crm`

#### Tags

- CRM
- Companies
- Accounts

### Revert Unified CRM Notes API

Read, list, create, and update notes attached to CRM records across connected CRMs.

- **Human URL:** [https://docs.revert.dev/api-reference/api-reference/crm/note](https://docs.revert.dev/api-reference/api-reference/crm/note)
- **Base URL:** `https://api.revert.dev/crm`

#### Tags

- CRM
- Notes
- Unified API

### Revert Unified CRM Tasks API

Read, list, create, and update tasks across connected CRMs using Revert's unified task model.

- **Human URL:** [https://docs.revert.dev/api-reference/api-reference/crm/task](https://docs.revert.dev/api-reference/api-reference/crm/task)
- **Base URL:** `https://api.revert.dev/crm`

#### Tags

- CRM
- Tasks
- Unified API

### Revert Unified CRM Events API

Read, list, create, and update calendar events / activities across connected CRMs using one normalized event model.

- **Human URL:** [https://docs.revert.dev/api-reference/api-reference/crm/event](https://docs.revert.dev/api-reference/api-reference/crm/event)
- **Base URL:** `https://api.revert.dev/crm`

#### Tags

- CRM
- Events
- Calendar

### Revert Unified CRM Users API

Read and list CRM users (record owners) across connected CRMs, useful for owner assignment and reference lookups.

- **Human URL:** [https://docs.revert.dev/api-reference/api-reference/crm/user](https://docs.revert.dev/api-reference/api-reference/crm/user)
- **Base URL:** `https://api.revert.dev/crm`

#### Tags

- CRM
- Users
- Owners

### Revert CRM Proxy (Passthrough) API

Passthrough proxy that forwards a raw request to the underlying connected provider's native API using Revert's managed OAuth token, so you can reach provider-specific endpoints not yet covered by the unified model.

- **Human URL:** [https://docs.revert.dev/api-reference/api-reference/crm/proxy](https://docs.revert.dev/api-reference/api-reference/crm/proxy)
- **Base URL:** `https://api.revert.dev/crm`

#### Tags

- Proxy
- Passthrough
- Escape Hatch

### Revert CRM Properties & Field Mapping API

List a connected CRM's available object properties and manage field mappings between provider custom fields and Revert's unified schema.

- **Human URL:** [https://docs.revert.dev/api-reference/api-reference/crm/properties](https://docs.revert.dev/api-reference/api-reference/crm/properties)
- **Base URL:** `https://api.revert.dev/crm`

#### Tags

- Properties
- Field Mapping
- Custom Fields

### Revert Metadata API

Retrieve integration metadata for an account, including the list of supported apps, their status, and the configuration needed to render Revert's connection UI.

- **Human URL:** [https://docs.revert.dev/api-reference/api-reference/metadata](https://docs.revert.dev/api-reference/api-reference/metadata)
- **Base URL:** `https://api.revert.dev`

#### Tags

- Metadata
- Integrations
- Catalog

### Revert Webhooks API

Register and manage webhook subscriptions so Revert can notify your backend when connection and record events happen across connected third-party tools.

- **Human URL:** [https://docs.revert.dev/api-reference/api-reference/webhook](https://docs.revert.dev/api-reference/api-reference/webhook)
- **Base URL:** `https://api.revert.dev`

#### Tags

- Webhooks
- Events
- Notifications

## Common Properties

- [GitHub Organization](https://github.com/revertinc)
- [LinkedIn](https://www.linkedin.com/company/revertdev)
- [Website](https://revert.dev)
- [Documentation](https://docs.revert.dev)
- [Plans](plans/revert-dev-plans-pricing.yml)
- [Rate Limits](rate-limits/revert-dev-rate-limits.yml)
- [Fin Ops](finops/revert-dev-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
