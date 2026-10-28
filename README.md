# 4chan

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

4chan is a simple image-based bulletin board where anyone can post comments and share images across topic-specific boards. 4chan exposes a read-only JSON API (launched September 2012) that serves the same board, thread, catalog, and archive data consumed by the public site via static JSON files at a.4cdn.org. The API supports GET/HEAD/OPTIONS only — there is no posting, authentication, or write surface.

**Areas:** Social · Bulletin Board · Imageboard · Read Only · JSON · Public APIs · Community

## 4chan on APIs.io

Everything profiled for 4chan is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/4chan/](https://apis.io/providers/4chan/)** — or go straight to one of the APIs or properties below.

### APIs (6)

- [4chan Archive API](https://apis.io/apis/4chan/4chan-archive-api/) — Per-board list of OP numbers for closed, archived threads.
- [4chan Boards API](https://apis.io/apis/4chan/4chan-boards-api/) — List of all boards on 4chan and 4channel and their per-board settings.
- [4chan Catalog API](https://apis.io/apis/4chan/4chan-catalog-api/) — Per-board catalog snapshot containing every OP and its preview replies, grouped by index page.
- [4chan Indexes API](https://apis.io/apis/4chan/4chan-indexes-api/) — Per-board, per-page index document of threads (each with a posts array including the OP and a small number of preview replies).
- [4chan Threadlist API](https://apis.io/apis/4chan/4chan-threadlist-api/) — Per-board summary list of every live thread (id, last-modified, reply count) grouped by index page.
- [4chan Threads API](https://apis.io/apis/4chan/4chan-threads-api/) — Single-thread document containing the OP and every reply.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [4Chan Agentic Access](https://apis.io/agentic-access/4chan/4chan-agentic-access/)

#### JSON Schema (13)

The data models the API reads and writes.

- [ArchiveResponse](https://apis.io/schemas/4chan/4chan-api-archive-response/)
- [Board](https://apis.io/schemas/4chan/4chan-api-board/)
- [BoardsResponse](https://apis.io/schemas/4chan/4chan-api-boards-response/)
- [CatalogPage](https://apis.io/schemas/4chan/4chan-api-catalog-page/)
- [CatalogResponse](https://apis.io/schemas/4chan/4chan-api-catalog-response/)
- [Cooldowns](https://apis.io/schemas/4chan/4chan-api-cooldowns/)
- [IndexPageResponse](https://apis.io/schemas/4chan/4chan-api-index-page-response/)
- [IndexPageThread](https://apis.io/schemas/4chan/4chan-api-index-page-thread/)
- [Post](https://apis.io/schemas/4chan/4chan-api-post/)
- [ThreadResponse](https://apis.io/schemas/4chan/4chan-api-thread-response/)
- [ThreadlistEntry](https://apis.io/schemas/4chan/4chan-api-threadlist-entry/)
- [ThreadlistPage](https://apis.io/schemas/4chan/4chan-api-threadlist-page/)
- [ThreadlistResponse](https://apis.io/schemas/4chan/4chan-api-threadlist-response/)

#### JSON Structure (13)

Data models expressed in JSON Structure.

- [4Chan Api Archive Response Structure](https://apis.io/json-structure/4chan/4chan-api-archive-response-structure/)
- [4Chan Api Board Structure](https://apis.io/json-structure/4chan/4chan-api-board-structure/)
- [4Chan Api Boards Response Structure](https://apis.io/json-structure/4chan/4chan-api-boards-response-structure/)
- [4Chan Api Catalog Page Structure](https://apis.io/json-structure/4chan/4chan-api-catalog-page-structure/)
- [4Chan Api Catalog Response Structure](https://apis.io/json-structure/4chan/4chan-api-catalog-response-structure/)
- [4Chan Api Cooldowns Structure](https://apis.io/json-structure/4chan/4chan-api-cooldowns-structure/)
- [4Chan Api Index Page Response Structure](https://apis.io/json-structure/4chan/4chan-api-index-page-response-structure/)
- [4Chan Api Index Page Thread Structure](https://apis.io/json-structure/4chan/4chan-api-index-page-thread-structure/)
- [4Chan Api Post Structure](https://apis.io/json-structure/4chan/4chan-api-post-structure/)
- [4Chan Api Thread Response Structure](https://apis.io/json-structure/4chan/4chan-api-thread-response-structure/)
- [4Chan Api Threadlist Entry Structure](https://apis.io/json-structure/4chan/4chan-api-threadlist-entry-structure/)
- [4Chan Api Threadlist Page Structure](https://apis.io/json-structure/4chan/4chan-api-threadlist-page-structure/)
- [4Chan Api Threadlist Response Structure](https://apis.io/json-structure/4chan/4chan-api-threadlist-response-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [4Chan Context](https://apis.io/jsonld/4chan/4chan-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [4Chan Vocabulary](https://apis.io/vocabularies/4chan/4chan-vocabulary/)

#### Examples (10)

Example requests and responses.

- [4Chan Api Board Example](https://apis.io/examples/4chan/4chan-api-board-example/)
- [4Chan Api Boards Response Example](https://apis.io/examples/4chan/4chan-api-boards-response-example/)
- [4Chan Api Catalog Page Example](https://apis.io/examples/4chan/4chan-api-catalog-page-example/)
- [4Chan Api Cooldowns Example](https://apis.io/examples/4chan/4chan-api-cooldowns-example/)
- [4Chan Api Index Page Response Example](https://apis.io/examples/4chan/4chan-api-index-page-response-example/)
- [4Chan Api Index Page Thread Example](https://apis.io/examples/4chan/4chan-api-index-page-thread-example/)
- [4Chan Api Post Example](https://apis.io/examples/4chan/4chan-api-post-example/)
- [4Chan Api Thread Response Example](https://apis.io/examples/4chan/4chan-api-thread-response-example/)
- [4Chan Api Threadlist Entry Example](https://apis.io/examples/4chan/4chan-api-threadlist-entry-example/)
- [4Chan Api Threadlist Page Example](https://apis.io/examples/4chan/4chan-api-threadlist-page-example/)

#### Collections (7)

Postman and Open Collection request collections.

- [4chan Read-Only JSON API](https://apis.io/collections/4chan/open-4chan-api/)
- [4chan Read-Only JSON Archive API](https://apis.io/collections/4chan/open-4chan-archive-api/)
- [4chan Read-Only JSON Archive Boards API](https://apis.io/collections/4chan/open-4chan-boards-api/)
- [4chan Read-Only JSON Archive Catalog API](https://apis.io/collections/4chan/open-4chan-catalog-api/)
- [4chan Read-Only JSON Archive Indexes API](https://apis.io/collections/4chan/open-4chan-indexes-api/)
- [4chan Read-Only JSON Archive Threadlist API](https://apis.io/collections/4chan/open-4chan-threadlist-api/)
- [4chan Read-Only JSON Archive Threads API](https://apis.io/collections/4chan/open-4chan-threads-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [4chan — jsonschema rules](https://apis.io/rules/4chan/4chan-jsonschema-spectral-rules/)
- [4chan API Rules](https://apis.io/rules/4chan/4chan-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [4Chan Domain Security](https://apis.io/security/4chan/4chan-domain-security/)
- [4Chan Vulnerability Disclosure](https://apis.io/security/4chan/4chan-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [4Chan Plans Pricing](https://apis.io/plans/4chan/4chan-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [4Chan Rate Limits](https://apis.io/rate-limits/4chan/4chan-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.4chan.org)
- [Documentation](https://github.com/4chan/4chan-API)
- [GitHub](https://github.com/4chan)

## API Evangelist rating

**Kin Score 29.9** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 21.3 |
| Contract governance | 27.3 |
| Operational transparency | 10.5 |
| Developer ergonomics | 31.0 |
| Access clarity | 28.9 |

**Agent readiness 23.6** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | na |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | na |
| Error Semantics | — |
| OpenAPI Examples | verified |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 20.6** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/4chan/](https://apis.io/providers/4chan/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for 4chan: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/4chan/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
