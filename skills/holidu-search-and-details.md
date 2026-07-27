---
name: Search Holidu offers and retrieve details
description: Search vacation-rental offers, page through results, fetch detailed property information, and check real-time availability using the Holidu Affiliate API.
api: openapi/holidu-affiliate-api.json
operations: [search, details, availabilities, changed]
---

# Search Holidu offers and retrieve details

Use the Holidu **Affiliate API** (`https://external-api.holidu.com`) to surface
vacation-rental inventory to travellers.

## Auth
Send your API key in the `x-api-key` header. (Holidu-initiated LOS-push callbacks
to your side use an OAuth 2.0 Bearer JWT instead — see `los-push` in
`asyncapi/holidu-webhooks.yml`.)

## Steps
1. **`search`** — POST `/search` with filter criteria (`searchTerm`,
   `locationBoundingBox`, `checkin`/`checkout`, `adults`/`children`,
   `propertyTypes`, `facilities`, `locale`, `currency`). Page with `pageIndex`
   and `pageSize`; read `metadata.totalCount` and iterate. When dates are given,
   only available offers are returned with exact pricing.
2. **`details`** — POST `/details` for the offer IDs you want to show. Use the
   `extras` parameter to include extra data points. The response includes an
   RFC 6570 `urlTemplate` — expand it with check-in/check-out dates to build the
   checkout link.
3. **`availabilities`** — POST `/availabilities` to re-check real-time prices and
   availability for specific properties and dates before displaying a final price.
4. **`changed`** — POST `/changed` with a time window to get property IDs whose
   data changed, then re-fetch only those (delta sync).

## Conventions & errors
- Batch endpoints return an `errors[]` array alongside `items` — handle
  per-property failures without discarding the whole response.
- `401` = missing/invalid API key; `429` = back off. See
  `errors/holidu-problem-types.yml`.
