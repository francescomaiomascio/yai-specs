# Spec Map

Mappa canonica delle specs e del loro stato nel repository `yai-specs`.

## Protocol

- Version: `v1` (where tagged)
- Status: stable
- Links:
  - `protocol/protocol.h`
  - `protocol/transport.h`
  - `protocol/yai_protocol_ids.h`
  - `protocol/errors.h`
  - `protocol/auth.h`
  - `protocol/roles.h`
  - `protocol/session.h`
  - `protocol/audit.h`
  - `protocol/runtime/rpc_runtime.h`

## Control

- Version: `v1` (`control_plane`)
- Status: stable
- Links:
  - `control/control_plane.v1.json`
  - `control/authority.json`

## CLI

- Version: `v1` (`commands`)
- Status: stable
- Links:
  - `cli/commands.v1.json`
  - `cli/commands.schema.json`

## Vault

- Version: ABI current (`v1` schema)
- Status: stable
- Links:
  - `vault/vault_abi.json`
  - `vault/yai_vault_abi.h`

## Graph

- Version: `v1`
- Status: stable
- Links:
  - `graph/graph.v1.json`

## Providers

- Version: `v1`
- Status: stable
- Links:
  - `providers/providers.v1.json`

## Compliance

- Version: `v1` (context/policy)
- Status: draft
- Links:
  - `compliance/compliance.context.v1.json`
  - `compliance/retention.policy.v1.json`

## Engine

- Version: `v1` (`engine_cortex`)
- Status: experimental
- Links:
  - `engine/engine_cortex.v1.json`

## Vectors

- Version: snapshot set
- Status: draft
- Links:
  - `vectors/transport_vectors.json`
  - `vectors/auth_vectors.json`
  - `vectors/audit_vectors.json`
