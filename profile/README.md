# bitchat-sdk

Cross-platform SDK packages for the [BitChat](https://github.com/permissionlesstech/bitchat) mesh networking protocol.

[![npm: protocol-core](https://img.shields.io/npm/v/@bitchat-sdk/protocol-core?label=npm%3A%20protocol-core)](https://www.npmjs.com/package/@bitchat-sdk/protocol-core)
[![npm: nostr](https://img.shields.io/npm/v/@bitchat-sdk/nostr?label=npm%3A%20nostr)](https://www.npmjs.com/package/@bitchat-sdk/nostr)
[![PyPI: bitchat-protocol](https://img.shields.io/pypi/v/bitchat-protocol?label=PyPI%3A%20bitchat-protocol)](https://pypi.org/project/bitchat-protocol/)
[![PyPI: bitchat-nostr](https://img.shields.io/pypi/v/bitchat-nostr?label=PyPI%3A%20bitchat-nostr)](https://pypi.org/project/bitchat-nostr/)
[![License: Unlicense](https://img.shields.io/badge/license-Unlicense-blue.svg)](https://unlicense.org)

BitChat is a decentralized, encrypted P2P chat network that runs over Bluetooth LE mesh and Nostr relays — no servers, no accounts, no infrastructure required. These packages let you build on top of that protocol in any environment.

## Packages

### Protocol Core — binary wire format, TLV codec, peer ID utilities

| Platform | Package | Install |
|----------|---------|---------|
| JavaScript / Node.js | [`@bitchat-sdk/protocol-core`](https://www.npmjs.com/package/@bitchat-sdk/protocol-core) | `npm install @bitchat-sdk/protocol-core` |
| Python | [`bitchat-protocol`](https://pypi.org/project/bitchat-protocol/) | `pip install bitchat-protocol` |
| Swift (iOS / macOS) | [`BitchatProtocol`](https://github.com/bitchat-sdk/BitchatProtocol) | SPM — see repo |
| Android (Kotlin) | [`io.github.bitchat-sdk:protocol-core`](https://github.com/bitchat-sdk/android-sdk) | Gradle — see repo |

### Nostr Transport — NIP-17 gift wrap, relay client, embedded packet helpers

| Platform | Package | Install |
|----------|---------|---------|
| JavaScript / Node.js | [`@bitchat-sdk/nostr`](https://www.npmjs.com/package/@bitchat-sdk/nostr) | `npm install @bitchat-sdk/nostr` |
| Python | [`bitchat-nostr`](https://pypi.org/project/bitchat-nostr/) | `pip install bitchat-nostr` |
| Swift (iOS / macOS) | [`BitchatNostr`](https://github.com/bitchat-sdk/BitchatNostr) | SPM — see repo |
| Android (Kotlin) | [`io.github.bitchat-sdk:nostr`](https://github.com/bitchat-sdk/android-sdk) | Gradle — see repo |

### Supporting

| Package | Description |
|---------|-------------|
| [`BitLogger`](https://github.com/bitchat-sdk/BitLogger) | Security-aware logging for Swift packages (iOS / macOS / Linux) |

## Wire Format Compatibility

All packages implement the same binary wire format. Packets encoded in JavaScript can be decoded in Python, Swift, or Kotlin. Cross-language compatibility is verified by a shared fixture suite.

## License

All packages are released under the [Unlicense](https://unlicense.org) — public domain, no restrictions.
