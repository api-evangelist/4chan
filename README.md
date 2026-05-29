# 4chan (4chan)

4chan is a simple image-based bulletin board where anyone can post comments and share images across topic-specific boards. 4chan exposes a read-only JSON API (launched September 2012) that serves the same board, thread, catalog, and archive data consumed by the public site via static JSON files at a.4cdn.org. The API supports GET/HEAD/OPTIONS only — there is no posting, authentication, or write surface.

**URL:** [Visit APIs.json URL](https://github.com/4chan/4chan-API)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Social, Bulletin Board, Imageboard, Read Only, JSON, Public APIs, Community

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-28

## APIs

### 4chan Read-Only JSON API
Read-only HTTP JSON API serving boards.json, threads.json, catalog.json, archive.json, board index pages, and individual thread documents from a.4cdn.org. Mirrors the data visible at boards.4chan.org / boards.4channel.org. No authentication, no write operations. CORS allowed only from boards.4chan.org and boards.4channel.org origins.

**Human URL:** [https://github.com/4chan/4chan-API](https://github.com/4chan/4chan-API)

#### Tags:

 - Social, Imageboard, Read Only

#### Properties

- [Documentation](https://github.com/4chan/4chan-API)
- [OpenAPI](openapi/4chan-api.yml)
- [SignUp](https://github.com/4chan/4chan-API#api-rules)
- [Support](mailto:api@4chan.org)
- [TermsOfService](https://github.com/4chan/4chan-API#api-terms-of-service)
- [NaftikoCapability](capabilities/4chan-api-boards.yaml)
- [NaftikoCapability](capabilities/4chan-api-threadlist.yaml)
- [NaftikoCapability](capabilities/4chan-api-catalog.yaml)
- [NaftikoCapability](capabilities/4chan-api-archive.yaml)
- [NaftikoCapability](capabilities/4chan-api-indexes.yaml)
- [NaftikoCapability](capabilities/4chan-api-threads.yaml)

## Common Properties

- [Website](https://www.4chan.org)
- [Documentation](https://github.com/4chan/4chan-API)
- [GitHubOrganization](https://github.com/4chan)
- [SourceCode — 4chan native browser extension source](https://github.com/4chan/4chan-JS)
- [ContactEmail](mailto:api@4chan.org)
- [Tools — MCP Server (community, unofficial)](https://github.com/sh0n0/chan-mcp-server)
- [SDK — Python Wrapper (BASC-py4chan, community)](https://github.com/bibanon/BASC-py4chan)
- [SDK — Python Wrapper (py-4chan, community)](https://github.com/e000/py-4chan)
- [SDK — Node.js Client (4chanjs, community)](https://github.com/yocontra/4chanjs)
- [SDK — Go Client (go-4chan-api, community)](https://github.com/moshee/go-4chan-api)
- [SDK — Rust Client (rchan, community)](https://github.com/insomnimus/rchan)
- [SDK — Racket Client (yotsubAPI, community)](https://github.com/g-gundam/yotsubAPI)
- [Tools — BA Thread Archiver (community)](https://github.com/hydrusnetwork/BA-4chan-thread-archiver)
- [PublicAPIsListing](https://github.com/public-apis/public-apis)
- [Plans](plans/4chan-plans-pricing.yml)
- [RateLimits](rate-limits/4chan-rate-limits.yml)
- [Vocabulary](vocabulary/4chan-vocabulary.yml)
- [SpectralRules](rules/4chan-rules.yml)
- [JSONLD](json-ld/4chan-context.jsonld)

## Features

| Name | Description |
|------|-------------|
| Read-Only JSON Catalog | Static JSON representations of boards, threads, catalogs, and archives are served from a.4cdn.org; clients use standard HTTP semantics including If-Modified-Since for caching. |
| No Authentication | The API requires no API key, no token, and no account; it is fully anonymous and serves the same data visible to anonymous web visitors. |
| HTTP Caching Built In | The API requires clients to send If-Modified-Since headers on repeated requests, allowing 304 Not Modified responses and reducing server load. |
| CORS Restricted to 4chan Origins | CORS is enabled but only for origins boards.4chan.org and boards.4channel.org via HTTP or HTTPS; only GET/OPTIONS/HEAD methods are accepted. |
| Per-Board Catalog | Every board (a, b, g, pol, po, etc.) exposes catalog, threadlist, archive, and per-page index endpoints with the same shape, making bulk crawling trivial. |
| Static Media Domains | User-uploaded images and thumbnails live at i.4cdn.org/{board}/{tim}.{ext}; static site assets including flags, spoiler images, and capcode icons live at s.4cdn.org. |

## Use Cases

| Name | Description |
|------|-------------|
| Read-Only Board Crawlers | Build research crawlers that periodically snapshot board catalogs, threads, and archives while respecting the 1 request per second limit and 10 second per-thread refresh floor. |
| Thread Archivers | Mirror archived threads and their attached media to durable storage for academic study or cultural preservation (see BA Thread Archiver, Ayase / Asagi). |
| Imageboard Analytics | Use threads.json and catalog.json to chart posting volume, reply velocity, and moderator/admin capcode activity across boards over time. |
| Language Models and Markov Chains | Feed cleaned post comments from catalog.json and thread.json into text generation experiments (see 4chanMarkovText). |
| Static Site Mirrors | Combine boards.json + per-board catalog/thread JSON to build static site mirrors of individual threads suitable for read-only display. |

## Integrations

| Name | Description |
|------|-------------|
| BASC-py4chan | Python wrapper providing Pythonic access to boards, threads, and posts. |
| 4chanjs | Node.js and browser client for the 4chan JSON API. |
| go-4chan-api | Go client for crawling and consuming 4chan board JSON. |
| rchan | Rust crate exposing typed boards/threads/posts and a basic client. |
| Ayase / Asagi | Archive middleware that ingests 4chan JSON and stores posts in SQL for replay. |
| chan-mcp-server (community) | Unofficial Model Context Protocol server exposing 4chan boards/threads/catalog as MCP tools. |

## Solutions

| Name | Description |
|------|-------------|
| Imageboard Research Archive | Combine threads.json polling with archive.json snapshots and i.4cdn.org media downloads to build a long-term archive that respects the published rate limits. |
| Capcode Activity Dashboard | Use catalog.json/thread.json capcode and id fields to surface moderator and admin activity per board over time. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [4chan Read-Only JSON API](openapi/4chan-api.yml)

### JSON Schema

- [Archive Response](json-schema/4chan-api-archive-response-schema.json)
- [Board](json-schema/4chan-api-board-schema.json)
- [Boards Response](json-schema/4chan-api-boards-response-schema.json)
- [Catalog Page](json-schema/4chan-api-catalog-page-schema.json)
- [Catalog Response](json-schema/4chan-api-catalog-response-schema.json)
- [Cooldowns](json-schema/4chan-api-cooldowns-schema.json)
- [Index Page Response](json-schema/4chan-api-index-page-response-schema.json)
- [Index Page Thread](json-schema/4chan-api-index-page-thread-schema.json)
- [Post](json-schema/4chan-api-post-schema.json)
- [Thread Response](json-schema/4chan-api-thread-response-schema.json)
- [Threadlist Entry](json-schema/4chan-api-threadlist-entry-schema.json)
- [Threadlist Page](json-schema/4chan-api-threadlist-page-schema.json)
- [Threadlist Response](json-schema/4chan-api-threadlist-response-schema.json)

### JSON Structure

- [Archive Response](json-structure/4chan-api-archive-response-structure.json)
- [Board](json-structure/4chan-api-board-structure.json)
- [Boards Response](json-structure/4chan-api-boards-response-structure.json)
- [Catalog Page](json-structure/4chan-api-catalog-page-structure.json)
- [Catalog Response](json-structure/4chan-api-catalog-response-structure.json)
- [Cooldowns](json-structure/4chan-api-cooldowns-structure.json)
- [Index Page Response](json-structure/4chan-api-index-page-response-structure.json)
- [Index Page Thread](json-structure/4chan-api-index-page-thread-structure.json)
- [Post](json-structure/4chan-api-post-structure.json)
- [Thread Response](json-structure/4chan-api-thread-response-structure.json)
- [Threadlist Entry](json-structure/4chan-api-threadlist-entry-structure.json)
- [Threadlist Page](json-structure/4chan-api-threadlist-page-structure.json)
- [Threadlist Response](json-structure/4chan-api-threadlist-response-structure.json)

### JSON-LD

- [4chan Context](json-ld/4chan-context.jsonld)

### Examples

- [Archive Response](examples/4chan-api-archive-response-example.json)
- [Board](examples/4chan-api-board-example.json)
- [Boards Response](examples/4chan-api-boards-response-example.json)
- [Catalog Page](examples/4chan-api-catalog-page-example.json)
- [Catalog Response](examples/4chan-api-catalog-response-example.json)
- [Cooldowns](examples/4chan-api-cooldowns-example.json)
- [Index Page Response](examples/4chan-api-index-page-response-example.json)
- [Index Page Thread](examples/4chan-api-index-page-thread-example.json)
- [Post](examples/4chan-api-post-example.json)
- [Thread Response](examples/4chan-api-thread-response-example.json)
- [Threadlist Entry](examples/4chan-api-threadlist-entry-example.json)
- [Threadlist Page](examples/4chan-api-threadlist-page-example.json)
- [Threadlist Response](examples/4chan-api-threadlist-response-example.json)

## Capabilities

Naftiko capabilities organized one self-contained file per business surface (OpenAPI tag), each with both a REST adapter and an MCP adapter.

### 4chan Read-Only JSON API

| Capability | Operations | File |
|------------|------------|------|
| Boards | 1 | [capabilities/4chan-api-boards.yaml](capabilities/4chan-api-boards.yaml) |
| Threadlist | 1 | [capabilities/4chan-api-threadlist.yaml](capabilities/4chan-api-threadlist.yaml) |
| Catalog | 1 | [capabilities/4chan-api-catalog.yaml](capabilities/4chan-api-catalog.yaml) |
| Archive | 1 | [capabilities/4chan-api-archive.yaml](capabilities/4chan-api-archive.yaml) |
| Indexes | 1 | [capabilities/4chan-api-indexes.yaml](capabilities/4chan-api-indexes.yaml) |
| Threads | 1 | [capabilities/4chan-api-threads.yaml](capabilities/4chan-api-threads.yaml) |

## Vocabulary

- [4chan Vocabulary](vocabulary/4chan-vocabulary.yml) — Unified taxonomy mapping 6 resources, 2 actions, 6 workflows, and 3 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [4chan Spectral Ruleset](rules/4chan-rules.yml) — 45 rules across 12 categories enforcing 4chan API conventions

## Plans & Rate Limits

- [4chan Plans / Pricing](plans/4chan-plans-pricing.yml) — Free read-only JSON API; 4chan Pass documented for context only
- [4chan Rate Limits](rate-limits/4chan-rate-limits.yml) — 1 req/sec global, 10 seconds-per-thread polling floor, IP-scoped

## Notes

The 4chan Read-Only JSON API was bulk-registered as part of a public-apis catalog sweep on 2026-05-28 and then enriched with a full OpenAPI 3.0.3 spec, Microcks-compatible inline examples, a Spectral ruleset, six per-tag Naftiko capabilities (REST + MCP), JSON Schema / JSON Structure / JSON-LD / example artifacts, a vocabulary, and API Commons Plans + Rate Limits documents — all generated from the official documentation at github.com/4chan/4chan-API.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
