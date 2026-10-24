<h1 align="center">apple-native</h1>

<p align="center">
  An LLM-optimized catalog of Apple-native SwiftUI components, for iOS 13 to 26.
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/github/license/tszaks/apple-native" alt="MIT license"></a>
  <img src="https://img.shields.io/badge/iOS-13%E2%80%9326-blue" alt="Covers iOS 13 to 26">
  <img src="https://img.shields.io/badge/SwiftUI-catalog-orange" alt="SwiftUI catalog">
</p>

Each entry in [`CATALOG.md`](CATALOG.md) has the same three parts, so an agent can scan it fast:

```
### Large title collapse
EXISTS: The signature iOS settle: big left-aligned bold title living in the content, compressing into a small centered bar title on scroll.
USE WHEN: Every root screen of a section. Apple: Settings, Mail, Music, Health. Detail screens go `.inline`.
BUILD: a Swift snippet, the minimum OS, a fallback, and the gotchas.
```

This catalog covers the drawers, collapsing bars, glass, scroll physics, symbol effects, haptics, and long-tail quirks that make an iOS app feel like Apple built it.

The problem it solves: these things exist, but you have to (1) know they exist, (2) know what they are for, and (3) know how to build them. Every entry answers exactly those three questions (**EXISTS / USE WHEN / BUILD**) with verified availability floors, fallbacks, and the gotchas that only show up in production.

## Features

- **Parts 1 to 11:** the major components in full. Navigation and chrome, sheets and detents, Liquid Glass, scroll behavior, lists and the five states, rolling numbers, motion, symbols and haptics, controls, gesture physics, the accessibility contract.
- **Part 12:** the long tail. 100+ verified lesser-known APIs in compact form, from `privacySensitive()` to `geometryGroup()` to `springLoadingBehavior`.
- **Part 13:** house patterns proven in production (Vero, Payday). The tucked drawer, undo toast, glass wrappers, the `.search`-role action tab, currency input, chart scrubbing, haptic tiers, and the reduce-motion idioms.
- **Up front:** the ten cross-cutting facts that save the most pain, and an availability ladder from iOS 13 to 26.

## Quick start

Nothing to install. It is one Markdown file.

```sh
git clone https://github.com/tszaks/apple-native.git
open apple-native/CATALOG.md
```

Or read it on GitHub: [`CATALOG.md`](CATALOG.md).

## Using with agents

Paste `CATALOG.md` into an AI coding session before building iOS UI, or point the agent at the file. The agent can scan the USE WHEN lines against the screen it is building and discover the native component it did not know to look for, instead of inventing something custom.

A prompt that works:

```
Read CATALOG.md. Before you build any custom UI for this screen, find the
entry whose USE WHEN matches, use its BUILD recipe, and respect its OS floor.
```

For the rules on how the finished screen should look and behave, pair it with the [design thesis](https://github.com/tszaks/design-thesis): the thesis is what should feel native and why, and this catalog is the how.

Compiled from Apple documentation, WWDC 23/24/25 sessions, and shipping code, August 2026.

## Contributing

Corrections are welcome: a wrong availability floor, a broken recipe, a dead link. Please read [CONTRIBUTING.md](CONTRIBUTING.md) first. Security problems go through [SECURITY.md](SECURITY.md). Everyone taking part follows the [Code of Conduct](CODE_OF_CONDUCT.md).

Docs: [catalog](CATALOG.md) · [changelog](CHANGELOG.md)

## License

[MIT](LICENSE) © 2026 Tyler Szakacs
