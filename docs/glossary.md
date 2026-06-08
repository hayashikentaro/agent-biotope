# Glossary

## Agent Biotope

A designed habitat where AI agents can perform useful work with bounded autonomy.

An agent biotope includes roles, boundaries, flows, watchdogs, review gates, decomposition paths, and human intervention surfaces.

## Agent

An AI execution unit that can perform work inside the habitat.

Agents may be workers, reviewers, integrators, summarizers, decomposers, scouts, or other role-specific instances.

## Worker

An agent that produces changes or artifacts.

Workers should operate inside scoped workspaces, branches, tasks, or goals. They should not merge themselves unless explicitly assigned that authority.

## Reviewer

An agent that inspects worker output from a narrow responsibility perspective.

Reviewers should usually be read-only and should produce structured reports rather than fixes.

## Integrator

A role that combines worker outputs or reviewer reports into a coherent next step.

An integrator may decide merge order, summarize risks, or prepare a human-facing recommendation. Merge authority should be explicit, not assumed.

## Watchdog

A deterministic program that monitors the habitat for rule violations, abnormal loops, missing gates, invalid outputs, failed checks, or dangerous capability use.

A watchdog should not rely on semantic judgment when a deterministic check is possible.

## Habitat

The designed environment where agents operate.

A habitat includes filesystem boundaries, branches, tools, permissions, prompts, protocols, schemas, review policies, and UI surfaces.

## Boundary

A structural constraint that limits what an agent can do.

Examples:

- read-only reviewer sessions;
- allowed path lists;
- branch isolation;
- no merge rights for workers;
- output schema validation;
- sandbox or permission profiles.

## Capability Boundary

A boundary expressed as tool or action availability.

Instead of asking a reviewer not to edit files, remove write tools from the reviewer environment.

## Circulation

The flow that moves work through the habitat.

Example:

```text
goal -> worker -> review -> integration -> human decision -> merge / retry / reject
```

## Decomposer

A process or agent that handles stale, failed, abandoned, or obsolete work.

Decomposers prevent the habitat from filling with dead branches, outdated reports, and unprocessed failures.

## Intervention Point

A surfaced decision or action that genuinely needs human judgment.

Good intervention points are rare, specific, and decision-oriented.

## Gardener

The human role in a mature agent biotope.

A gardener does not micromanage every action. A gardener shapes the habitat, adjusts boundaries, prunes unhealthy growth, introduces new roles, and decides what counts as value.

## Law

The force of boundary, constraint, schema, gate, watchdog, naming, and structure.

Law gives a habitat shape. Without Life, Law becomes dead order.

## Life

The force of generation, exploration, circulation, accident, growth, and agent activity.

Life gives a habitat movement. Without Law, Life becomes uncontrolled growth.

## Love

The cultivating judgment that decides what is worth preserving, what should be pruned, and what value means.

Love prevents Law and Life from becoming cold automation. It is not indulgence; it is the care that accepts both growth and necessary cutting.

## Rulebook

Durable written criteria that let role sessions be recreated without depending on conversation memory.

Rulebooks may include principles, reviewer profiles, architecture doctrine, glossary entries, schemas, and gate policy.

## Gate

A required check before work can proceed to a later stage.

Gates may be deterministic, LLM-based, or human. Deterministic gates should be preferred whenever possible.

## Productive Autonomy

Autonomy that creates useful outcomes inside safe boundaries.

Autonomy without usefulness is noise. Autonomy without boundaries is risk.

## Health Signal

A measurement or observation that describes whether the habitat is working well.

Examples include safe merge throughput, unresolved intervention count, repeated failure loops, scope discipline, architectural coherence, and human micromanagement load.
