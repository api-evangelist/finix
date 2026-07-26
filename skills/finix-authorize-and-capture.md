---
name: Authorize and capture a card payment
description: Place a hold on a card with an Authorization, then capture the funds, using the Finix API.
api: openapi/finix-openapi-original.yml
operations: [createIdentity, createPaymentInstrument, createAuthorization, captureAuthorization]
generated: '2026-07-19'
method: generated
---

# Authorize and capture a card payment

## Auth & conventions
- HTTP Basic auth (RFC 7617) + `Finix-Version: 2022-02-01`.
- Pass `idempotency_id` on `createAuthorization` to make retries safe.
- Errors: HAL `_embedded.errors[]`; card declines carry `failure_code`/`failure_message` (see `errors/finix-decline-codes.yml`).

## Steps
1. **Create the buyer Identity** — `createIdentity` (`POST /identities`).
2. **Add the card** — `createPaymentInstrument` (`POST /payment_instruments`) with `type: PAYMENT_CARD` and the buyer `identity`. In sandbox, card `4242424242424242` returns `RESTRICTED_CARD`; use a type-testing card such as `5200820000007201` for a clean approval.
3. **Authorize** — `createAuthorization` (`POST /authorizations`) with `amount`, `currency`, `merchant_identity`, and `source` (the instrument). Capture `id` (AUxxxx).
4. **Capture** — `captureAuthorization` (`PUT /authorizations/{authorization_id}`) with `capture_amount`. The response `transfer` links the resulting Transfer (TRxxxx).

## Notes
- To release a hold instead of capturing, call `voidAuthorization`.
- Subscribe to `authorization.updated` and `transfer.updated` webhooks for state changes.
