# Pattern: Decomposition Loop

A Decomposition Loop prevents failed, stale, or oversized work from accumulating as dead matter.

In a healthy biotope, abandoned output should either become useful knowledge or be cleared away.

## Problem

Agent habitats can accumulate clutter:

- failed branches;
- stale review reports;
- half-finished tasks;
- obsolete plans;
- repeated failed attempts;
- large work packages that never converge.

If this material is not decomposed, the habitat becomes harder to reason about and future agents inherit confusing residue.

## Pattern

When work fails or stalls, route it through decomposition:

```text
failed or stale work
  -> summarize what happened
  -> extract reusable facts
  -> identify blockers
  -> close, archive, retry, or split
  -> update rulebook or task design when needed
```

## Decomposer Responsibilities

A decomposer may:

- summarize the attempt;
- identify why it failed;
- preserve useful findings;
- recommend retry instructions;
- split a task into smaller goals;
- archive or close dead branches;
- suggest new watchdog checks or reviewer gates.

## Non-Goals

A decomposer should not keep every artifact alive forever.

The point is not memory hoarding. The point is nutrient recovery.

## Example Outcomes

```text
RETRY:
  The goal is still valid, but the worker changed too many files.
  Retry with explicit allowed paths.

SPLIT:
  The goal contains UI behavior and server persistence.
  Split into protocol, runtime, and UI tasks.

ARCHIVE:
  The branch implements an abandoned direction.
  Preserve the summary and close the branch.

RULEBOOK UPDATE:
  The same failure occurred three times.
  Add a deterministic watchdog check or reviewer rule.
```

## Why It Matters

A biotope is not healthy because nothing dies.

It is healthy because dead matter is transformed into future stability.
