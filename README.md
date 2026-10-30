# Finix

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

Finix is a full-stack payments technology provider that lets software platforms, marketplaces, and merchants accept and send payments online and in person. The Finix API is a HAL/HATEOAS REST API (HTTP Basic authentication per RFC 7617, date-based Finix-Version header, cursor pagination, idempotency_id) covering Identities, Merchants, Payment Instruments, Authorizations, Transfers, Settlements, Disputes, Fee Profiles, Verifications, Onboarding Forms, Devices, Balance Transfers, Split Transfers, and Webhooks, plus low-code Checkout, Payment Links, Subscriptions, and Payouts. It is Level 1 PCI DSS certified with finix.js browser tokenization, native iOS/Android SDKs, and official Python, Node.js, Java, and PHP client libraries. This profile was enriched from Finix's own public developer surface.

**Areas:** Company · Fintech · Payments · Payment Processing · Payment Facilitation · Merchant Onboarding · Payouts · Marketplace · Embedded Finance · ACH · Card Acceptance · PCI DSS

## Finix on APIs.io

Everything profiled for Finix is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/finix/](https://apis.io/providers/finix/)** — or go straight to one of the APIs or properties below.

### APIs (19)

- [Finix Authorizations API](https://apis.io/apis/finix/finix-authorizations-api/) — {'$ref': 'api-descriptions/tags/authorizations.md'}
- [Finix Balance Transfers API](https://apis.io/apis/finix/finix-balance-transfers-api/) — {'$ref': 'api-descriptions/tags/balance-transfers.md'}
- [Finix Compliance Forms API](https://apis.io/apis/finix/finix-compliance-forms-api/) — {'$ref': 'api-descriptions/tags/compliance-forms.md'}
- [Finix Devices API](https://apis.io/apis/finix/finix-devices-api/) — {'$ref': 'api-descriptions/tags/devices.md'}
- [Finix Disputes API](https://apis.io/apis/finix/finix-disputes-api/) — {'$ref': 'api-descriptions/tags/disputes.md'}
- [Finix Fee Profiles API](https://apis.io/apis/finix/finix-fee-profiles-api/) — {'$ref': 'api-descriptions/tags/fee-profiles.md'}
- [Finix Files API](https://apis.io/apis/finix/finix-files-api/) — {'$ref': 'api-descriptions/tags/files.md'}
- [Finix Identities API](https://apis.io/apis/finix/finix-identities-api/) — {'$ref': 'api-descriptions/tags/identities.md'}
- [Finix Instrument Updates API](https://apis.io/apis/finix/finix-instrument-updates-api/) — {'$ref': 'api-descriptions/tags/instrument-updates.md'}
- [Finix Merchant Profiles API](https://apis.io/apis/finix/finix-merchant-profiles-api/) — {'$ref': 'api-descriptions/tags/merchant-profiles.md'}
- [Finix Merchants API](https://apis.io/apis/finix/finix-merchants-api/) — {'$ref': 'api-descriptions/tags/merchants.md'}
- [Finix Onboarding Forms API](https://apis.io/apis/finix/finix-onboarding-forms-api/) — {'$ref': 'api-descriptions/tags/onboarding-forms.md'}
- [Finix Payment Instruments API](https://apis.io/apis/finix/finix-payment-instruments-api/) — {'$ref': 'api-descriptions/tags/payment-instruments.md'}
- [Finix Payout Profiles API](https://apis.io/apis/finix/finix-payout-profiles-api/) — {'$ref': 'api-descriptions/tags/payout-profiles.md'}
- [Finix Settlements API](https://apis.io/apis/finix/finix-settlements-api/) — {'$ref': 'api-descriptions/tags/settlements.md'}
- [Finix Split Transfers API](https://apis.io/apis/finix/finix-split-transfers-api/) — {'$ref': 'api-descriptions/tags/split-transfers.md'}
- [Finix Transfers API](https://apis.io/apis/finix/finix-transfers-api/) — {'$ref': 'api-descriptions/tags/transfers.md'}
- [Finix Verifications API](https://apis.io/apis/finix/finix-verifications-api/) — {'$ref': 'api-descriptions/tags/verifications.md'}
- [Finix Webhooks API](https://apis.io/apis/finix/finix-webhooks-api/) — {'$ref': 'api-descriptions/tags/webhooks.md'}

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (4)

Multi-step workflows that chain operations into a business task.

- [Finix Authorize and Capture](https://apis.io/arazzos/finix/finix-authorize-and-capture-workflow/)
- [Finix Onboard Merchant](https://apis.io/arazzos/finix/finix-onboard-merchant-workflow/)
- [Finix Refund Transfer](https://apis.io/arazzos/finix/finix-refund-transfer-workflow/)
- [Finix Tokenize and Charge](https://apis.io/arazzos/finix/finix-tokenize-and-charge-workflow/)

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Finix Webhook Events](https://apis.io/asyncapis/finix/finix-events-asyncapi/)

#### Event channels (12)

Individual events and webhooks the provider emits.

- [authorization](https://apis.io/channels/finix/authorization/)
- [dispute](https://apis.io/channels/finix/dispute/)
- [fee](https://apis.io/channels/finix/fee/)
- [file](https://apis.io/channels/finix/file/)
- [gateway_integration](https://apis.io/channels/finix/gateway-integration/)
- [identity](https://apis.io/channels/finix/identity/)
- [instrument](https://apis.io/channels/finix/instrument/)
- [low_code](https://apis.io/channels/finix/low-code/)
- [merchant](https://apis.io/channels/finix/merchant/)
- [settlement](https://apis.io/channels/finix/settlement/)
- [transfer](https://apis.io/channels/finix/transfer/)
- [verification](https://apis.io/channels/finix/verification/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [Finix MCP Server](https://apis.io/servers/finix/finix-mcp-server/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Finix Agentic Access](https://apis.io/agentic-access/finix/finix-agentic-access/)

#### Collections (38)

Postman and Open Collection request collections.

- [Finix Authorizations API](https://apis.io/collections/finix/open-finix-authorizations-api/)
- [Finix Authorizations Balance Transfers API](https://apis.io/collections/finix/open-finix-balance-transfers-api/)
- [Finix Authorizations Compliance Forms API](https://apis.io/collections/finix/open-finix-compliance-forms-api/)
- [Finix Authorizations Devices API](https://apis.io/collections/finix/open-finix-devices-api/)
- [Finix Authorizations Disputes API](https://apis.io/collections/finix/open-finix-disputes-api/)
- [Finix Authorizations Fee Profiles API](https://apis.io/collections/finix/open-finix-fee-profiles-api/)
- [Finix Authorizations Files API](https://apis.io/collections/finix/open-finix-files-api/)
- [Finix Authorizations Identities API](https://apis.io/collections/finix/open-finix-identities-api/)
- [Finix Authorizations Instrument Updates API](https://apis.io/collections/finix/open-finix-instrument-updates-api/)
- [Finix Authorizations Merchant Profiles API](https://apis.io/collections/finix/open-finix-merchant-profiles-api/)
- [Finix Authorizations Merchants API](https://apis.io/collections/finix/open-finix-merchants-api/)
- [Finix Authorizations Onboarding Forms API](https://apis.io/collections/finix/open-finix-onboarding-forms-api/)
- [Finix Authorizations Payment Instruments API](https://apis.io/collections/finix/open-finix-payment-instruments-api/)
- [Finix Authorizations Payout Profiles API](https://apis.io/collections/finix/open-finix-payout-profiles-api/)
- [Finix Authorizations Settlements API](https://apis.io/collections/finix/open-finix-settlements-api/)
- [Finix Authorizations Split Transfers API](https://apis.io/collections/finix/open-finix-split-transfers-api/)
- [Finix Authorizations Transfers API](https://apis.io/collections/finix/open-finix-transfers-api/)
- [Finix Authorizations Verifications API](https://apis.io/collections/finix/open-finix-verifications-api/)
- [Finix Authorizations Webhooks API](https://apis.io/collections/finix/open-finix-webhooks-api/)
- [Finix Authorizations API](https://apis.io/collections/finix/postman-finix-authorizations-api/)
- [Finix Authorizations Balance Transfers API](https://apis.io/collections/finix/postman-finix-balance-transfers-api/)
- [Finix Authorizations Compliance Forms API](https://apis.io/collections/finix/postman-finix-compliance-forms-api/)
- [Finix Authorizations Devices API](https://apis.io/collections/finix/postman-finix-devices-api/)
- [Finix Authorizations Disputes API](https://apis.io/collections/finix/postman-finix-disputes-api/)
- [Finix Authorizations Fee Profiles API](https://apis.io/collections/finix/postman-finix-fee-profiles-api/)
- …and 13 more published on APIs.io

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Finix Openapi Overlay](https://apis.io/overlays/finix/finix-openapi-overlay/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Finix Authentication](https://apis.io/security/finix/finix-authentication/)
- [Finix Domain Security](https://apis.io/security/finix/finix-domain-security/)
- [Finix Trust Center](https://apis.io/security/finix/finix-trust-center/)
- [Finix Vulnerability Disclosure](https://apis.io/security/finix/finix-vulnerability-disclosure/)

#### Rate limits (1)

Published request limits.

- [Finix Rate Limits](https://apis.io/rate-limits/finix/finix-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://finix.com/)
- [Documentation](https://docs.finix.com/)
- [Getting started](https://docs.finix.com/guides/getting-started)
- [API reference](https://docs.finix.com/api)
- [Pricing](https://finix.com/pricing)
- [Sign up](https://finix.payments-dashboard.com/signup)
- [Support](https://docs.finix.com/guides/getting-started/support-at-finix)
- [Blog](https://finix.com/resources/blogs)
- [Security](https://trust.finix.com/)
- [Compliance](https://trust.finix.com/)
- [Terms of service](https://finix.com/terms-and-policies)
- [Privacy policy](https://finix.com/terms-and-policies/privacy-policy)
- [GitHub](https://github.com/finix-payments)
- [Status](https://status.finix.com/)

## API Evangelist rating

**Kin Score 61.9** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 71.7 |
| Contract quality | 57.0 |
| Contract governance | 18.2 |
| Operational transparency | 73.7 |
| Developer ergonomics | 74.4 |
| Access clarity | 53.9 |

**Agent readiness 43.3** — agent-native

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | verified |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 44.6** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/finix/](https://apis.io/providers/finix/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Finix: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/finix/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
