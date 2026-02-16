# Versioning

This repository follows Semantic Versioning for contract evolution.

## Version Components

- `MAJOR`: incompatible normative changes
- `MINOR`: backward-compatible additive normative changes
- `PATCH`: non-normative fixes, clarifications, metadata, or typo-level corrections

## What Is Breaking

A change is breaking when an existing compliant consumer can no longer interoperate without code changes.
Examples include removing required fields, changing required types, changing envelope/header semantics, or deleting canonical commands/IDs.

## What Is Non-Breaking

Additive optional fields, additive commands gated by capability/version rules, and documentation-only improvements are non-breaking.

## SPECS_API_VERSION (Concept)

`SPECS_API_VERSION` is the logical compatibility identifier exposed by this repository.
Consumers should map their supported contracts to this version and validate compatibility before runtime operations.
