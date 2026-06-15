# Sanity (sanity)

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
