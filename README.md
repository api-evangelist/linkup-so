# Linkup (linkup-so)

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

Linkup is a production-grade web search and answer API for AI agents and LLMs. Its /search endpoint grounds model responses in real-time web context, returning ranked results, sourced answers with citations, or structured output, plus /fetch for clean LLM-ready markdown, an async /research endpoint, and a credits balance endpoint - all authenticated with a Bearer API key.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/linkup-so/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/linkup-so/refs/heads/main/apis.yml)

## Tags

- AI
- LLM
- Web Search
- Grounding
- RAG

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Linkup Search API

Grounds AI agents and LLMs in real-time web context. POST /search runs a natural-language query at fast, standard, or deep precision and returns ranked search results, a sourced answer with inline citations, or schema-driven structured output, with date, domain, and image filters.

- **Human URL:** [https://docs.linkup.so/pages/documentation/api-reference/endpoint/post-search](https://docs.linkup.so/pages/documentation/api-reference/endpoint/post-search)
- **Base URL:** `https://api.linkup.so/v1`

#### Tags

- Web Search
- Sourced Answer
- Structured Output

#### Properties

- [Documentation](https://docs.linkup.so/pages/documentation/get-started/introduction)
- [API Reference](https://docs.linkup.so/pages/documentation/api-reference/endpoint/post-search)
- [OpenAPI](openapi/linkup-so-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/linkup-so.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linkup-so.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Linkup Fetch API

POST /fetch retrieves the content of a given URL as clean, LLM-ready markdown, with options to render JavaScript, include raw HTML, and extract images.

- **Human URL:** [https://docs.linkup.so/pages/documentation/api-reference/endpoint/post-fetch](https://docs.linkup.so/pages/documentation/api-reference/endpoint/post-fetch)
- **Base URL:** `https://api.linkup.so/v1`

#### Tags

- Fetch
- Markdown
- Content Extraction

#### Properties

- [API Reference](https://docs.linkup.so/pages/documentation/api-reference/endpoint/post-fetch)
- [OpenAPI](openapi/linkup-so-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/linkup-so.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linkup-so.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Linkup Research API

Asynchronous deep-research endpoint (beta). POST /research starts an autonomous web investigation that returns a task id; poll the task until it reaches a terminal state to retrieve a synthesized, cited report.

- **Human URL:** [https://docs.linkup.so/pages/documentation/get-started/introduction](https://docs.linkup.so/pages/documentation/get-started/introduction)
- **Base URL:** `https://api.linkup.so/v1`

#### Tags

- Research
- Async
- Citations

#### Properties

- [Documentation](https://docs.linkup.so/pages/documentation/get-started/introduction)
- [OpenAPI](openapi/linkup-so-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/linkup-so.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linkup-so.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Linkup Credits API

GET /credits/balance returns the number of credits remaining in your account.

- **Human URL:** [https://docs.linkup.so/pages/documentation/api-reference/endpoint/get-balance](https://docs.linkup.so/pages/documentation/api-reference/endpoint/get-balance)
- **Base URL:** `https://api.linkup.so/v1`

#### Tags

- Credits
- Account
- Balance

#### Properties

- [API Reference](https://docs.linkup.so/pages/documentation/api-reference/endpoint/get-balance)
- [OpenAPI](openapi/linkup-so-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/linkup-so.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linkup-so.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/LinkupPlatform)
- [LinkedIn](https://www.linkedin.com/company/linkup-platform)
- [Website](https://www.linkup.so)
- [Documentation](https://docs.linkup.so)
- [Plans](plans/linkup-so-plans-pricing.yml)
- [Rate Limits](rate-limits/linkup-so-rate-limits.yml)
- [Fin Ops](finops/linkup-so-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
