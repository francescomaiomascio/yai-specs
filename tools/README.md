# Tools Layout

This repository uses `tools/` as the only canonical home for executable tooling.

## Top-level layout

- `tools/bin`: user and CI entrypoints
- `tools/ops`: operational orchestration (gate/suite/verify)
- `tools/dev`: developer helpers
- `tools/release`: release and pinning utilities
- `tools/data`: dataset and data helpers
- `tools/bundle`: packaging/bundling helpers
- `tools/lib`: shared shell helpers

Tests are outside `tools/` under `tests/`.
