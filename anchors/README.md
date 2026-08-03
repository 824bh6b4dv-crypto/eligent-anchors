# Public anchor records

This directory mirrors public Eligent ledger anchor records.

These records publish cryptographic commitments only. They must not contain patient data, customer data, raw artifacts, internal hostnames, private keys, passwords, recovery codes, or API tokens.

Suggested stable paths:

- `latest-anchor.json` - most recent public anchor mirror.
- `history/YYYY-MM-DD.json` - historical public anchor records by anchor date.

GitHub is a publication and transparency location. A verifier must still validate signatures and key identity against an independently trusted key resolver or pinned fingerprint.
