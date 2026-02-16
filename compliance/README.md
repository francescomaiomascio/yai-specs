# Compliance

## What It Is

Machine-readable policy specifications and policy packs used for governance and retention.

Definitions:
- Policy spec: the schema and semantics (e.g., context, retention).
- Policy pack: concrete defaults and taxonomies for a jurisdiction or regime.

## Normative Artifacts

Policy specs:
- `compliance.context.v1.json`
- `retention.policy.v1.json`

Policy packs:
- `packs/gdpr-eu/2026Q1/pack.meta.json`
- `packs/gdpr-eu/2026Q1/retention.defaults.json`
- `packs/gdpr-eu/2026Q1/taxonomy.data_classes.json`
- `packs/gdpr-eu/2026Q1/taxonomy.legal_basis.json`
- `packs/gdpr-eu/2026Q1/taxonomy.purposes.json`

## Versioning Rules

- Policy specs use `vN` filenames (major version).
- Packs are versioned by path (e.g., `2026Q1`) and are immutable once published.
- Breaking changes require a new spec major or a new pack version.

## Consumers

- `yai-core`
- `yai-cli`
- `yai-yx`

## Change Procedure

- Update the policy spec or pack contents.
- Update `REGISTRY.md`, `SPEC_MAP.md`, and `CHANGELOG.md`.
- Add new pack versions instead of mutating existing ones.
