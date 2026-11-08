# Security Policy

## Reporting a vulnerability

Please **do not** open a public issue for security problems.

Use GitHub's private vulnerability reporting:
**Security → Advisories → Report a vulnerability** on this repository.

Include:

- affected package and version,
- a minimal reproduction or proof of concept,
- impact (state corruption, hidden-information leak, code execution, etc.),
- whether the issue affects online play, local play, or package loading.

## Supported versions

| Version | Supported |
| :--- | :--- |
| `0.1.x` and later | ✅ (once published) |
| pre-release / canary | best effort |

## Scope

High-priority areas:

- game-package parsing (zip-slip, zip bombs, path traversal, unsigned packages),
- rule execution sandboxing (no `new Function` / remote code execution),
- socket protocol authentication and hidden-information redaction,
- token storage in desktop/mobile shells,
- supply-chain provenance (npm package attestations).

## Disclosure

We aim to acknowledge reports within 3 business days and to publish a fix and
advisory as soon as practical. Please give us a reasonable window before public
disclosure.
