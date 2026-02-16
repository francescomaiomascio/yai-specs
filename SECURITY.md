# Security Policy

## Reporting

Report potential security issues privately to the maintainers through your designated private security channel.
Do not disclose exploit details publicly before coordinated remediation.

## Scope

Security issues in scope include:
- protocol parsing and validation weaknesses
- authorization/role gating bypasses in contract definitions
- ambiguity that can cause unsafe consumer behavior

## Threat Model Notes

Spec tampering is meaningless unless a consumer accepts an untrusted or unsigned bundle.
Consumers MUST pin and verify specs before use.

## Repository Hygiene

- Never commit secrets, tokens, credentials, or private keys.
- Keep examples and vectors synthetic and non-sensitive.
