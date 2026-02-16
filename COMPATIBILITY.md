# Compatibility

Compatibility is evaluated against `SPECS_API_VERSION`.

## Consumer Matrix (Conceptual)

- Core runtime must be compatible with the active `SPECS_API_VERSION`.
- CLI must be compatible with the active `SPECS_API_VERSION`.
- UI/Mind/YX integrations must target a compatible `SPECS_API_VERSION` through their runtime/CLI boundary.

## Hard Rule

Consumers must reject `MAJOR` mismatch.
Minor/patch differences may be accepted only when backward compatibility is guaranteed by the normative contract.
