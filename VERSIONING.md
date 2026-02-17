# Versioning

This repository follows Semantic Versioning for repository releases.
Version changes apply to repository tags and to explicitly versioned normative artifacts.

Public release baseline: `v0.1.0` (2026-02-17).

## Version Scheme (Repository Tags)

- `MAJOR`: incompatible normative contract change
- `MINOR`: backward-compatible additive normative change
- `PATCH`: documentation, clarifications, compatible corrections

## Compatibility Identifier

`SPECS_API_VERSION` is the protocol/contract compatibility line.
Current value: `v1`.

Important:
- Repository release version (`v0.1.0`, `v0.1.1`, ...) and `SPECS_API_VERSION` are related but not identical.
- The repo can be `0.x` while the active contract compatibility line is `v1`.

## What Is Breaking

A change is breaking when a compliant consumer can no longer interoperate without code changes.
Examples:
- removing required fields or commands
- changing required types or semantics
- altering ABI/protocol constants or envelope rules
- reusing IDs or changing ID meaning

## Pinning and Releases

- Consumers MUST pin a specific repo revision or release tag.
- Pin updates MUST reference `CHANGELOG.md` and `COMPATIBILITY.md`.
- Tags SHOULD follow `vMAJOR.MINOR.PATCH`.
