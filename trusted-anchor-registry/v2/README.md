# Trusted anchor registry v2

This directory publishes the current public anchor-signing key registry.

Current pinned root fingerprint:

```text
f11ac208e795e781fbe81b87525b3db0425e8bdafb274dd6806d10d0783b41ad
```

Fingerprint algorithm:

```text
SHA-256 over SubjectPublicKeyInfo DER bytes
```

A verifier may fetch `registry.json` from this repository, but must not trust the fetched registry merely because it came from GitHub. The verifier must compare the fetched key's SPKI fingerprint to a value already trusted through an independent pinned configuration or equivalent root-installation process.

The file `registry.sha256` is a content-addressing aid for detecting accidental drift in this repository. It is not a substitute for the pinned root fingerprint and is not a signature.

Production signing note: the registry should later be accompanied by a detached signature produced by an offline registry-signing key or by a release artifact signed under the approved release process. Do not generate or store private signing keys in this repository.
