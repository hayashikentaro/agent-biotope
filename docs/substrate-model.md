# Substrate Model

Visible agent work depends on invisible substrate health.

In a real biotope, fish die quickly if the soil, filter media, and microbial ecosystem are not stable. The visible organisms depend on invisible metabolism.

Agent Biotope uses the same principle: do not scale visible agents faster than the habitat can metabolize their waste.

## Core Rule

```text
Do not scale fish faster than the substrate can metabolize waste.
```

For agent systems:

```text
Do not increase agent parallelism before the habitat can decompose failed work, stale branches, noisy logs, invalid reports, and scope drift.
```

## Ecological Mapping

```text
Fish
  Worker agents, reviewer agents, integrator agents.
  Visible productive activity.

Water
  Task flow, logs, diffs, reports, state updates, and review circulation.
  The operational medium agents live in.

Plants
  Docs, tests, examples, prompts, issue structure, and architecture notes.
  They absorb excess nutrients, stabilize the environment, and provide structure.

Soil / Filter Media
  Repository structure, branch/worktree isolation, permissions, schemas, protocols, and durable rulebooks.
  The substrate where invisible stabilizers can live.

Microbes
  Watchdog checks, linters, type checks, test suites, schema validators, stale cleanup, decomposers, and small patrol models.
  They process waste and keep the water livable.
```

## Waste

Agent habitats produce waste as a normal part of activity.

Examples:

- failed attempts;
- stale branches;
- oversized diffs;
- unmerged partial work;
- noisy logs;
- invalid review reports;
- duplicated concepts;
- weak tests;
- ambiguous prompts;
- scope drift;
- stale TODOs;
- reviewer disagreement without resolution;
- human attention debt.

Waste is not automatically bad. Waste becomes toxic when the habitat cannot process it.

## Microbial Layer

The microbial layer should be boring, mostly deterministic, and mostly invisible.

Examples:

- `git diff --check`;
- build, test, lint, and type checks;
- output schema validation;
- allowed path checks;
- generated/runtime file checks;
- required reviewer resolution;
- stale task detection;
- stale branch cleanup;
- failed attempt summarization;
- duplicate concept detection;
- watchdog rules;
- decomposer loops.

The gardener does not need to see every microbe. The gardener needs to know whether the substrate is healthy.

## Health Signals

Useful substrate health signals include:

- stale work count;
- repeated failure loops;
- branch age and abandoned branch count;
- review report validity rate;
- required gate completion rate;
- test stability;
- drift or duplicate concept detection;
- human intervention backlog;
- watchdog alert frequency;
- ratio of harvested outputs to decomposed residue.

## Scaling Rule

Do not increase one trophic layer alone.

Increasing worker agents without increasing review, decomposition, watchdog, and rulebook capacity is like adding fish to an immature tank. The system may look productive briefly, then the water degrades.

Scale in layers:

```text
more workers
  -> more reviewer capacity
  -> stronger watchdogs
  -> better decomposition
  -> richer rulebooks
  -> stronger substrate
```

## Design Implication

Before building more visible agent activity, build the invisible substrate:

- clear repository structure;
- isolated workspaces;
- role-specific capabilities;
- review report schemas;
- deterministic watchdog checks;
- decomposer workflows;
- tests and examples;
- durable rulebooks.

A healthy substrate lets the gardener intervene less, not because nothing happens, but because invisible processes keep the habitat livable.
