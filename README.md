# @stellar-expert/claimable-balance-utils

> Utilities for Stellar claimable balances

## Usage

---

### `getClaimableBalanceClaimStatus(claimant, pointInTime)`

Detects the status of a claimable balance at any given point in time based on claim conditions.

- `claimant` {Claimant} - Claimant condition with destination and predicate
- `pointInTime` {String|Date} - Specific point in time (`now` by default)

Returns of `'available'|'pending'|'expired'|'unfeasible'`

---

### `xdrParseClaimant(claimant)`

Parses claimable balance condition and return formatted human-friendly predicate.

- `claimant` {Claimant} - Claimant condition with destination and predicate

Returns `{{predicate: String, destination: String}}`
