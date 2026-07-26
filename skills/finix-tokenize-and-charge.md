---
name: Tokenize and charge a buyer
description: Convert a finix.js browser token into a Payment Instrument and create a Transfer (sale) with the Finix API.
api: openapi/finix-openapi-original.yml
operations: [createPaymentInstrument, createTransfer]
generated: '2026-07-19'
method: generated
---

# Tokenize and charge a buyer

## Auth & conventions
- HTTP Basic auth (RFC 7617) + `Finix-Version: 2022-02-01`.
- Collect card/bank data client-side with finix.js `Finix.PaymentForm` (`https://js.finix.com/v/2/finix.js`) — never handle raw PAN server-side unless PCI-certified.
- Always send `idempotency_id` on `createTransfer` to prevent double charges on retry.

## Steps
1. **Create a Payment Instrument from the token** — `createPaymentInstrument` (`POST /payment_instruments`) with `token` (from `Finix.PaymentForm` onSubmit) and the buyer `identity`. Capture `id` (PIxxxx).
2. **Charge** — `createTransfer` (`POST /transfers`) with `amount`, `currency`, `source` (the PIxxxx), `merchant`, and `idempotency_id`. A successful sale returns `state: SUCCEEDED` (or `PENDING` for ACH).

## Notes
- Refund via the `refundTransfer` flow (`createTransferReversal`).
- Decline handling: inspect `failure_code`/`failure_message`; see `errors/finix-decline-codes.yml`.
