# Eligent Public Anchors

This repository is a public publication and mirror location for Eligent anchor material.

It contains only public verification data:

- trusted anchor public key records;
- public ledger anchor records;
- format notes for offline verifiers.

This repository is not the cryptographic root of trust. Verifiers must trust a pinned root key or fingerprint obtained through an independent channel. Content fetched from GitHub is accepted only after the verifier checks the applicable key, purpose, provider, validity window, signature, and digest rules.

Do not commit private keys, signing keys, passwords, recovery codes, API keys, patient data, customer data, or internal system identifiers to this repository.

## Current public locations

- `trusted-anchor-registry/v2/registry.json` - current public registry snapshot.
- `trusted-anchor-registry/v2/registry.sha256` - checksum for the registry snapshot.
- `trusted-anchor-registry/v2/eligent-root-2026-01.json` - current public anchor signing key record.
- `trusted-anchor-registry/v2/eligent-root-2026-01.spki-sha256` - pinned SPKI SHA-256 fingerprint for the current root.
- `anchors/latest-anchor.json` - latest public ledger anchor mirror.
- `anchors/history/` - historical public ledger anchor records.

## Current pinned fingerprint

```text
f11ac208e795e781fbe81b87525b3db0425e8bdafb274dd6806d10d0783b41ad
```

The fingerprint is SHA-256 over the root public key's SubjectPublicKeyInfo DER bytes.

## Verification boundary

GitHub provides availability and transparency. It does not prove signer identity by itself. The verifier must reject any anchor or registry material that does not chain to a root already trusted by the verifier.
