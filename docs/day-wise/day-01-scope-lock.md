# Day 1 - Kickoff + Scope Lock

## Goal

Lock the P0 MVP scope for MarizFirst, freeze the product direction, and remove ambiguity before development begins.

## Summary

MarizFirst will be built as a production healthcare appointment discovery and assisted booking platform. It is not a static directory, coupon platform, emergency care product, or medical advice product.

The MVP booking model is locked: patients can select a preferred slot, but every appointment request starts as Pending Confirmation. A request becomes Confirmed only after an admin or authorized partner confirms it.

## Decisions Completed

- Created the project documentation structure.
- Frozen the MVP product positioning.
- Locked the P0 MVP module scope.
- Marked Phase 1 exclusions clearly to prevent scope creep.
- Confirmed the non-negotiable appointment lifecycle rule: Pending Confirmation first, manual confirmation second.

## Files Created

- `docs/decisions/product-positioning.md`
- `docs/product/mvp-scope-lock.md`
- `docs/day-wise/day-01-scope-lock.md`

## Development Note

Future product, UX, database, and API decisions must follow this Day 1 scope. Any feature that conflicts with assisted booking, pending confirmation, healthcare trust, privacy, or Phase 1 exclusions should be rejected or moved to a later phase.
