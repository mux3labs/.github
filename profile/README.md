# Mux3

Mux3 builds the infrastructure for multi-chain applications.

Modern Web3 development is fragmented. Every chain has its own SDK,
wallet logic, signing patterns, and network abstractions. Mux3 exists to
unify that experience without forcing developers into heavy frameworks.

We build modular, composable packages that allow applications to
interact with multiple blockchain ecosystems through a single runtime
interface.

## What is Mux3?

Mux3 is a multi-chain runtime built around a simple idea:

> One core. Many adapters.

At the center is:

- `@mux3/core` --- the chain-agnostic runtime layer.

Adapters extend it:

- `@mux3/evm` --- Ethereum & EVM chains\
- (more coming)

Each adapter implements a shared interface, allowing applications to
switch or combine chains without rewriting business logic.

## Design Principles

**Modular**\
Every chain lives in its own package. No cross-polluted dependencies.

**Composable**\
Adapters plug into the core runtime without modifying it.

**Framework-agnostic**\
Works in vanilla JavaScript or React. UI layers are optional.

**Minimal surface area**\
Small APIs. Predictable behavior. No magic.

**Extensible by design**\
New chains can be added without changing the core runtime.

## Ecosystem Structure

The Mux3 ecosystem is organized as a monorepo containing independent
packages:

- `@mux3/core` --- runtime and adapter registry\
- `@mux3/evm` --- EVM adapter\
- Future tooling (CLI, scaffolding, dev utilities)

Each package can be installed independently and versioned separately.

## Vision

The long-term goal is simple:

Make multi-chain development feel like developing against one system.

Not by hiding differences.\
Not by abstracting away everything.\
But by providing a consistent interface layer that developers control.

Mux3 does not attempt to replace chain SDKs.\
It standardizes how applications interact with them.

## Status

Mux3 is actively being built.

Core runtime and EVM adapter are under development.\
Additional adapters and CLI tooling are planned.

## Contributing

We welcome contributors who care about:

- Clean architecture\
- Strong type systems\
- Predictable APIs\
- Long-term ecosystem thinking

Open an issue or discussion to get involved.

## License

MIT
