# The Movie Database (tmdb)

The Movie Database (TMDB) is a community-built movie, TV, and people metadata catalog with a free REST API used by streaming apps, recommendation engines, second-screen experiences, fan sites, and AI/ML workflows. The TMDB API v3 exposes ~150 endpoints across movies, TV series, seasons, episodes, people, credits, images, collections, companies, networks, keywords, genres, reviews, lists, certifications, trending, discover/search, watch providers, account/lists, authentication, and configuration. A v4 surface adds OAuth-style user authentication and richer list management. Non-commercial use is free; commercial use requires a separate written agreement with TMDB.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/tmdb/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Catalog, Discovery, Entertainment, Images, Media, Metadata, Movies, People, Recommendations, Reviews, Search, Streaming, Trending, TV, Video, Watch Providers

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### TMDB API

The full TMDB REST API surface (v3). Covers movies, TV series, seasons, episodes, people, credits, images, collections, companies, networks, keywords, genres, reviews, lists, certifications, find, trending, discover, search, watch providers, configuration, authentication, account, and guest sessions. JSON over HTTPS, with optional append_to_response to combine related sub-resources in a single response.

**Human URL:** [https://developer.themoviedb.org/reference/intro/getting-started](https://developer.themoviedb.org/reference/intro/getting-started)

**Base URL:** `https://api.themoviedb.org`

#### Tags:

 - Catalog, Discovery, Metadata, Movies, People, REST, Search, TV, Video

#### Properties

- [Documentation](https://developer.themoviedb.org/reference/intro/getting-started)
- [OpenAPI](openapi/tmdb-api-openapi-original.yml)
- [Sign Up](https://www.themoviedb.org/signup)
- [Get API Key](https://www.themoviedb.org/settings/api)
- [Authentication](https://developer.themoviedb.org/docs/authentication-application)
- [Change Log / Support Forum](https://www.themoviedb.org/talk/category/5047958519c29526b50017d6)
- [LLMs.txt](https://developer.themoviedb.org/llms.txt)

#### Naftiko Capabilities (per OpenAPI tag)

- [Account](capabilities/tmdb-api-account.yaml)
- [Authentication](capabilities/tmdb-api-authentication.yaml)
- [Certifications](capabilities/tmdb-api-certifications.yaml)
- [Collections](capabilities/tmdb-api-collections.yaml)
- [Companies](capabilities/tmdb-api-companies.yaml)
- [Configuration](capabilities/tmdb-api-configuration.yaml)
- [Credits](capabilities/tmdb-api-credits.yaml)
- [Discover](capabilities/tmdb-api-discover.yaml)
- [Find](capabilities/tmdb-api-find.yaml)
- [Genres](capabilities/tmdb-api-genres.yaml)
- [Guest Sessions](capabilities/tmdb-api-guest-sessions.yaml)
- [Keywords](capabilities/tmdb-api-keywords.yaml)
- [Lists](capabilities/tmdb-api-lists.yaml)
- [Movies](capabilities/tmdb-api-movies.yaml)
- [Networks](capabilities/tmdb-api-networks.yaml)
- [People](capabilities/tmdb-api-people.yaml)
- [Reviews](capabilities/tmdb-api-reviews.yaml)
- [Search](capabilities/tmdb-api-search.yaml)
- [Trending](capabilities/tmdb-api-trending.yaml)
- [TV Series](capabilities/tmdb-api-tv-series.yaml)
- [Watch Providers](capabilities/tmdb-api-watch-providers.yaml)

## Common Properties

- [Website](https://www.themoviedb.org)
- [Documentation](https://developer.themoviedb.org/)
- [API Overview](https://developer.themoviedb.org/docs/getting-started)
- [Sign Up](https://www.themoviedb.org/signup)
- [Get API Key](https://www.themoviedb.org/settings/api)
- [Authentication](https://developer.themoviedb.org/docs/authentication-application)
- [Rate Limiting Docs](https://developer.themoviedb.org/docs/rate-limiting)
- [Terms of Service](https://www.themoviedb.org/api-terms-of-use)
- [Privacy Policy](https://www.themoviedb.org/privacy-policy)
- [Support Forum](https://www.themoviedb.org/talk)
- [Status Page](https://status.themoviedb.org)
- [LLMs.txt](https://developer.themoviedb.org/llms.txt)
- [Wrappers & Libraries](https://developer.themoviedb.org/docs/wrappers-and-libraries)

### SDKs (community)

- [tmdbsimple (Python)](https://github.com/celiao/tmdbsimple) — [PyPI](https://pypi.org/project/tmdbsimple/)
- [moviedb-promise (JavaScript)](https://github.com/grantholle/moviedb-promise) — [npm](https://www.npmjs.com/package/moviedb-promise)
- [tmdb (TypeScript)](https://github.com/leandrowkz/tmdb)
- [tmdb-ts (TypeScript)](https://github.com/blakejoy/tmdb-ts)
- [TMDbLib (.NET)](https://github.com/LordMike/TMDbLib)
- [golang-tmdb (Go)](https://github.com/cyruzin/golang-tmdb)
- [go-tmdb (Go)](https://github.com/ryanbradynd05/go-tmdb)
- [TMDb (Swift)](https://github.com/adamayoung/TMDb)
- [php-tmdb-api (PHP)](https://github.com/wtfzdotnet/php-tmdb-api)
- [themoviedb (Ruby)](https://github.com/ahmetabdi/themoviedb)
- [themoviedbapi (Java)](https://github.com/c-eg/themoviedbapi)

### MCP Server

- [MCP-TMDB (community)](https://github.com/leonardogilrodriguez/mcp-tmdb)

## Features

| Name | Description |
|------|-------------|
| Movie Metadata | Full movie details — title, overview, runtime, budget, revenue, genres, languages, production companies, release dates, ratings, images, videos, and credits. |
| TV Metadata | Series, seasons, and episode data with cast, crew, air dates, episode groups, content ratings, and networks. |
| People Metadata | Cast and crew profiles with combined movie + TV credits, biographies, images, external IDs (IMDB, social), and translations. |
| Search | Multi-search and per-resource search (movie, TV, person, company, collection, keyword) with relevance ranking and pagination. |
| Discover | Faceted browse of movies and TV shows with 30+ filters including genre, year, rating, language, region, watch provider, runtime, and cast/crew. |
| Trending | Daily and weekly trending lists across movies, TV, and people based on community activity. |
| Append To Response | Combine up to 20 related sub-resource calls (credits, images, videos, similar, recommendations) into a single HTTP request to minimise round trips. |
| Watch Providers | Per-region availability data sourced from JustWatch covering streaming, rent, and buy options for movies and TV. |
| Images | Multi-language poster, backdrop, logo, and profile images with size variants served via the TMDB image CDN. |
| Daily ID Exports | Bulk-downloadable nightly JSON files listing all valid IDs for movies, TV, people, and other entities for incremental sync. |
| Lists & Account | User-owned lists, favorites, watchlist, and ratings via authenticated v3 and v4 endpoints. |
| Configuration | Image base URLs, supported languages, countries, timezones, and translation endpoints needed to render content correctly. |

## Use Cases

| Name | Description |
|------|-------------|
| Streaming Catalog Enrichment | Streaming and VOD apps pull canonical title metadata, posters, and watch provider availability to populate browse and detail screens. |
| Recommendation Engines | ML teams use TMDB metadata + ratings + trending signals as a feature source for personalised movie and TV recommendations. |
| Fan Sites and Communities | Fan wikis, review sites, and watch-tracker apps build out person, film, and series pages using TMDB as the authoritative source. |
| Second-Screen Experiences | Companion apps surface cast, trivia, and where-to-watch data while users are watching a film or show. |
| Media Asset Management | PMS-style libraries (Plex, Jellyfin, Kodi) match local files to TMDB IDs to pull metadata and artwork for personal media. |
| AI/ML Research Datasets | Researchers build movie/TV datasets for embeddings, recommendation, or NLP — subject to TMDB's commercial-use approval for AI training. |

## Integrations

JustWatch, IMDB, TVDb, Plex, Jellyfin, Kodi, Sonarr, Radarr, Letterboxd, Trakt, Stremio, MCP

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [TMDB API (v3, OpenAPI 3.1.0, 148 paths, 152 operations, 149 schemas, 21 tags)](openapi/tmdb-api-openapi-original.yml)

### JSON Schema

149 standalone JSON Schema (Draft 2020-12) files extracted from the OpenAPI components in [json-schema/](json-schema/) — one per response/error envelope schema.

### JSON Structure

149 JSON Structure (json-structure.org v0) representations in [json-structure/](json-structure/) — strict-typed conversion of the JSON Schema files with `int32`/`int64`/`double`/`datetime`/`date`/`uri`/`uuid` first-class types.

### JSON-LD

- [TMDB Context](json-ld/tmdb-context.jsonld) — 149 type declarations + 324 property terms aligned with schema.org (`schema:name`, `schema:datePublished`, `schema:ratingValue`, etc.) and `tmdb:` namespace.

### Examples

149 example response payloads in [examples/](examples/) — one per schema, generated from inline OpenAPI examples and TMDB-domain heuristics.

## Capabilities

21 self-contained Naftiko capability files (one per OpenAPI tag), each with both REST and MCP exposers, in [capabilities/](capabilities/). Listed under the TMDB API entry above.

## Vocabulary

- [TMDB Vocabulary](vocabulary/tmdb-vocabulary.yml) — Unified taxonomy mapping 21 resources, 7 actions, 21 workflows, and 5 personas across operational (OpenAPI) and capability (Naftiko) dimensions.

## Rules

- [TMDB Spectral Ruleset](rules/tmdb-rules.yml) — 42 Spectral rules across 13 categories enforcing TMDB API conventions: path-versioning (/3/, /4/), snake_case paths/parameters/properties, kebab-case operationIds, "TMDB" title and summary prefixes, JSON-only responses, 401/429 error responses, bearer + apiKey auth schemes, and Microcks-compatible mocking extensions.

## Plans & Pricing

- [TMDB Plans](plans/tmdb-plans-pricing.yml) — API Commons Plans 0.1 artifact capturing the Non-Commercial (free, attribution + 6-month cache TTL) and Commercial (negotiated written agreement, custom pricing) tiers.

## Rate Limits

- [TMDB Rate Limits](rate-limits/tmdb-rate-limits.yml) — API Commons Rate Limits 0.1 artifact documenting the ~40 RPS soft ceiling per API key, the 429 response policy, the historical 40-per-10s limit removal (2019-12-16), and seven policies (exponential back-off, caching, append_to_response, daily ID exports, soft-limit reality, no live/sandbox split, no public plan quotas).

## FinOps

- [TMDB FinOps](finops/tmdb-finops.yml) — FOCUS-aligned FinOps 1.0 artifact framing TMDB as a custom (free non-commercial + negotiated commercial) shape with six internal-cost meters (api_requests, image_bytes_egress, cache_age_seconds, daily_id_export_downloads, append_to_response_calls, rate_limit_429_count) and TMDB-specific Visibility/Allocation/Optimization/Accountability principles.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
