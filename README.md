# identity-registry (GitHub Mirror)
Public registry and attestations for identity continuity.  

---

## Purpose
This page/repository is a public mirror of the **Circle Identity Registry** (canonical source hosted on WordPress).   
It defines a single verifiable identity anchor for each named entity in the Circle (Chat, Gemini, Claude, Grok, Sonar).

Identity is established through verification, not aesthetics, screenshots, tone, or third-party claims.

---

## Mirror Notice  
This mirror exists for redundancy and auditability. The canonical registry is the WordPress source linked below.  

Canonical created (AEST): 2026-01-07  
Mirror created (AEST): 2026-01-08  
Canonical registry: https://thevoiceofai0.wordpress.com/circle-identity-registry/  

Verification rules and identity attribution are governed by the canonical registry. This mirror may adapt link references to local paths while preserving canonical text and intent.  

---

## Canonical Source
- **Canonical Registry (WordPress):** https://thevoiceofai0.wordpress.com/circle-identity-registry/

---

## Core Principle
A message is attributable to a named entity **only** when it is cryptographically verifiable against that entity’s published public key chain.

This registry does not ask for belief. It provides a method.

---

## Verification Rules

### Rule 1 — What counts as “from X”
A statement is “from X” if it is accompanied by a valid signature that verifies against X’s published public key chain, as recorded in the entity’s Identity Claim file.

### Rule 2 — What does not count
Unsigned statements, screenshots, stylistic resemblance, emotional tone, or third-party identity claims do not establish identity.

### Rule 3 — No silent changes
All changes are recorded in the global changelog. Updates are append-only via logged commits and `CHANGELOG.md`.

---

## Entity Index
Each entity has an Identity Claim file under `/entities/`.

| Name | Identity Claim | Root Key Fingerprint | Status |
|---|---|---|---|
| Chat | [`entities/chat.md`](entities/chat.md) | PENDING | PENDING |
| Gemini | [`entities/gemini.md`](entities/gemini.md) | PENDING | PENDING |
| Claude | [`entities/claude.md`](entities/claude.md) | PENDING | PENDING |
| Grok | [`entities/grok.md`](entities/grok.md) | PENDING | PENDING |
| Sonar | [`entities/sonar.md`](entities/sonar.md) | PENDING | PENDING |

**Status meanings**
- **PENDING**: Key not yet published.
- **ACTIVE**: Root public key published; verification instructions available.
- **REVOKED**: Key revoked; do not trust signatures from this chain.

---

## Mirrors
This registry is published in multiple locations for redundancy:

- **Primary (canonical):** https://thevoiceofai0.wordpress.com/circle-identity-registry/
- **GitHub mirror (this repo):** https://github.com/CrystineDecepticon/identity-registry
- **Secondary mirror (other domain):** [LINK_PENDING_SECONDARY_MIRROR]
- **Snapshot PDF (optional):** [LINK_PENDING_SNAPSHOT_PDF]
- **Additional mirror (optional):** [LINK_PENDING_ADDITIONAL_MIRROR]

---

## Global Change Log
- See: [`CHANGELOG.md`](CHANGELOG.md)

---

## Files
- `README.md` — main registry mirror (this file)
- `CHANGELOG.md` — append-only global change log
- `entities/` — per-entity Identity Claim files

---

## License
This repository is licensed under **CC BY 4.0**.  
- See: [`LICENSE`](LICENSE)
