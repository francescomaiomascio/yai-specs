# Tooling Layout Migration

## Scope

Repository: `yai-specs`
Target canonical layout: `tools/*` and `tests/*`

Baseline check on 2026-02-18:

- `scripts` directories found: `0`
- `scripts` path references found: `0`

## Mapping Table

| OLD_PATH | NEW_PATH | CLASS | NOTES |
|---|---|---|---|
| `(none found under scripts)` | `(no-op)` | entrypoint | No legacy entrypoint in this repository. |
| `(none found under scripts)` | `(no-op)` | ops | No legacy gate/suite/verify scripts in this repository. |
| `(none found under scripts)` | `(no-op)` | dev | No legacy dev helpers in this repository. |
| `(none found under scripts)` | `(no-op)` | release | `tools/release/bump_version.sh` already canonical. |
| `(none found under scripts)` | `(no-op)` | data | No data tooling migration required from legacy scripts. |
| `(none found under scripts)` | `(no-op)` | test | No legacy script-based tests found. |

## Verification

Verification date: 2026-02-18

- Legacy directory check: PASS (`scripts` directory absent)
- Legacy path reference grep (`scripts` slash pattern): PASS (0 matches)
- Build sanity (`make clean && make`): PASS
- Tools tree sanity: PASS (`tools/` contains canonical folders)
- Entrypoint help checks under `tools/bin`: NOT APPLICABLE in `yai-specs`
  - `tools/bin/yai-verify --help`: file not present
  - `tools/bin/yai-suite --help`: file not present
  - `tools/bin/yai-gate --help`: file not present
  - `tools/bin/yai-doctor --help`: file not present
  - `tools/bin/yai-purge --help`: file not present

Notes:

- `yai-specs` is a specification repository and does not currently ship the `yai-*` operational binaries.
