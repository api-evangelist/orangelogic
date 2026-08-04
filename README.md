# Orange Logic (orangelogic)

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
