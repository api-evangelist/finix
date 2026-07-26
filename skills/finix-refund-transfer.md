---
name: Refund a transfer
description: Look up a Transfer and issue a full or partial reversal (refund) with the Finix API.
api: openapi/finix-openapi-original.yml
operations: [getTransfer, createTransferReversal]
generated: '2026-07-19'
method: generated
---

# Refund a transfer

## Auth & conventions
- HTTP Basic auth (RFC 7617) + `Finix-Version: 2022-02-01`.
- Send `idempotency_id` on the reversal so retries do not double-refund.

## Steps
1. **Fetch the Transfer** — `getTransfer` (`GET /transfers/{transfer_id}`); confirm `state` is `SUCCEEDED` or `PENDING`.
2. **Reverse it** — `createTransferReversal` (`POST /transfers/{transfer_id}/reversals`) with `refund_amount` (in cents; omit for a full refund) and `idempotency_id`. Capture the reversal `id`.

## Notes
- List prior reversals with `listTransferReversals`.
- In sandbox, card `4000000000000135` forces a refund `FAILED` state for testing.
- Watch `transfer.updated` webhooks for the reversal outcome.
