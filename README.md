# Kimi (Moonshot AI) (kimi-moonshot)

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

Moonshot AI is a Beijing-based AI lab that develops the Kimi family of long-context multilingual large language models. The consumer assistant is available at kimi.com (and kimi.ai); the developer platform at platform.moonshot.cn (also platform.kimi.com / platform.kimi.ai) exposes an OpenAI-compatible REST API for chat completions, embeddings, file management, fine-tuning, and model listing. Kimi models advertise very long context windows (8K, 32K, 128K, with newer K2.x models pushing toward 256K) and the platform offers multimodal text, image, and video inputs on the flagship Kimi K2.x line. Open-source weights for prior Kimi releases live under the MoonshotAI GitHub organization.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/kimi-moonshot/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/kimi-moonshot/refs/heads/main/apis.yml)

## Tags

- LLM
- Long Context
- AI
- OpenAI Compatible
- Multimodal
- China

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-05-29

## APIs

### Kimi Chat Completions API

OpenAI-compatible chat completions endpoint. Accepts a messages array, model identifier (moonshot-v1-8k / 32k / 128k, kimi-k2.5, kimi-k2.6), and standard sampling parameters. Supports streaming responses, function/tool calling, and JSON mode.

- **Human URL:** [https://platform.moonshot.cn/docs](https://platform.moonshot.cn/docs)
- **Base URL:** `https://api.moonshot.cn/v1/chat/completions`

#### Tags

- Chat
- LLM
- OpenAI Compatible
- Streaming
- SSE

#### Properties

- [Documentation](https://platform.moonshot.cn/docs)
- [OpenAPI](openapi/kimi-moonshot-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kimi-moonshot.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kimi-moonshot.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/kimi-moonshot-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Kimi Embeddings API

OpenAI-compatible embeddings endpoint that returns vector representations of input text for semantic search, clustering, and retrieval-augmented generation workflows.

- **Human URL:** [https://platform.moonshot.cn/docs](https://platform.moonshot.cn/docs)
- **Base URL:** `https://api.moonshot.cn/v1/embeddings`

#### Tags

- Embeddings
- Vectors

#### Properties

- [Documentation](https://platform.moonshot.cn/docs)
- [Postman Collection](collections/kimi-moonshot.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kimi-moonshot.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kimi Files API

File management endpoint for uploading documents that can be referenced from chat completions (for example, long-document Q&A and the file_id-based context attachment pattern).

- **Human URL:** [https://platform.moonshot.cn/docs](https://platform.moonshot.cn/docs)
- **Base URL:** `https://api.moonshot.cn/v1/files`

#### Tags

- Files
- Documents

#### Properties

- [Documentation](https://platform.moonshot.cn/docs)
- [Postman Collection](collections/kimi-moonshot.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kimi-moonshot.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kimi Fine-Tuning API

Fine-tuning jobs endpoint for customizing Moonshot base models on customer-supplied training data. Mirrors the OpenAI fine-tuning surface.

- **Human URL:** [https://platform.moonshot.cn/docs](https://platform.moonshot.cn/docs)
- **Base URL:** `https://api.moonshot.cn/v1/fine_tuning`

#### Tags

- Fine-Tuning
- Training

#### Properties

- [Documentation](https://platform.moonshot.cn/docs)
- [Postman Collection](collections/kimi-moonshot.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kimi-moonshot.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kimi Models API

Lists models available to the authenticated account and exposes per-model metadata (context window, modality support, pricing tier).

- **Human URL:** [https://platform.moonshot.cn/docs](https://platform.moonshot.cn/docs)
- **Base URL:** `https://api.moonshot.cn/v1/models`

#### Tags

- Models
- Catalog

#### Properties

- [Documentation](https://platform.moonshot.cn/docs)
- [Postman Collection](collections/kimi-moonshot.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kimi-moonshot.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kimi Tokenizer API

Helper endpoint exposed by the Moonshot platform for counting tokens against a given model's tokenizer prior to submission, useful for managing long-context budgets.

- **Human URL:** [https://platform.moonshot.cn/docs](https://platform.moonshot.cn/docs)
- **Base URL:** `https://api.moonshot.cn/v1/tokenizers`

#### Tags

- Tokenizer
- Utilities

#### Properties

- [Documentation](https://platform.moonshot.cn/docs)
- [Postman Collection](collections/kimi-moonshot.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kimi-moonshot.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kimi Assistant (kimi.com)

Consumer-facing AI assistant at kimi.com (also kimi.ai) powered by the Kimi models. Supports long-document upload, web search grounding, and tool use through a chat UI.

- **Human URL:** [https://kimi.com/](https://kimi.com/)
- **Base URL:** `https://kimi.com/`

#### Tags

- Assistant
- Consumer

#### Properties

- [Website](https://kimi.com/)
- [Postman Collection](collections/kimi-moonshot.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kimi-moonshot.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Moonshot Open-Weights Releases

Open-weight Kimi model releases (for example prior Kimi K1 / K2 checkpoints) published under the MoonshotAI GitHub organization for research and self-hosted use.

- **Human URL:** [https://github.com/MoonshotAI](https://github.com/MoonshotAI)
- **Base URL:** `https://github.com/MoonshotAI`

#### Tags

- Open Weights
- Research

#### Properties

- [Repository](https://github.com/MoonshotAI)
- [Postman Collection](collections/kimi-moonshot.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kimi-moonshot.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.moonshot.cn/)
- [Assistant](https://kimi.com/)
- [Platform](https://platform.moonshot.cn/)
- [Documentation](https://platform.moonshot.cn/docs)
- [Git Hub](https://github.com/MoonshotAI)
- [Hugging Face](https://huggingface.co/moonshotai)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
