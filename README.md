# YAI Specs

`yai-specs` is the canonical contract repository for YAI.
It defines the shared protocol and data contracts consumed by runtime components.
The repository is designed to be pinned and consumed across multiple codebases.
It is intentionally stable, explicit, and versioned.
It is the source of truth for cross-repo compatibility.

## Normative vs Informative

Normative artifacts:
- JSON contracts (`*.json`)
- C headers that define protocol/ABI (`protocol/*.h`, `vault/yai_vault_abi.h`)

Informative artifacts:
- Markdown documentation (`*.md`), runbooks, and explanatory notes

If there is a conflict, normative artifacts take precedence.

## Consumption Model

Consumers should use this repository as a pinned dependency (submodule or snapshot).
Pinning must be explicit and tied to a known specs revision.
Upgrades should be deliberate and validated against compatibility rules.

## Repository Sections

- `protocol/` - transport envelope, IDs, auth, errors, runtime protocol headers
- `vault/` - vault ABI contract and header
- `control/` - control plane schema and authority model
- `cli/` - CLI command contracts and schema
- `engine/` - engine contract surface
- `graph/` - graph contract schema
- `providers/` - provider-facing contract schema
- `compliance/` - compliance context and retention policy contracts
- `vectors/` - conformance and protocol test vectors

## Indexes

- `REGISTRY.md` - canonical registry of normative artifacts
- `VERSIONING.md` - semantic versioning and breakage policy
- `COMPATIBILITY.md` - consumer compatibility rules
- `CHANGELOG.md` - documented contract changes
