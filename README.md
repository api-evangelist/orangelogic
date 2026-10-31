# Orange Logic

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

Orange Logic builds OrangeDAM (formerly branded Cortex), an enterprise digital asset management (DAM) and media asset management (MAM) platform used by museums, media companies, financial institutions, healthcare, and government archives. OrangeDAM exposes a documented REST API for assets, metadata, search, users, folders, and webhooks. The API is per-instance and customer-gated - every call is made against your own organization's Orange Logic instance host rather than a single shared public gateway, so the base URL is written here as the placeholder https://{OrangeLogicURL}/webapi. Endpoints come in two families - the newer /webapi/ endpoints (each ending in a unique identifier and version, e.g. token_48I_v1) and the legacy /api/ endpoints (with a version number in the path); Orange Logic recommends the /webapi/ family. Responses are JSON or XML. Pricing is enterprise contact-sales only.

**Areas:** Digital Asset Management · Media Asset Management · MAM · Enterprise · Metadata · Archives

## Orange Logic on APIs.io

Everything profiled for Orange Logic is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/orangelogic/](https://apis.io/providers/orangelogic/)** — or go straight to one of the APIs or properties below.

### APIs (48)

- [Orange Logic Authentication API](https://apis.io/apis/orangelogic/orangelogic-authentication-api/) — Authenticate against an Orange Logic instance and obtain tokens for subsequent calls. Supports OAuth 2.0 (client ID and secret), non-expiring bearer tokens,…
- [Orange Logic Search API](https://apis.io/apis/orangelogic/orangelogic-search-api/) — Find assets across the DAM with query criteria, field selection, pagination, sorting, and AI-powered semantic search. The confirmed endpoint is GET or POST…
- [Orange Logic Assets and Media API](https://apis.io/apis/orangelogic/orangelogic-assets-media-api/) — Upload, import, retrieve, and manage digital assets and their representations - single-file uploads, batch uploads, cloud-storage imports, and large-file…
- [Orange Logic DataTable API](https://apis.io/apis/orangelogic/orangelogic-datatable-api/) — Work directly with database objects - assets (images, video, audio), folders, groups, users, tags, keywords, and relationships - through generic CREATE,…
- [Orange Logic Metadata API](https://apis.io/apis/orangelogic/orangelogic-metadata-api/) — List and modify asset metadata - retrieve all metadata fields, update tags and linked fields, and manage language-specific field values. Includes batch edit…
- [Orange Logic Users and Contacts API](https://apis.io/apis/orangelogic/orangelogic-users-contacts-api/) — Manage user and contact accounts, group assignments, permissions, and organizational hierarchies. Handled through the DataTable object model (Users, Groups,…
- [Orange Logic Webhooks API](https://apis.io/apis/orangelogic/orangelogic-webhooks-api/) — Subscribe to asset lifecycle events and send webhooks to a third-party service when assets are created, edited, or deleted. This is a server-to-endpoint…
- [Orange Logic Batcheditfields 4FQ V1 API](https://apis.io/apis/orangelogic/orangelogic-batcheditfields-4fq-v1-api/) — The Batcheditfields 4FQ V1 API from Orange Logic — 1 operation(s) for batcheditfields 4fq v1.
- [Orange Logic Batchupsert 4FY V1 API](https://apis.io/apis/orangelogic/orangelogic-batchupsert-4fy-v1-api/) — The Batchupsert 4FY V1 API from Orange Logic — 1 operation(s) for batchupsert 4fy v1.
- [Orange Logic Batchupsert Csv 4G3 V1 API](https://apis.io/apis/orangelogic/orangelogic-batchupsert-csv-4g3-v1-api/) — The Batchupsert Csv 4G3 V1 API from Orange Logic — 1 operation(s) for batchupsert csv 4g3 v1.
- [Orange Logic Batchupsertassetlinkswithcustomroute 41FD V2 API](https://apis.io/apis/orangelogic/orangelogic-batchupsertassetlinkswithcustomroute-41fd-v2-api/) — The Batchupsertassetlinkswithcustomroute 41FD V2 API from Orange Logic — 1 operation(s) for batchupsertassetlinkswithcustomroute 41fd v2.
- [Orange Logic Bearerauthentication API](https://apis.io/apis/orangelogic/orangelogic-bearerauthentication-api/) — The Bearerauthentication API from Orange Logic — 2 operation(s) for bearerauthentication.
- [Orange Logic Clientcredentialsauthentication API](https://apis.io/apis/orangelogic/orangelogic-clientcredentialsauthentication-api/) — The Clientcredentialsauthentication API from Orange Logic — 1 operation(s) for clientcredentialsauthentication.
- [Orange Logic Complete 27 V1 API](https://apis.io/apis/orangelogic/orangelogic-complete-27-v1-api/) — The Complete 27 V1 API from Orange Logic — 1 operation(s) for complete 27 v1.
- [Orange Logic Create 22E V1 API](https://apis.io/apis/orangelogic/orangelogic-create-22e-v1-api/) — The Create 22E V1 API from Orange Logic — 1 operation(s) for create 22e v1.
- [Orange Logic Create Crop Link API](https://apis.io/apis/orangelogic/orangelogic-createcroplink-api/) — The CreateCropLink API from Orange Logic — 1 operation(s) for createcroplink.
- [Orange Logic Createsharelink 41M9 V1 API](https://apis.io/apis/orangelogic/orangelogic-createsharelink-41m9-v1-api/) — The Createsharelink 41M9 V1 API from Orange Logic — 1 operation(s) for createsharelink 41m9 v1.
- [Orange Logic Documents.All:List Fields API](https://apis.io/apis/orangelogic/orangelogic-documents-all-listfields-api/) — The Documents.All:ListFields API from Orange Logic — 1 operation(s) for documents.all:listfields.
- [Orange Logic Documents.{Asset Type}.{Asset Subtype}:AssignLeadDocument API](https://apis.io/apis/orangelogic/orangelogic-documents-asset-type-asset-subtype-assignleaddocument-api/) — The Documents.{Asset Type}.{Asset Subtype}:AssignLeadDocument API from Orange Logic — 1 operation(s) for documents.{asset type}.{asset…
- [Orange Logic Getfilterinfo 4104 V1 API](https://apis.io/apis/orangelogic/orangelogic-getfilterinfo-4104-v1-api/) — The Getfilterinfo 4104 V1 API from Orange Logic — 1 operation(s) for getfilterinfo 4104 v1.
- [Orange Logic Getlink 4HZ V1 API](https://apis.io/apis/orangelogic/orangelogic-getlink-4hz-v1-api/) — The Getlink 4HZ V1 API from Orange Logic — 1 operation(s) for getlink 4hz v1.
- [Orange Logic Getlinks 45W V1 API](https://apis.io/apis/orangelogic/orangelogic-getlinks-45w-v1-api/) — The Getlinks 45W V1 API from Orange Logic — 1 operation(s) for getlinks 45w v1.
- [Orange Logic Getpresignedlink 4ar V1 API](https://apis.io/apis/orangelogic/orangelogic-getpresignedlink-4ar-v1-api/) — The Getpresignedlink 4ar V1 API from Orange Logic — 1 operation(s) for getpresignedlink 4ar v1.
- [Orange Logic Getpresignedlinks In Batch 4G8 V1 API](https://apis.io/apis/orangelogic/orangelogic-getpresignedlinks-in-batch-4g8-v1-api/) — The Getpresignedlinks In Batch 4G8 V1 API from Orange Logic — 1 operation(s) for getpresignedlinks in batch 4g8 v1.
- [Orange Logic Getreport 4103 V1 API](https://apis.io/apis/orangelogic/orangelogic-getreport-4103-v1-api/) — The Getreport 4103 V1 API from Orange Logic — 1 operation(s) for getreport 4103 v1.
- [Orange Logic Getreportinfo 4102 V1 API](https://apis.io/apis/orangelogic/orangelogic-getreportinfo-4102-v1-api/) — The Getreportinfo 4102 V1 API from Orange Logic — 1 operation(s) for getreportinfo 4102 v1.
- [Orange Logic Getsharelinkstatus 41MA V1 API](https://apis.io/apis/orangelogic/orangelogic-getsharelinkstatus-41ma-v1-api/) — The Getsharelinkstatus 41MA V1 API from Orange Logic — 1 operation(s) for getsharelinkstatus 41ma v1.
- [Orange Logic Getwatermarkpresets 41MB V1 API](https://apis.io/apis/orangelogic/orangelogic-getwatermarkpresets-41mb-v1-api/) — The Getwatermarkpresets 41MB V1 API from Orange Logic — 1 operation(s) for getwatermarkpresets 41mb v1.
- [Orange Logic InvalidateCloudfrontCache 2cl V1 API](https://apis.io/apis/orangelogic/orangelogic-invalidatecloudfrontcache-2cl-v1-api/) — The InvalidateCloudfrontCache 2cl V1 API from Orange Logic — 1 operation(s) for invalidatecloudfrontcache 2cl v1.
- [Orange Logic Item API](https://apis.io/apis/orangelogic/orangelogic-item-api/) — The Item API from Orange Logic — 1 operation(s) for item.
- [Orange Logic List All Database Objects API](https://apis.io/apis/orangelogic/orangelogic-list-all-database-objects-api/) — The List All Database Objects API from Orange Logic — 1 operation(s) for list all database objects.
- [Orange Logic List Criteria API](https://apis.io/apis/orangelogic/orangelogic-listcriteria-api/) — The ListCriteria API from Orange Logic — 1 operation(s) for listcriteria.
- [Orange Logic List Fields API](https://apis.io/apis/orangelogic/orangelogic-listfields-api/) — The ListFields API from Orange Logic — 1 operation(s) for listfields.
- [Orange Logic Login API](https://apis.io/apis/orangelogic/orangelogic-login-api/) — The Login API from Orange Logic — 1 operation(s) for login.
- [Orange Logic Oauth2 API](https://apis.io/apis/orangelogic/orangelogic-oauth2-api/) — The Oauth2 API from Orange Logic — 3 operation(s) for oauth2.
- [Orange Logic Query Batchupsert 4G2 V1 API](https://apis.io/apis/orangelogic/orangelogic-query-batchupsert-4g2-v1-api/) — The Query Batchupsert 4G2 V1 API from Orange Logic — 1 operation(s) for query batchupsert 4g2 v1.
- [Orange Logic Querybatchupsertassetlinkswithcustomroutejobstatus 41FE V1 API](https://apis.io/apis/orangelogic/orangelogic-querybatchupsertassetlinkswithcustomroutejobstatus-41fe-v1-api/) — The Querybatchupsertassetlinkswithcustomroutejobstatus 41FE V1 API from Orange Logic — 1 operation(s) for querybatchupsertassetlinkswithcustomroutejobstatus…
- [Orange Logic Regenerate Proxies For Asset API](https://apis.io/apis/orangelogic/orangelogic-regenerateproxiesforasset-api/) — The RegenerateProxiesForAsset API from Orange Logic — 1 operation(s) for regenerateproxiesforasset.
- [Orange Logic Register 25 V1 API](https://apis.io/apis/orangelogic/orangelogic-register-25-v1-api/) — The Register 25 V1 API from Orange Logic — 1 operation(s) for register 25 v1.
- [Orange Logic Rotatesecret 22P V1 API](https://apis.io/apis/orangelogic/orangelogic-rotatesecret-22p-v1-api/) — The Rotatesecret 22P V1 API from Orange Logic — 1 operation(s) for rotatesecret 22p v1.
- [Orange Logic Search API](https://apis.io/apis/orangelogic/orangelogic-search-api/) — The Search API from Orange Logic — 1 operation(s) for search.
- [Orange Logic Transaction API](https://apis.io/apis/orangelogic/orangelogic-transaction-api/) — The Transaction API from Orange Logic — 1 operation(s) for transaction.
- [Orange Logic UploadFileFromCloudStorage 4OY V1 API](https://apis.io/apis/orangelogic/orangelogic-uploadfilefromcloudstorage-4oy-v1-api/) — The UploadFileFromCloudStorage 4OY V1 API from Orange Logic — 1 operation(s) for uploadfilefromcloudstorage 4oy v1.
- [Orange Logic Uploadimageandgetlargestdownloadlink 4CM V1 API](https://apis.io/apis/orangelogic/orangelogic-uploadimageandgetlargestdownloadlink-4cm-v1-api/) — The Uploadimageandgetlargestdownloadlink 4CM V1 API from Orange Logic — 1 operation(s) for uploadimageandgetlargestdownloadlink 4cm v1.
- [Orange Logic Uploadmedia 4az V1 API](https://apis.io/apis/orangelogic/orangelogic-uploadmedia-4az-v1-api/) — The Uploadmedia 4az V1 API from Orange Logic — 1 operation(s) for uploadmedia 4az v1.
- [Orange Logic Uploadmediawithurl 45L V1 API](https://apis.io/apis/orangelogic/orangelogic-uploadmediawithurl-45l-v1-api/) — The Uploadmediawithurl 45L V1 API from Orange Logic — 1 operation(s) for uploadmediawithurl 45l v1.
- [Orange Logic Upload New Media API](https://apis.io/apis/orangelogic/orangelogic-uploadnewmedia-api/) — The UploadNewMedia API from Orange Logic — 1 operation(s) for uploadnewmedia.
- [Orange Logic Upload New Version API](https://apis.io/apis/orangelogic/orangelogic-uploadnewversion-api/) — The UploadNewVersion API from Orange Logic — 1 operation(s) for uploadnewversion.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [orangelogic-mcp.yml](https://apis.io/servers/orangelogic/orangelogic-mcp-yml/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Orangelogic Agentic Access](https://apis.io/agentic-access/orangelogic/orangelogic-agentic-access/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Orange Logic API Rules](https://apis.io/rules/orangelogic/orangelogic-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Orangelogic Authentication](https://apis.io/security/orangelogic/orangelogic-authentication/)
- [Orangelogic Domain Security](https://apis.io/security/orangelogic/orangelogic-domain-security/)
- [Orangelogic Trust Center](https://apis.io/security/orangelogic/orangelogic-trust-center/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Orangelogic Scopes](https://apis.io/scopes/orangelogic/orangelogic-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Orangelogic Plans Pricing](https://apis.io/plans/orangelogic/orangelogic-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Orangelogic Rate Limits](https://apis.io/rate-limits/orangelogic/orangelogic-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Orangelogic Finops](https://apis.io/finops/orangelogic/orangelogic-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.orangelogic.com)
- [Documentation](https://developer.orangelogic.com)
- [Blog](https://www.orangelogic.com/dam-blog)
- [Security](https://www.orangelogic.com/features/security)
- [Compliance](https://www.orangelogic.com/security)
- [Terms of service](https://www.orangelogic.com/terms-and-conditions)
- [Privacy policy](https://www.orangelogic.com/privacy-policy)

## API Evangelist rating

**Kin Score 42.4** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 80.4 |
| Contract quality | 43.9 |
| Contract governance | 18.2 |
| Operational transparency | 18.4 |
| Developer ergonomics | 26.2 |
| Access clarity | 42.1 |

**Agent readiness 27.1** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | verified |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 39.2** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/orangelogic/](https://apis.io/providers/orangelogic/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Orange Logic: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/orangelogic/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
