# Pattern: Intervention Surface

An Intervention Surface is the part of an agent habitat that shows humans only the decisions that need human judgment.

It is not a log viewer for everything agents do.

## Problem

Agent systems can create too much output:

- terminal logs;
- diffs;
- test results;
- review reports;
- branch status;
- repeated questions;
- partial plans.

If all of this is shown equally, the human becomes the bottleneck again.

## Pattern

Design a surface that compresses the habitat into decision points:

- needs human input;
- ready to merge;
- blocked by gate;
- repeated failure;
- scope violation;
- security risk;
- product tradeoff;
- stale work needs decomposition.

## Good Intervention Points

A good intervention point is:

- specific;
- actionable;
- grounded in evidence;
- tied to a decision;
- small enough for a human to resolve;
- rare enough to preserve attention.

## Bad Intervention Points

Avoid surfacing everything as equally urgent:

- raw logs without summary;
- every agent status update;
- low-confidence internal state;
- generic warnings;
- unprioritized review notes;
- endless queues of maybe-interesting details.

## Example

Instead of:

```text
Agent A produced output.
Agent B produced output.
Reviewer C produced output.
Tests ran.
Diff changed.
```

Show:

```text
Needs you:
  PR #42 is blocked by Architecture Reviewer.
  Reason: UI reimplemented server-side attention inference.
  Recommended action: retry with server-owned source of truth.
```

## Why It Matters

The human should not be the scheduler, parser, and debugger for the whole habitat.

The human should be the gardener who sees where intervention changes the system.
