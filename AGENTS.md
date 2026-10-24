# apple-native

Documentation only: `CATALOG.md`, an LLM-optimized catalog of Apple-native SwiftUI components (EXISTS / USE WHEN / BUILD, iOS 13 to 26). There is no code, build or test suite.

This file is for AI agents that **edit** this repo. If you are an agent that **uses** the catalog while building iOS UI, read [CATALOG.md](CATALOG.md) directly and scan the USE WHEN lines against the screen you are building.

## Files
- `CATALOG.md`: the catalog. Cross-cutting facts, an availability ladder, then Parts 1 to 13.
- `README.md`: the overview.
- `CONTRIBUTING.md`, `SECURITY.md`, `CODE_OF_CONDUCT.md`, `CHANGELOG.md`, `.github/`: repo housekeeping.

## Conventions
- Keep every entry in the EXISTS / USE WHEN / BUILD shape.
- Every availability claim names an iOS version. Do not guess a floor: verify it against Apple documentation or a WWDC session.
- Code samples must compile. Keep them small.
- Short, specific sentences. No em dashes, no emoji, no marketing words.
- Add a line under `[Unreleased]` in `CHANGELOG.md` for any change a reader would notice.

## Related repo
The same catalog also ships as `APPLE_NATIVE.md` in [design-thesis](https://github.com/tszaks/design-thesis), alongside the thesis it supports. That copy has one more cross-cutting fact (11, backwards compatibility) that this one lacks, so check both before you edit.

## Do not
- Do not add secrets, personal data or client names.
