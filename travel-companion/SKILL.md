---
name: travel-companion
description: Plan a multi-day trip from research through a practical mobile travel assistant, including reservations, photo references, safety, preparation, and shared expense settlement. Use when a user wants end-to-end trip planning or a travel companion website; do not use for a single travel fact or one-off booking question.
---

# Travel Companion

Create a trip that can actually be followed on a phone, not merely a polished itinerary. Work in the requested scope: research and planning, a mobile travel assistant, or both.

## Start with the trip brief

Establish only the decisions that change the plan: dates and cities, travelers, pace and priorities, confirmed transport/lodging/reservations, budget or constraints, and whether the user wants a shareable site. Keep confirmed items distinct from suggestions and options.

When researching time-sensitive details such as opening hours, ticket releases, closures, strikes, prices, or transport, verify against official sources first. State what is confirmed, what is a recommendation, and what the traveler must still check. Do not book, pay, or send messages without explicit authorization.

## Plan before styling

Build a day-by-day operational plan with:

- fixed commitments and the arrival buffer they require;
- route order, transfers, and a realistic stopping point;
- one clearly labelled backup for weather, fatigue, disruptions, or sold-out tickets;
- actionable arrival, check-in, luggage, and anti-theft instructions where relevant.

Use the user's original guidance in full where it helps someone execute the trip. Do not replace concrete instructions with generic travel prose.

## Build the mobile assistant only after the plan is usable

Favor clear information hierarchy and touch-friendly interactions over decorative complexity. A travel site may include daily plans, tickets, stays, map links, photo references, safety, preparation, food options, and expense settlement. Keep information that is needed while standing on the street short, visible, and easy to copy or open.

Photo references should be organized by place or moment and shown as images with their source links; do not add filler copy. Keep multiple references as a swipeable or clearly grouped gallery.

For changes to a confirmed plan, preserve the original item and show the reason and replacement rather than silently deleting history.

## Shared expenses

If more than one traveler must see or edit expenses, use a persistent shared backend. Browser local storage alone is not a shared ledger. Support payer, date, original currency, category, note, participants, and equal split calculation. Preserve original currencies separately unless the user explicitly supplies an exchange-rate rule.

Before migrating a local-only ledger, read [shared-ledger.md](references/shared-ledger.md). For privacy and data handling, read [trip-data-boundaries.md](references/trip-data-boundaries.md).

## Deliver and maintain

Before publishing, verify the mobile layout, core links, ticket opening behavior, map links, password/access flow if used, and every shared-data endpoint. Explain any hosting cost, access limitation, or refresh behavior honestly. Deploy only with the user's authorization and return the final share link.

Treat the end of the trip as a closeout phase: keep a final expense export/settlement view and preserve the itinerary as an archive. Do not reuse private trip data in later trips unless the user explicitly provides it again.
