# Principles

Agent Biotope uses ecological language as a design tool, not as decoration.

The core idea is simple: autonomous agents become more useful when they live inside a designed habitat with boundaries, circulation, decomposition, detection, and intervention points.

## 1. Shape The Habitat

Do not rely on better prompts alone.

Create an environment where useful behavior is the easiest path:

- clear task boundaries;
- isolated workspaces;
- role-specific capabilities;
- explicit handoff formats;
- durable rulebooks;
- visible intervention points.

## 2. Constrain Capabilities

LLMs will make mistakes. More LLM supervision does not remove that fact.

Use deterministic boundaries for deterministic constraints:

- read-only reviewers;
- no direct merge rights for workers;
- allowed path checks;
- output schema validation;
- required gates;
- sandbox and permission policies.

Let LLMs reason. Let programs constrain.

## 3. Prefer Flows Over Queues

A pile of agent outputs is not a biotope.

Healthy systems have circulation:

```text
goal
  -> worker
  -> review
  -> integration
  -> human decision
  -> merge / retry / reject / decompose
```

The system should move work forward or break it down, not merely accumulate it.

## 4. Make Decomposition First-Class

Stale work, failed branches, obsolete reports, and abandoned experiments should not rot forever.

A healthy agent habitat needs decomposers:

- close failed loops;
- archive dead branches;
- summarize abandoned work;
- extract reusable knowledge;
- turn failure into future constraints.

## 5. Surface Intervention Points

The human should not inspect everything.

The system should surface only meaningful intervention points:

- merge decision;
- risk acceptance;
- product direction choice;
- boundary violation;
- repeated failure;
- architectural drift;
- security-relevant change.

## 6. Keep Reviewers Narrow

Reviewer agents should not be general judges of everything.

They should be role instances with narrow responsibilities:

- boundary;
- architecture;
- UX/product doctrine;
- test/regression;
- security;
- integration summary.

Narrow reviewers are easier to refresh, compare, and constrain.

## 7. Treat Rulebooks As Source Of Truth

Do not depend on a long-lived reviewer session remembering the culture.

Put judgment criteria into durable files:

- principles;
- glossary;
- architecture doctrine;
- reviewer profiles;
- gate policy;
- output schema.

Sessions are disposable. Rulebooks persist.

## 8. Reduce Human Work By Increasing System Maturity

In a stable biotope, intervention decreases over time.

The goal is not zero human involvement. The goal is that human involvement moves upward:

```text
manual execution
  -> supervision
  -> boundary design
  -> ecosystem gardening
  -> value judgment
```

## 9. Measure Health, Not Activity

Agent activity is not the same as progress.

Better health signals include:

- useful completed work;
- low unresolved intervention count;
- low repeated-failure loops;
- review quality;
- scope discipline;
- architectural coherence;
- low human micromanagement;
- safe merge throughput.

## 10. Build Boundaries Instead Of Infinite Rules

Rules that depend on every agent remembering them are fragile.

Prefer structures that make bad paths impossible or visible:

- capabilities;
- schemas;
- branch policies;
- deterministic gates;
- watchdogs;
- isolated workspaces;
- role-specific tools.
