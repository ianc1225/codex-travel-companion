# Shared ledger migration and settlement

## Before migration

- Tell every traveler not to clear browser data and to use the same device and browser where they recorded expenses.
- Establish whether existing entries are local-only, shared already, or a mix.
- Keep system-provided seed entries identifiable by stable IDs so they do not duplicate during import.

## Migration behavior

- Each device imports its local user-created entries once.
- Do not repeatedly re-import old browser caches: that can restore entries another traveler intentionally deleted.
- Queue edits made offline and synchronize them deliberately when connection returns.
- Explain that each traveler must complete their own first sync before the group starts editing or deleting shared entries.

## Settlement behavior

- For each currency, calculate paid, owed, and net balance per traveler.
- Net transactions across all shared entries. If one traveler paid some bills but still owes more than their total share, they remain a payer in the final settlement.
- Show the arithmetic in plain language when a user questions a transfer path. Do not force conversion between EUR, USD, and CNY without an agreed rate and date.

## Safety checks

- Confirm shared read and write endpoints after deploy, not only the client UI.
- Add a delete confirmation; explain that deleting a shared entry affects everyone.
- Keep an export or readable itemized list before closing out the trip.
