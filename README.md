# Agent Biotope

Agent Biotope is a design philosophy for cultivating autonomous AI work ecosystems.

The goal is not to command every agent. The goal is to shape a habitat where agents can produce useful work, reviewers can inspect it, watchdogs can constrain dangerous behavior, and humans only intervene at meaningful decision points.

## Core Image

A mature agent system should feel less like a command center and more like a stable biotope.

In a healthy biotope:

- activity continues without constant human instruction;
- boundaries prevent destructive spillover;
- circulation keeps work moving;
- decomposers clear stale or failed material;
- watchdogs detect abnormal conditions;
- humans intervene as gardeners, not micromanagers.

## Contrast

Some systems burn computation to preserve symbolic value.

Agent Biotope asks a different question:

> How can computation keep producing concrete, useful improvements while requiring less human intervention over time?

The target is not empty automation. The target is a productive habitat where useful work emerges, is reviewed, is constrained, and is surfaced to humans only at meaningful decision points.

## Repository Role

This repository holds the ideal theory, vocabulary, and design patterns.

Implementation-specific work belongs elsewhere.

For example:

- `agent-biotope`: why, principles, vocabulary, patterns.
- `task-deck`: one possible implementation surface for supervising and cultivating agent work ecosystems.

## Documents

- [Manifesto](docs/manifesto.md)
- [Principles](docs/principles.md)
- [Glossary](docs/glossary.md)
- [TaskDeck relationship](docs/notes/taskdeck-relationship.md)

Patterns:

- [Watchdog](docs/patterns/watchdog.md)
- [Capability Boundary](docs/patterns/capability-boundary.md)
- [Reviewer Gate](docs/patterns/reviewer-gate.md)
- [Decomposition Loop](docs/patterns/decomposition-loop.md)
- [Intervention Surface](docs/patterns/intervention-surface.md)

## Working Thesis

```text
Do not command every agent; shape the habitat.
Do not trust every agent; constrain capabilities.
Do not review everything manually; surface intervention points.
Do not preserve every output; decompose stale work.
Do not add infinite rules; build boundaries and flows.
```

## Status

Early concept repository. Language, structure, and patterns are expected to evolve.
