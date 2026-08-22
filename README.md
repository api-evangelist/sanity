# Sanity (sanity)

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

Sanity is a composable content platform providing a headless CMS with a real-time collaborative editor (Sanity Studio) and a powerful HTTP API for managing structured content. The Sanity Content Lake stores content as flexible documents queryable via GROQ (Graph-Relational Object Queries). Key API capabilities include document querying, mutations, real-time listening, asset management, project management, webhooks, scheduling, roles and permissions, vector embeddings, and AI-powered content agents.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/sanity/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/sanity/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Headless CMS
- Content Management
- GROQ
- Real-Time
- Structured Content
- Developer Platform

## Timestamps

- **Created:** 2026-05-02
- **Modified:** 2026-05-30

## APIs

### Sanity Query API

The Sanity Query API enables querying Content Lake documents using GROQ (Graph-Relational Object Queries). Supports GET for queries under 11 KB and POST for larger queries. Available at both the standard API endpoint and a CDN endpoint for edge-cached results. Supports perspectives (drafts, published), result source maps, and query explain functionality.

- **Human URL:** [https://www.sanity.io/docs/http-query](https://www.sanity.io/docs/http-query)

#### Tags

- GROQ
- Query
- Content Lake
- CDN

#### Properties

- [Documentation](https://www.sanity.io/docs/http-query)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/sanity/refs/heads/main/openapi/sanity-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [JSON Schema](json-schema/sanity-document-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/sanity-webhook-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Postman Collection](collections/sanity.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sanity.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sanity Mutation API

The Sanity Mutation API enables creating, updating, patching, and deleting documents in Content Lake. Mutations are submitted as arrays of operations (create, createOrReplace, createIfNotExists, patch, delete) against a dataset endpoint.

- **Human URL:** [https://www.sanity.io/docs/http-reference](https://www.sanity.io/docs/http-reference)

#### Tags

- Mutation
- Documents
- CRUD
- Content Lake

#### Properties

- [Documentation](https://www.sanity.io/docs/http-reference)
- [Postman Collection](collections/sanity.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sanity.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sanity Assets API

The Sanity Assets API handles uploading, retrieving, and managing file and image assets in Content Lake. Assets are stored as documents and referenced from content documents.

- **Human URL:** [https://www.sanity.io/docs/http-reference](https://www.sanity.io/docs/http-reference)

#### Tags

- Assets
- Images
- Files
- Upload

#### Properties

- [Documentation](https://www.sanity.io/docs/http-reference)
- [Postman Collection](collections/sanity.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sanity.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sanity Projects API

The Sanity Projects API enables programmatic management of Sanity projects including creating projects, managing datasets, configuring CORS origins, managing access tokens, and checking user permissions. Authentication uses Bearer tokens.

- **Human URL:** [https://www.sanity.io/docs/projects-api](https://www.sanity.io/docs/projects-api)

#### Tags

- Projects
- Datasets
- Access Control
- Tokens

#### Properties

- [Documentation](https://www.sanity.io/docs/projects-api)
- [Postman Collection](collections/sanity.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sanity.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sanity Webhooks API

The Sanity Webhooks API enables configuring event-driven notifications for content changes. Webhooks can be created to trigger on document create, update, delete, and publish events with customizable filter expressions.

- **Human URL:** [https://www.sanity.io/docs/http-reference](https://www.sanity.io/docs/http-reference)

#### Tags

- Webhooks
- Events
- Notifications
- Real-Time

#### Properties

- [Documentation](https://www.sanity.io/docs/http-reference)
- [Documentation](https://www.sanity.io/docs/webhooks)
- [AsyncAPI](https://raw.githubusercontent.com/api-evangelist/sanity/refs/heads/main/asyncapi/sanity-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/sanity.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sanity.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sanity Listen API

The Sanity Listen API provides real-time event streaming via Server-Sent Events (SSE) for content changes in a dataset. Clients can subscribe to a GROQ query and receive real-time notifications when matching documents change.

- **Human URL:** [https://www.sanity.io/docs/http-reference](https://www.sanity.io/docs/http-reference)

#### Tags

- Real-Time
- SSE
- Events
- Streaming

#### Properties

- [Documentation](https://www.sanity.io/docs/http-reference)
- [Postman Collection](collections/sanity.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sanity.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sanity Roles API

The Sanity Roles API provides endpoints for managing user roles and permissions within Sanity projects. Supports predefined roles (Administrator, Read+Write, Read, Viewer) and custom role management.

- **Human URL:** [https://www.sanity.io/docs/roles-reference](https://www.sanity.io/docs/roles-reference)

#### Tags

- Roles
- Permissions
- Access Control
- Security

#### Properties

- [Documentation](https://www.sanity.io/docs/roles-reference)
- [Postman Collection](collections/sanity.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sanity.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sanity Scheduling API

The Sanity Scheduling API enables scheduling content for future publication or unpublication at specific times, supporting editorial workflows and content calendars.

- **Human URL:** [https://www.sanity.io/docs/http-reference](https://www.sanity.io/docs/http-reference)

#### Tags

- Scheduling
- Publishing
- Content Calendar
- Workflow

#### Properties

- [Documentation](https://www.sanity.io/docs/http-reference)
- [Postman Collection](collections/sanity.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sanity.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sanity Embeddings Index API

The Sanity Embeddings Index API enables creating and managing vector embedding indexes for Content Lake documents, supporting semantic search and AI-powered content retrieval workflows.

- **Human URL:** [https://www.sanity.io/docs/http-reference](https://www.sanity.io/docs/http-reference)

#### Tags

- Embeddings
- Vector Search
- AI
- Semantic Search

#### Properties

- [Documentation](https://www.sanity.io/docs/http-reference)
- [Postman Collection](collections/sanity.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sanity.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [LinkedIn](https://www.linkedin.com/company/sanity-io)
- [Website](https://www.sanity.io)
- [Documentation](https://www.sanity.io/docs)
- [H T T P  A P I  Reference](https://www.sanity.io/docs/http-reference)
- [Developer  Portal](https://www.sanity.io/docs)
- [GitHub Organization](https://github.com/sanity-io)
- [Getting Started](https://www.sanity.io/docs/getting-started-with-sanity)
- [Java Script  S D K](https://www.npmjs.com/package/@sanity/client)
- [Pricing](https://www.sanity.io/pricing)
- [Community](https://slack.sanity.io)
- [Blog](https://www.sanity.io/blog)
- [Status Page](https://status.sanity.io)
- [Vocabulary](vocabulary/sanity-vocabulary.yml)
- [Spectral Rules](rules/sanity-rules.yml)
- [Capabilities](capabilities/content-management.yaml)
- [JSON-LD](json-ld/sanity-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [M C P Server](https://github.com/sanity-io/sanity-mcp-server)
- [Agent Skill](https://www.sanity.io/blog/introducing-sanity-agent-skills)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
