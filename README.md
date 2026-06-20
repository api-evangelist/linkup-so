# Linkup (linkup-so)

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
