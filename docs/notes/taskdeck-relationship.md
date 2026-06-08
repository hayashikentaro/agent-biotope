# TaskDeck Relationship

Agent Biotope is the philosophy layer.

TaskDeck can be one implementation surface for that philosophy.

## Division Of Responsibility

```text
agent-biotope
  why
  principles
  vocabulary
  patterns
  ideal theory

task-deck
  how
  runtime
  UI
  PTY/session orchestration
  watchdog implementation
  review orchestration
  intervention surface
```

Keep ideal theory here when it is not yet ready to become implementation guidance.

Move concrete operational rules into TaskDeck when they become specific enough to guide agents, reviewers, watchdogs, or UI behavior.

## Mapping Concepts

| Agent Biotope concept | Possible TaskDeck expression |
| --- | --- |
| Habitat | local workspace, agent profiles, branches, task records, permissions |
| Worker | Codex/Goose/other agent session assigned a goal |
| Reviewer Gate | role-specific reviewer sessions and reports |
| Watchdog | deterministic program enforcing gates, schemas, permissions, and merge eligibility |
| Intervention Surface | `Needs you` / `Not now`, review summaries, merge/retry/reject decisions |
| Gardener | human operator supervising and shaping the ecosystem |
| Decomposer | stale task cleanup, failed branch summarization, retry/split/archive workflows |

## Important Boundary

TaskDeck should not become a repository of every ideal metaphor.

Agent Biotope should not become a backlog for TaskDeck implementation tasks.

Use this repository to develop language and patterns. Use TaskDeck to implement the parts that prove useful.

## Direction

A mature TaskDeck-like system would not simply show many terminals.

It would help cultivate an agent biotope:

- agents can work in parallel;
- reviewers can inspect narrow concerns;
- deterministic watchdogs constrain unsafe paths;
- decomposers prevent stale work buildup;
- humans see intervention points instead of raw chaos.
