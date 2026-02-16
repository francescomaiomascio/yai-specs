# Contributing

## Scope

This repository is a specs-only contract source of truth.
Do not add runtime implementation guidance or operational playbooks here.

## Pull Request Rules

- Keep changes small and atomic.
- Use descriptive commits.
- Update `REGISTRY.md` when adding/removing normative artifacts.
- Update `CHANGELOG.md` for contract-facing changes.
- Update `SPEC_MAP.md` when adding/removing specs or packs.

## Normative Artifact Policy

Normative artifacts include JSON contracts, policy packs, and protocol/ABI headers.
Any normative change must:
- include explicit versioning intent (`MAJOR`, `MINOR`, or `PATCH` rationale)
- preserve compatibility guarantees or clearly declare breakage
- include corresponding vector/test updates when applicable

## Naming

Use canonical names only (no internal nicknames or marketing labels).
Prefer direct terms such as `registry`, `protocol`, `vector`, `policy`, `pack`.
