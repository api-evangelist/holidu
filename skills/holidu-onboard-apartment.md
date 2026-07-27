---
name: Onboard an apartment to Holidu
description: Create or update an apartment on the Holidu Connectivity API, attach descriptions, photos and facilities, validate it, and activate it for distribution.
api: openapi/holidu-connectivity-api.json
operations: [upsertApartment, upsertApartmentDescriptions, updatePhotos, updateFacilities, getApartmentValidation, activateApartment, deactivateApartment]
---

# Onboard an apartment to Holidu

Use the Holidu **Connectivity API**. Test against
`https://provider-api-sandbox.holidu.com` first, then
`https://provider-api.holidu.com` for production.

## Auth
Send your partner key in the `api-key` header.

## Steps
1. **`upsertApartment`** — POST `/v2/apartment` with the full apartment payload.
   Upserts are full-replace (RFC 9110 semantics) — always send the complete
   representation.
2. **`upsertApartmentDescriptions`** — POST `/v2/description` to attach localized
   descriptions.
3. **`updatePhotos`** — POST `/v2/photos` with the apartment's photo set.
4. **`updateFacilities`** — POST `/v2/facilities` (use `getFacilityTypes` /
   `getFacilityLocations` to look up valid values).
5. **`getApartmentValidation`** — GET `/v2/apartment/validation` and resolve any
   issues (a `418` signals a business-rule validation failure).
6. **`activateApartment`** — PUT `/v2/apartment/activate` once valid. Use
   **`deactivateApartment`** (PUT `/v2/apartment/deactivate`) to pull it.

## Conventions & errors
- Only one in-flight update per apartment; concurrent same-apartment updates
  return `429`, with a 15-second lock after an interrupted update. Parallelize
  across *different* apartments only. See `conventions/holidu-conventions.yml`.
