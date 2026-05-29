# Noun Project (noun-project)

The Noun Project is a visual language platform providing access to nearly 10 million royalty-free PNG and SVG icons through an OAuth 1.0a-secured REST API. The v2 API supports icon search with style and line-weight filtering, similar-icon lookup, collection browsing, custom recoloring, autocomplete, per-client blocklists, and usage telemetry. Built on AWS, it serves more than 300 million requests per month at 99.99% uptime.

**URL:** [Visit APIs.json URL](http://api.thenounproject.com/index.html)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Art And Design, Icons, SVG, Visual Language, Design Assets, Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-28

## APIs

### Noun Project API V2

OAuth 1.0a-secured REST API for searching and retrieving icons, collections, autocomplete suggestions, and usage statistics from the Noun Project's library of nearly 10 million royalty-free icons. Supports style filtering, line-weight filtering, hex color recoloring, multiple thumbnail sizes, SVG download, similar-icon discovery, and per-client blocklists.

**Human URL:** [https://api.thenounproject.com/documentation.html](https://api.thenounproject.com/documentation.html)

#### Tags:

 - Icons, Search, Collections, Visual Language

#### Properties

- [Documentation](https://api.thenounproject.com/documentation.html)
- [GettingStarted](https://api.thenounproject.com/getting_started.html)
- [SignUp](https://thenounproject.com/developers/apps/)
- [APIExplorer](https://api.thenounproject.com/explorer)
- [Authentication](https://api.thenounproject.com/getting_started.html)
- [OpenAPI](openapi/noun-project-openapi.yml)
- [NaftikoCapability](capabilities/noun-project-icon.yaml)
- [NaftikoCapability](capabilities/noun-project-collection.yaml)
- [NaftikoCapability](capabilities/noun-project-autocomplete.yaml)
- [NaftikoCapability](capabilities/noun-project-blocklist.yaml)
- [NaftikoCapability](capabilities/noun-project-usage.yaml)

## Common Properties

- [Website](https://thenounproject.com/)
- [Pricing](https://thenounproject.com/api/)
- [SignUp](https://thenounproject.com/developers/apps/)
- [Support](https://thenounproject.zendesk.com/)
- [HelpCenter](https://help.thenounproject.com/)
- [GitHubOrganization](https://github.com/TheNounProject)
- [TermsOfService](https://thenounproject.com/legal/api-terms-of-use/)
- [PublicAPIsListing](https://github.com/public-apis/public-apis)
- [Plans](plans/noun-project-plans-pricing.yml)
- [RateLimits](rate-limits/noun-project-rate-limits.yml)
- [FinOps](finops/noun-project-finops.yml)
- [Vocabulary](vocabulary/noun-project-vocabulary.yml)
- [SpectralRules](rules/noun-project-rules.yml)

## Features

| Name | Description |
|------|-------------|
| Icon Search | Search nearly 10 million icons by query term, with optional filters for style (solid/line), line weight (1-60 pixels at 512px rendering), public domain status, and thumbnail size. |
| Similar Icons | Discover stylistically similar icons by providing a seed icon ID, enabling consistent visual language across a project. |
| Icon Download with Recoloring | Download any icon in SVG or PNG format with a custom hexadecimal color and pixel size (20-1200 for PNG). |
| Collection Browsing | Search and retrieve curated icon collections (icon sets) with full metadata and member icons. |
| Autocomplete | Suggest search terms based on a query prefix, returning up to 10 matches. |
| Per-Client Blocklist | Maintain a per-API-key blocklist of icon IDs, collection IDs, terms, and phrases to filter out unwanted content from search results. Blocklist is cached for 10 minutes. |
| Usage Telemetry | Retrieve current API key usage against hourly, daily, and monthly limits via the /v2/client/usage endpoint. |

## Use Cases

| Name | Description |
|------|-------------|
| Icon Library Integration | Embed Noun Project's visual language into a design tool, no-code builder, or web/mobile application so end users can pick from millions of icons without leaving the host product. |
| Branded Iconography | Recolor icons to match brand palettes on the fly using the hex color parameter on the download endpoint, eliminating per-icon design work. |
| Style-Consistent Design Systems | Use the more-like-this endpoint to source visually consistent icon sets from a single seed icon, accelerating design system curation. |
| Content Moderation | Apply per-client blocklists to suppress icons that conflict with brand safety, regional, or audience-appropriate guidelines. |
| Educational and Reference Tools | Pair the autocomplete and icon search endpoints to power glossary-style visual references and learning tools. |

## Integrations

| Name | Description |
|------|-------------|
| OAuth 1.0a Client Libraries | Compatible with any standards-compliant OAuth 1.0a library, including requests_oauthlib (Python), oauth1 (Node.js), Faraday-OAuth (Ruby), DotNetOpenAuth (.NET), and Guzzle OAuth Subscriber (PHP). |
| Sketch | The provider maintains Sketch plugin tooling (SketchPluginReloader) and historically distributed a Noun Project Sketch plugin. |
| Microsoft Office and Google Workspace | Provider-distributed plugins for Microsoft 365 and Google Slides surface the same icon catalog backed by this API. |

## Solutions

| Name | Description |
|------|-------------|
| Design Tool Vendors | Power icon pickers, asset browsers, and template galleries inside design, presentation, and document-creation tools. |
| Marketing and Brand Teams | On-demand recoloring of icons to enforce brand palettes across web, print, and presentation assets. |
| Education Platforms | Add visual reference material to learning content with royalty-free, commercially-licensed icons. |
| No-Code and Low-Code Builders | Expose a curated icon library to citizen developers building dashboards, portals, and forms. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Noun Project API V2](openapi/noun-project-openapi.yml)

### JSON Schema

16 schemas extracted from the Noun Project API V2 OpenAPI spec:

- [Autocomplete Response](json-schema/noun-project-autocomplete-response-schema.json)
- [Blocklist](json-schema/noun-project-blocklist-schema.json)
- [Blocklist ID Request](json-schema/noun-project-blocklist-id-request-schema.json)
- [Blocklist Response](json-schema/noun-project-blocklist-response-schema.json)
- [Blocklist Term Request](json-schema/noun-project-blocklist-term-request-schema.json)
- [Collection](json-schema/noun-project-collection-schema.json)
- [Collection Response](json-schema/noun-project-collection-response-schema.json)
- [Collection Search Response](json-schema/noun-project-collection-search-response-schema.json)
- [Icon](json-schema/noun-project-icon-schema.json)
- [Icon Creator](json-schema/noun-project-icon-creator-schema.json)
- [Icon Response](json-schema/noun-project-icon-response-schema.json)
- [Icon Search Response](json-schema/noun-project-icon-search-response-schema.json)
- [Tag](json-schema/noun-project-tag-schema.json)
- [Usage](json-schema/noun-project-usage-schema.json)
- [Usage Response](json-schema/noun-project-usage-response-schema.json)
- [Usage Window](json-schema/noun-project-usage-window-schema.json)

### JSON Structure

16 JSON Structure files converted from the JSON Schema set:

- [Autocomplete Response](json-structure/noun-project-autocomplete-response-structure.json)
- [Blocklist](json-structure/noun-project-blocklist-structure.json)
- [Blocklist ID Request](json-structure/noun-project-blocklist-id-request-structure.json)
- [Blocklist Response](json-structure/noun-project-blocklist-response-structure.json)
- [Blocklist Term Request](json-structure/noun-project-blocklist-term-request-structure.json)
- [Collection](json-structure/noun-project-collection-structure.json)
- [Collection Response](json-structure/noun-project-collection-response-structure.json)
- [Collection Search Response](json-structure/noun-project-collection-search-response-structure.json)
- [Icon](json-structure/noun-project-icon-structure.json)
- [Icon Creator](json-structure/noun-project-icon-creator-structure.json)
- [Icon Response](json-structure/noun-project-icon-response-structure.json)
- [Icon Search Response](json-structure/noun-project-icon-search-response-structure.json)
- [Tag](json-structure/noun-project-tag-structure.json)
- [Usage](json-structure/noun-project-usage-structure.json)
- [Usage Response](json-structure/noun-project-usage-response-structure.json)
- [Usage Window](json-structure/noun-project-usage-window-structure.json)

### JSON-LD

- [Noun Project Context](json-ld/noun-project-context.jsonld) — 82-term JSON-LD 1.1 context aligning schema properties with schema.org and the np: namespace.

### Examples

16 example payloads, one per JSON Schema:

- [examples/](examples/)

## Capabilities

Naftiko capabilities for the Noun Project API, one self-contained file per OpenAPI tag. Each file declares both a REST and an MCP exposer routed inline through its own consumes block.

### Noun Project API V2

| Capability | Operations | REST + MCP | File |
|------------|-----------:|-----------:|------|
| Icon | 4 | 4 + 4 | [capabilities/noun-project-icon.yaml](capabilities/noun-project-icon.yaml) |
| Collection | 2 | 2 + 2 | [capabilities/noun-project-collection.yaml](capabilities/noun-project-collection.yaml) |
| Autocomplete | 1 | 1 + 1 | [capabilities/noun-project-autocomplete.yaml](capabilities/noun-project-autocomplete.yaml) |
| Blocklist | 3 | 3 + 3 | [capabilities/noun-project-blocklist.yaml](capabilities/noun-project-blocklist.yaml) |
| Usage | 1 | 1 + 1 | [capabilities/noun-project-usage.yaml](capabilities/noun-project-usage.yaml) |

## Vocabulary

- [Noun Project Vocabulary](vocabulary/noun-project-vocabulary.yml) — Unified taxonomy mapping 5 resources, 7 actions, 5 workflows, and 6 personas across operational (OpenAPI) and capability (Naftiko) dimensions.

## Rules

- [Noun Project Spectral Rules](rules/noun-project-rules.yml) — 46 rules across 13 categories enforcing Noun Project API conventions (v2 path prefix, snake_case parameters, Title Case tags, OAuth 1.0a security, kebab-case paths, cursor pagination, thumbnail_size enum).

## Plans, Rate Limits, and FinOps

- [Plans & Pricing](plans/noun-project-plans-pricing.yml) — API Commons Plans 0.1 document covering Free Trial, Pay-Per-Use, and Custom Enterprise tiers.
- [Rate Limits](rate-limits/noun-project-rate-limits.yml) — API Commons Rate Limits 0.1 document covering per-key hourly, daily, and monthly windows split across service-call and icon-call metrics.
- [FinOps](finops/noun-project-finops.yml) — FOCUS-aligned FinOps Framework 1.0 document describing the Pay-As-You-Go + monthly minimum billing model with four meters and the four FinOps principles.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
