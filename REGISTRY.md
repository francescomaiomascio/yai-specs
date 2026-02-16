# Registry

This registry defines the canonical location of normative artifacts and the rules for allocating IDs.

## ID Registry

The authoritative ID registry lives in `protocol/yai_protocol_ids.h`.

Rules:
- IDs are never reused.
- Reserved ranges must remain reserved and documented in the header.
- New IDs require a corresponding spec change and a `CHANGELOG.md` entry.
- Any change that adds or reclassifies IDs must be reviewed for compatibility impact.

## Normative JSON Contracts

- `cli/commands.v1.json`
- `cli/commands.schema.json`
- `compliance/compliance.context.v1.json`
- `compliance/retention.policy.v1.json`
- `compliance/packs/gdpr-eu/2026Q1/pack.meta.json`
- `compliance/packs/gdpr-eu/2026Q1/retention.defaults.json`
- `compliance/packs/gdpr-eu/2026Q1/taxonomy.data_classes.json`
- `compliance/packs/gdpr-eu/2026Q1/taxonomy.legal_basis.json`
- `compliance/packs/gdpr-eu/2026Q1/taxonomy.purposes.json`
- `control/control_plane.v1.json`
- `control/authority.json`
- `engine/engine_cortex.v1.json`
- `graph/graph.v1.json`
- `providers/providers.v1.json`
- `vault/vault_abi.json`

## Normative C Headers

- `protocol/protocol.h`
- `protocol/transport.h`
- `protocol/yai_protocol_ids.h`
- `protocol/errors.h`
- `protocol/auth.h`
- `protocol/roles.h`
- `protocol/session.h`
- `protocol/audit.h`
- `protocol/runtime/rpc_runtime.h`
- `vault/yai_vault_abi.h`

## Conformance Vectors

Vectors are informative but should be updated when normative behavior changes.

- `vectors/transport_vectors.json`
- `vectors/auth_vectors.json`
- `vectors/audit_vectors.json`
