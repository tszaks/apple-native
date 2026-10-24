# Contributing to apple-native

This repo is one catalog of Apple-native SwiftUI components, written for AI agents. The bar for changes: is the fact correct, does it say which OS it applies to, and does it keep the entry short?

By taking part you agree to follow the [Code of Conduct](CODE_OF_CONDUCT.md).

## Before you start

- **Wrong floor, broken recipe, dead link:** open an issue with the "Report an error" template, or send a pull request directly.
- **A missing component:** open an issue with the "Suggest a change" template. Say what it is, when to use it, and the minimum iOS version.
- Security problems go through [SECURITY.md](SECURITY.md), not a public issue.

## Entry format

Every entry in `CATALOG.md` answers three questions:

- **EXISTS:** what it is called and what it looks like.
- **USE WHEN:** the moment it is for, and where Apple's own apps use it.
- **BUILD:** the recipe, the minimum OS, a fallback for older systems, and the gotchas.

## Style

- Match the surrounding entries: same shape, same density.
- Short, specific sentences. No em dashes, no emoji, no marketing words.
- Every claim about availability names an iOS version. Verify it against Apple documentation or a WWDC session, or run it on a device or simulator.
- Code samples must compile. Keep them small.
- The catalog says "Compiled 2026-08". Do not change that line unless you re-verify the whole catalog.

## Pull request checklist

- [ ] The facts are correct and sourced (Apple documentation, WWDC, or tested).
- [ ] The OS floor and a fallback are stated.
- [ ] Code samples compile.
- [ ] Links work.
- [ ] The change is small and focused.
- [ ] A line added under `[Unreleased]` in [CHANGELOG.md](CHANGELOG.md).

## Using AI agents to contribute

Fine, as long as you read and understand what you submit and the checklist above is true. [AGENTS.md](AGENTS.md) tells coding agents how this repository works.

## License

By contributing you agree that your contribution is licensed under the [MIT License](LICENSE).
