# Versioning

This repository follows Semantic Versioning for normative contracts.
Version changes apply to the repository tag and to any explicitly versioned files.

## Version Scheme

- `MAJOR`: incompatible normative change
- `MINOR`: backward-compatible additive normative change
- `PATCH`: non-normative edits (docs, clarifications) or compatible corrections

## What Is Breaking

A change is breaking when a compliant consumer can no longer interoperate without code changes.
Examples:
- removing required fields or commands
- changing required types or semantics
- altering header/ABI constants or envelope rules
- reusing IDs or changing ID meaning

## What Is Non-Breaking

- additive optional fields or commands
- additive policy packs that do not alter existing defaults
- documentation-only improvements

## Pinning and Tags

- Consumers MUST pin a specific repo revision or release tag.
- Pin updates must reference `CHANGELOG.md` and `COMPATIBILITY.md`.
- If a repo tag exists, it should follow `vMAJOR.MINOR.PATCH`.

## Compatibility Identifier

`SPECS_API_VERSION` is the logical compatibility identifier derived from this repo.
Consumers must validate compatibility against the active `SPECS_API_VERSION` before use.
