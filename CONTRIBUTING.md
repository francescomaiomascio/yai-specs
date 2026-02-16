# Contributing

## Scope

This repository is a contract repository. Treat normative artifacts as public API.

## Pull Request Rules

- Keep changes small and atomic.
- Use descriptive commits.
- Update `REGISTRY.md` when adding/removing normative artifacts.
- Update `CHANGELOG.md` for meaningful contract-facing changes.

## Normative Artifact Policy

Normative artifacts include `*.json` contracts and protocol/ABI headers.
Any normative change must:
- include explicit versioning intent (`MAJOR`, `MINOR`, or `PATCH` rationale)
- preserve compatibility guarantees or clearly declare breakage
- include corresponding vector/test updates when applicable

## Naming

Use canonical names only (no internal nicknames or marketing labels).
Prefer direct terms such as `runbook`, `registry`, `protocol`, `storage`, `vector`.
