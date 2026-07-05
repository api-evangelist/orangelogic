# Orange Logic (orangelogic)

Orange Logic builds OrangeDAM (formerly branded Cortex), an enterprise digital asset management (DAM) and media asset management (MAM) platform used by museums, media companies, financial institutions, healthcare, government, and non-profit archives. OrangeDAM exposes a documented REST API for assets, metadata, search, users, folders, and webhooks.

**Access model:** The Orange Logic API is per-instance and customer-gated. Every call is made against your own organization's Orange Logic instance host rather than a single shared public gateway, so base URLs are written throughout this catalog as the placeholder `https://{OrangeLogicURL}/webapi` (or `https://{OrangeLogicURL}/API` for legacy paths). You need an OrangeDAM instance and credentials to exercise the API. The reference documentation itself, however, is public at [developer.orangelogic.com](https://developer.orangelogic.com).

**Endpoint families:** Newer `/webapi/` endpoints each end in a unique identifier and version (for example `token_48I_v1`); legacy `/api/` endpoints carry a version number in the path. Orange Logic recommends the `/webapi/` family where both exist. Responses are returned as JSON or XML.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/orangelogic/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/orangelogic/refs/heads/main/apis.yml)

## Tags

- Digital Asset Management
- DAM
- Media Asset Management
- MAM
- Enterprise
- Metadata
- Archive

## Timestamps

- **Created:** 2026-07-05
- **Modified:** 2026-07-05

## APIs

### Orange Logic Authentication API

Authenticate against an Orange Logic instance and obtain tokens for subsequent calls. Supports OAuth 2.0 (client ID and secret), non-expiring bearer tokens, and basic username/password login. The OAuth token endpoint returns an access token valid for 24 hours and a refresh token valid for 30 days. Confirmed paths include `POST /webapi/security/oauth2/token_48I_v1` and `/webapi/security/clientcredentialsauthentication/authenticate_46H_v1`.

- **Human URL:** [https://developer.orangelogic.com/reference/authentication-endpoints](https://developer.orangelogic.com/reference/authentication-endpoints)
- **Base URL:** `https://{OrangeLogicURL}/webapi`

### Orange Logic Search API

Find assets with query criteria, field selection, pagination, sorting, and AI-powered semantic search. Confirmed endpoint: `GET`/`POST /API/search/v4.0/search`, accepting `query`, `fields`, `format` (JSON or XML), `countperpage`, `pagenumber`, `sort`, and `semanticquery`.

- **Human URL:** [https://developer.orangelogic.com/reference/search-api](https://developer.orangelogic.com/reference/search-api)
- **Base URL:** `https://{OrangeLogicURL}/API`

### Orange Logic Assets and Media API

Upload, import, retrieve, and manage digital assets and their representations - single-file, batch, cloud-storage, and large-file (>1.5GB) uploads, plus content delivery via public links, CDN, and presigned URLs. Upload endpoints are versioned (`UploadNewMedia` v1.0-v3.0 legacy; the newer `/webapi` upload family is recommended). Precise per-instance identifiers vary by instance and version.

- **Human URL:** [https://developer.orangelogic.com/reference/about](https://developer.orangelogic.com/reference/about)
- **Base URL:** `https://{OrangeLogicURL}/webapi`

### Orange Logic DataTable API

Work directly with database objects - assets (images, video, audio), folders, groups, users, tags, keywords, and relationships - through generic CREATE, READ, UPDATE, and DELETE calls. Paths follow the pattern `/API/DataTable/V2.2/Documents.{asset-type}.{asset-subtype}:Read` and similar verbs.

- **Human URL:** [https://developer.orangelogic.com/reference/datatable-apis](https://developer.orangelogic.com/reference/datatable-apis)
- **Base URL:** `https://{OrangeLogicURL}/API`

### Orange Logic Metadata API

List and modify asset metadata - retrieve all metadata fields, update tags and linked fields, and manage language-specific field values. Includes batch edit and batch upsert operations.

- **Human URL:** [https://developer.orangelogic.com/reference/about](https://developer.orangelogic.com/reference/about)
- **Base URL:** `https://{OrangeLogicURL}/webapi`

### Orange Logic Users and Contacts API

Manage user and contact accounts, group assignments, permissions, and organizational hierarchies through the DataTable object model (Users, Groups, Contacts).

- **Human URL:** [https://developer.orangelogic.com/reference/datatable-apis](https://developer.orangelogic.com/reference/datatable-apis)
- **Base URL:** `https://{OrangeLogicURL}/API`

### Orange Logic Webhooks API

Subscribe to asset lifecycle events and send webhooks to a third-party service when assets are created, edited, or deleted. This is a server-to-endpoint HTTP callback surface, not a persistent socket connection.

- **Human URL:** [https://developer.orangelogic.com/reference/about](https://developer.orangelogic.com/reference/about)
- **Base URL:** `https://{OrangeLogicURL}/webapi`

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/orange-logic)
- [Website](https://www.orangelogic.com)
- [Documentation](https://developer.orangelogic.com)
- [Plans](plans/orangelogic-plans-pricing.yml)
- [Rate Limits](rate-limits/orangelogic-rate-limits.yml)
- [Fin Ops](finops/orangelogic-finops.yml)

## Endpoints Modeled

Because the Orange Logic API is per-instance, most endpoint identifiers are specific to a customer's deployment and version. Where exact paths are published in the public reference (Authentication token, Search, DataTable), they are reproduced here. Elsewhere, endpoints are honestly modeled from the public documentation rather than fabricated. See `review.yml` for the full transport and access analysis.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
