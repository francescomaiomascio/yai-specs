# Compatibility

Compatibility is evaluated against `SPECS_API_VERSION`.
Current compatibility identifier: `v1`.

## Compatibility Matrix

| SPECS_API_VERSION | yai | yai-cli | yai-yx | Notes |
| --- | --- | --- | --- | --- |
| v1 | v0.1.x | v0.1.x | UNSET | Initial public baseline line |

## Rules

- Consumers MUST reject `MAJOR` compatibility mismatches.
- Minor/patch differences may be accepted only when backward compatibility is preserved.
- Every consumer release MUST record the pinned `yai-specs` commit or tag used for verification.
