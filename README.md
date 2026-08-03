# 4chan (4chan)

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

4chan is a simple image-based bulletin board where anyone can post comments and share images across topic-specific boards. 4chan exposes a read-only JSON API (launched September 2012) that serves the same board, thread, catalog, and archive data consumed by the public site via static JSON files at a.4cdn.org. The API supports GET/HEAD/OPTIONS only — there is no posting, authentication, or write surface.

**APIs.json:** [https://github.com/4chan/4chan-API](https://github.com/4chan/4chan-API)

## Tags

- Social
- Bulletin Board
- Imageboard
- Read Only
- JSON
- Public APIs
- Community

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-28

## APIs

### 4chan Read-Only JSON API

Read-only HTTP JSON API serving boards.json, threads.json, catalog.json, archive.json, board index pages, and individual thread documents from a.4cdn.org. Mirrors the data visible at boards.4chan.org / boards.4channel.org. No authentication, no write operations. CORS allowed only from boards.4chan.org and boards.4channel.org origins.

- **Human URL:** [https://github.com/4chan/4chan-API](https://github.com/4chan/4chan-API)
- **Base URL:** `https://a.4cdn.org`

#### Tags

- Social
- Imageboard
- Read Only

#### Properties

- [Documentation](https://github.com/4chan/4chan-API)
- [OpenAPI](openapi/4chan-api.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/4chan-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/4chan-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Sign Up](https://github.com/4chan/4chan-API#api-rules)
- [Support](mailto:api@4chan.org)
- [Terms of Service](https://github.com/4chan/4chan-API#api-terms-of-service)

## Common Properties

- [Website](https://www.4chan.org)
- [Documentation](https://github.com/4chan/4chan-API)
- [GitHub Organization](https://github.com/4chan)
- [Source Code](https://github.com/4chan/4chan-JS)
- [Contact Email](mailto:api@4chan.org)
- [Tools](https://github.com/sh0n0/chan-mcp-server)
- [SDK](https://github.com/bibanon/BASC-py4chan)
- [SDK](https://github.com/e000/py-4chan)
- [SDK](https://github.com/yocontra/4chanjs)
- [SDK](https://github.com/moshee/go-4chan-api)
- [SDK](https://github.com/insomnimus/rchan)
- [SDK](https://github.com/g-gundam/yotsubAPI)
- [Tools](https://github.com/hydrusnetwork/BA-4chan-thread-archiver)
- [Public APIs Listing](https://github.com/public-apis/public-apis)
- [Plans](plans/4chan-plans-pricing.yml)
- [Rate Limits](rate-limits/4chan-rate-limits.yml)
- [Vocabulary](vocabulary/4chan-vocabulary.yml)
- [Spectral Rules](rules/4chan-rules.yml)
- [JSON-LD](json-ld/4chan-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
