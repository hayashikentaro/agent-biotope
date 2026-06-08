# Pattern: Watchdog

A Watchdog is a deterministic monitor for an agent habitat.

It does not replace LLM reviewers. It prevents obvious unsafe or incoherent paths from continuing when a program can decide the condition more reliably than an LLM.

## Problem

Agents and reviewers can both make mistakes.

Adding another LLM supervisor does not eliminate uncertainty. It often creates another probabilistic layer that can also rationalize, overlook, or drift.

## Pattern

Use a deterministic program to monitor and enforce hard conditions:

- required reviewer missing;
- reviewer output schema invalid;
- worker touched files outside allowed scope;
- generated or runtime files changed;
- test command failed;
- merge attempted with blocking review;
- reviewer attempted write actions;
- branch/worktree does not match the assigned task;
- task loops or retries exceed threshold;
- change size exceeds configured limits;
- security-sensitive area changed without security gate.

## Rule

Let LLMs reason. Let programs constrain.

## Typical Actions

A watchdog may:

- block merge eligibility;
- mark a task as needing human intervention;
- stop or pause a session;
- request a missing reviewer;
- reject invalid reports;
- surface a concise alert.

## Non-Goals

A watchdog should not make fuzzy product judgments.

It should not decide whether an architecture is elegant, whether UX is aligned, or whether a tradeoff is acceptable unless that decision is encoded as a deterministic policy.

## Example

```text
if changed_files includes apps/server/src/server.js:
  require Architecture Reviewer

if changed_files includes permission or command construction code:
  require Security Reviewer

if any required reviewer verdict is BLOCK:
  merge_eligible = false

if reviewer_report is not valid schema:
  merge_eligible = false
```

## Why It Matters

A healthy biotope should not depend on every agent remembering every rule.

The habitat itself should make dangerous paths impossible, blocked, or visible.
