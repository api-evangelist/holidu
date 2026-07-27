---
name: Manage Holidu rates, availability and length-of-stay pricing
description: Keep an apartment's calendar, rate plans, length-of-stay pricing, extra costs and discounts in sync on the Holidu Connectivity API.
api: openapi/holidu-connectivity-api.json
operations: [updateAvailability, setRates, upsertLos, updateExtraCosts, upsertDiscount, getLosRateIds]
---

# Manage Holidu rates, availability and length-of-stay pricing

Use the Holidu **Connectivity API** with your `api-key` header. Choose one
pricing model per apartment: rate plans (`setRates`) **or** length-of-stay
(`upsertLos`) — pushing the wrong one for your configuration returns `406`.

## Steps
1. **`updateAvailability`** — POST `/v2/availability` to push the availability
   calendar.
2. **`setRates`** — POST `/v2/rates` to push rate plans. Max **500 rate plans**
   per request or you get `413`.
3. **`upsertLos`** — POST `/v2/los` to push length-of-stay pricing. Use
   **`getLosRateIds`** to resolve rate IDs. Upserts fully replace prior data.
4. **`updateExtraCosts`** — POST `/v2/apartments/extracosts` for cleaning fees,
   taxes, etc.
5. **`upsertDiscount`** — POST `/v2/discount` to add or replace a discount.

## Conventions & errors
- Upserts are idempotent full-replacements (RFC 9110). Send the complete dataset.
- `429` = too many concurrent updates for the same apartment; back off and retry
  after the 15-second lock. Full code list in `errors/holidu-problem-types.yml`.
