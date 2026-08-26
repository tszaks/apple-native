# apple-native

An LLM-optimized catalog of Apple-native SwiftUI design components: the drawers, collapsing bars, glass, scroll physics, symbol effects, haptics, and long-tail quirks that make an iOS app feel like Apple built it.

The problem it solves: these things exist, but you have to (1) know they exist, (2) know what they're for, and (3) know how to actually build them. Every entry in [`CATALOG.md`](CATALOG.md) answers exactly those three questions — **EXISTS / USE WHEN / BUILD** — with verified availability floors, fallbacks, and the gotchas that only show up in production.

## How to use it

Paste `CATALOG.md` into an AI coding session before building iOS UI. The agent can scan the USE WHEN lines against the screen it's building and discover the native component it didn't know to look for, instead of inventing something custom.

## What's inside

- **Parts 1–11:** the major components in full — navigation and chrome, sheets and detents, Liquid Glass, scroll behavior, lists and the five states, rolling numbers, motion, symbols and haptics, controls, gesture physics, the accessibility contract.
- **Part 12:** the long tail — 100+ verified lesser-known APIs in compact form, from `privacySensitive()` to `geometryGroup()` to `springLoadingBehavior`.
- **Part 13:** house patterns proven in production (Vero, Payday): the tucked drawer, undo toast, glass wrappers, the `.search`-role action tab, currency input, chart scrubbing, haptic tiers, and the reduce-motion idioms.
- Up front: the ten cross-cutting facts that save the most pain, and an availability ladder from iOS 13 to 26.

Compiled from Apple documentation, WWDC 23/24/25 sessions, and shipping code, August 2026. Companion to the [design thesis](https://github.com/tszaks/design-thesis): the thesis is what should feel native and why; this is the how.

Maintained by Tyler Szakacs.
