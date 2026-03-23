# Contributing to bitchat-sdk

Thank you for your interest in contributing. These packages implement the BitChat binary protocol and Nostr transport layer. Contributions that preserve wire-format compatibility are always welcome.

## Ground Rules

- **Do not change the wire format.** The binary packet structure, TLV encoding, and crypto semantics must remain identical across all language implementations. Any change that breaks cross-language compatibility will not be merged.
- **Test against the spec fixtures.** The `spec-tests/` fixture suite is the source of truth for encoding correctness. New codec behavior must be covered by fixtures.
- **One concern per PR.** Bug fixes, new features, and refactors should be separate pull requests.

## How to Contribute

### Reporting bugs
Open an issue using the **Bug report** template. Include the package name, version, language, and a minimal reproduction.

### Proposing features
Open an issue using the **Feature request** template before writing code. For anything that touches the wire format, open a discussion first — protocol changes require coordination across all language implementations.

### Submitting a pull request
1. Fork the repository and create a branch from `main`.
2. Make your changes and ensure all existing tests pass.
3. Add tests for any new behavior.
4. Fill out the pull request template fully.
5. Open the PR against `main`.

## Development Setup

Each package has its own toolchain. See the individual repository README for build and test instructions.

| Package | Test command |
|---------|-------------|
| JS packages | `npm test` |
| Python packages | `pytest` |
| Swift packages | `swift test` |
| Android SDK | `./gradlew test` |

## Code Style

Follow the conventions already present in each package. Do not reformat code unrelated to your change.

## License

By contributing, you agree that your contributions will be released into the public domain under the [Unlicense](https://unlicense.org).
