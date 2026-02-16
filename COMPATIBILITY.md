# Compatibility

Compatibility is evaluated against `SPECS_API_VERSION`.
This matrix MUST be updated whenever a consumer release pins a new specs version.

## Compatibility Matrix

| SPECS_API_VERSION | yai-core | yai-cli | yai-yx | Notes |
| --- | --- | --- | --- | --- |
| v1 | UNSET | UNSET | UNSET | Populate on first pinned release |

## Rules

- Consumers MUST reject `MAJOR` mismatches.
- Minor/patch differences may be accepted only when backward compatibility is guaranteed by the normative contract.
