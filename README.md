# Noom

Noom, Inc. is a New York-based digital health company founded in 2008 by Saeju Jeong and Artem Petakov. Its psychology-based weight-management app pairs behaviour-change coursework and human coaching with food and activity logging, and — through Noom Med — clinician-prescribed GLP-1 medication. Noom also sells to employers, health plans and health systems.

## API posture (probed 2026-07-31)

**Noom publishes no public API.** There is no developer portal, no OpenAPI/Swagger or GraphQL contract, no AsyncAPI or webhook catalog, no MCP server, no A2A agent card, and no first-party SDKs on npm, PyPI or RubyGems.

- `api.noom.com` — the application backend. Every anonymous request, on every probed path, returns HTTP 401 `{"code":"UNAUTHENTICATED"}`.
- `www.noom.com/wp-json/` — the one anonymously callable, self-describing surface found: the WordPress/Altis REST API behind the marketing site and blog (390 routes, 23 namespaces). A CMS content API, not a Noom product API. See `discovery/`.
- `healthcare.noom.com` — a single-page healthcare client application (login-gated).
- Health-system EHR integration is described as a business capability only, with no published specification.

## Links

- https://www.noom.com/
- https://www.noom.com/health/ — employers, health plans, health systems
- https://trust.noom.com/ — Vanta-hosted trust center
- https://github.com/noom
- https://forgeglobal.com/noom_stock/
