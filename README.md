# Noom

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
