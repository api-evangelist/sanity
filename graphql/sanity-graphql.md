# Sanity GraphQL API

Sanity provides a project-scoped GraphQL API that exposes Content Lake documents as a typed, queryable schema. The API is deployed per-project and per-dataset: you generate and deploy the schema from your Sanity Studio using the CLI (`sanity graphql deploy`), which introspects your studio's schema definitions and produces a GraphQL schema with PascalCase type names (e.g., a `bookAuthor` type becomes `BookAuthor`). For each document type in your schema, two root query fields are generated — `all<TypeName>` for list queries with filtering, sorting, and pagination, and `<TypeName>` for fetching a single document by its `_id`.

Requests are authenticated with a Sanity API token passed as a Bearer token in the `Authorization` header, or using a cookie-based session when querying from Sanity Studio. Read-only public datasets may be queried without authentication. Both a live API endpoint and a CDN-cached endpoint are available; the CDN endpoint provides lower latency for published content at the cost of slight eventual consistency. Queries support a `perspective` argument to control whether drafts, published, or raw documents are returned.

The built-in schema includes a set of system object types — `SanityImageAsset`, `SanityFileAsset`, `SanityImageMetadata`, `SanityImageDimensions`, `SanityImageHotspot`, `SanityImageCrop`, `SanityImagePalette`, `SanityImagePaletteSwatch`, `SanityAssetSourceData`, `Geopoint`, and `Slug` — that are always present regardless of project schema. Portable Text fields are exposed as a `<fieldName>Raw` JSON scalar to preserve the full block structure. Filter input types are generated per object and document type, supporting comparators such as `eq`, `neq`, `gt`, `gte`, `lt`, `lte`, `in`, `nin`, and `matches` depending on field scalar type.

**Endpoint:** `https://{projectId}.api.sanity.io/v2025-02-19/graphql/{dataset}/default`

**CDN Endpoint:** `https://{projectId}.apicdn.sanity.io/v2025-02-19/graphql/{dataset}/default`

**Documentation:** https://www.sanity.io/docs/graphql

**References:**
- Documentation: https://www.sanity.io/docs/graphql
- GettingStarted: https://www.sanity.io/docs/getting-started-with-sanity
