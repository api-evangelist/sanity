# Sanity

Sanity is a composable content platform providing a headless CMS with a real-time collaborative editor (Sanity Studio) and a powerful HTTP API for managing structured content. The Sanity Content Lake stores content as flexible documents queryable via GROQ (Graph-Relational Object Queries). Key capabilities include document querying, mutations, real-time event streaming, asset management, project management, webhooks, scheduling, roles and permissions, vector embeddings, and AI-powered content agents.

## APIs

### Sanity Query API
GROQ-based querying of Content Lake documents. Supports GET and POST, CDN caching, content perspectives, and result source maps.

- [Documentation](https://www.sanity.io/docs/http-query)
- [OpenAPI](openapi/sanity-openapi.yml)

### Sanity Mutation API
Create, update, patch, and delete documents in Content Lake as batched atomic operations.

- [Documentation](https://www.sanity.io/docs/http-reference)

### Sanity Projects API
Programmatic management of Sanity projects, datasets, CORS origins, access tokens, and permissions.

- [Documentation](https://www.sanity.io/docs/projects-api)

### Sanity Webhooks API
Event-driven notifications for content changes with GROQ filter expressions.

- [Documentation](https://www.sanity.io/docs/http-reference)

### Sanity Listen API
Real-time content change streaming via Server-Sent Events (SSE).

- [Documentation](https://www.sanity.io/docs/http-reference)

### Sanity Assets API
Upload and manage file and image assets in Content Lake.

- [Documentation](https://www.sanity.io/docs/http-reference)

### Sanity Roles API
Manage user roles and permissions for Sanity projects.

- [Documentation](https://www.sanity.io/docs/roles-reference)

### Sanity Scheduling API
Schedule content for future publication or unpublication.

- [Documentation](https://www.sanity.io/docs/http-reference)

### Sanity Embeddings Index API
Create and manage vector embedding indexes for semantic search workflows.

- [Documentation](https://www.sanity.io/docs/http-reference)

## Properties

| Type | URL |
|------|-----|
| Website | https://www.sanity.io |
| Documentation | https://www.sanity.io/docs |
| HTTP API Reference | https://www.sanity.io/docs/http-reference |
| GitHub Organization | https://github.com/sanity-io |
| JavaScript SDK | https://www.npmjs.com/package/@sanity/client |
| Community Slack | https://slack.sanity.io |
| Status | https://status.sanity.io |

## Artifacts

### OpenAPI Specifications
| Spec | Description |
|------|-------------|
| [Sanity OpenAPI](openapi/sanity-openapi.yml) | Core HTTP API spec covering Query, Mutations, Projects, Webhooks, Assets |

### Capabilities
| Capability | Description |
|------------|-------------|
| [Content Management](capabilities/content-management.yaml) | Unified content and project management workflows |

### Shared Capabilities
| Capability | Description |
|------------|-------------|
| [Sanity Content](capabilities/shared/sanity-content.yaml) | Content Lake query and mutation consumed definition |
| [Sanity Projects](capabilities/shared/sanity-projects.yaml) | Project and dataset management consumed definition |

### Schemas
| Schema | Description |
|--------|-------------|
| [Document Schema](json-schema/sanity-document-schema.json) | Base Content Lake document data model |
| [Webhook Schema](json-schema/sanity-webhook-schema.json) | Webhook configuration data model |

### Other Artifacts
| Artifact | Description |
|----------|-------------|
| [Document Structure](json-structure/sanity-document-structure.json) | Content Lake document field documentation |
| [JSON-LD Context](json-ld/sanity-context.jsonld) | Linked data context for Sanity concepts |
| [Vocabulary](vocabulary/sanity-vocabulary.yml) | Sanity platform domain vocabulary |
| [Rules](rules/sanity-rules.yml) | Spectral ruleset for API governance |

### Examples
| Example | Description |
|---------|-------------|
| [Query Documents](examples/sanity-query-documents-example.json) | GROQ query request/response example |
| [Mutate Documents](examples/sanity-mutate-documents-example.json) | Document mutation request/response example |
