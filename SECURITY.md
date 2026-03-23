# Security Policy

## Supported Versions

| Version | Supported |
|---------|-----------|
| 0.1.x   | ✓ |

## Reporting a Vulnerability

**Do not open a public GitHub issue for security vulnerabilities.**

Report via [GitHub Security Advisories](https://github.com/bitchat-sdk/.github/security/advisories/new) on the affected repository. Please include the package name, version, a description of the vulnerability, steps to reproduce, and potential impact.

You will receive a response within 72 hours. Confirmed vulnerabilities will be patched promptly and credited in the release notes unless you prefer to remain anonymous.

## Scope

Security issues of particular interest:

- Incorrect cryptographic primitive usage
- Packet parsing bugs that could cause crashes or memory issues
- Information leakage in encoded output
- Incorrect NIP-17 gift-wrap implementation (deanonymization risk)
