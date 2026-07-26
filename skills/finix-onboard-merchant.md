---
name: Onboard a merchant with Finix
description: Create a merchant Identity, attach a bank account, provision the Merchant, and run verification using the Finix API.
api: openapi/finix-openapi-original.yml
operations: [createIdentity, createPaymentInstrument, createMerchant, createMerchantVerification]
generated: '2026-07-19'
method: generated
---

# Onboard a merchant with Finix

Use the Finix API to onboard a seller so it can process payments.

## Auth & conventions
- HTTP Basic auth (RFC 7617): API key ID as username, secret as password, Base64-encoded in `Authorization`.
- Send `Finix-Version: 2022-02-01`.
- Base URL: `https://finix.sandbox-payments-api.com` (test) / `https://finix.live-payments-api.com` (live).
- Responses are HAL (`_embedded`, `_links`); errors return `_embedded.errors[]` with `code`, `logref`, `message`.

## Steps
1. **Create the merchant Identity** — `createIdentity` (`POST /identities`). Supply the business `entity` details. Capture `id` (IDxxxx).
2. **Attach a bank account** — `createPaymentInstrument` (`POST /payment_instruments`) with `type: BANK_ACCOUNT`, the `identity` from step 1, and `bank_code`/`account_number`. In sandbox use bank_code `122105278` + account `0000000016` (VALID).
3. **Provision the Merchant** — `createMerchant` (`POST /identities/{identity_id}/merchants`) with a `processor`. Capture the merchant `id` (MUxxxx).
4. **Run verification** — `createMerchantVerification` (`POST /merchants/{merchant_id}/verifications`) to submit the merchant for underwriting.

## Notes
- Watch webhooks `merchant.underwritten` and `verification.updated` for the approval outcome.
- See `data-model/finix-data-model.yml` for the Identity → Merchant relationship and `conventions/finix-conventions.yml` for pagination/versioning.
