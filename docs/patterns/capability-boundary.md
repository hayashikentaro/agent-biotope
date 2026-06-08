# Pattern: Capability Boundary

A Capability Boundary is a structural limit on what an agent can do.

It is stronger than a rule written in a prompt because it does not depend on the agent remembering or obeying the rule.

## Problem

Prompt-only rules are fragile:

```text
Do not edit files.
Do not merge.
Do not run unsafe commands.
Stay inside this scope.
```

Agents may forget, reinterpret, or accidentally violate them.

## Pattern

Move important constraints into capabilities:

- give reviewers read-only access;
- remove write tools from reviewer sessions;
- prevent workers from pushing or merging;
- isolate workers in branches or worktrees;
- restrict accessible paths;
- expose only approved commands;
- validate output before accepting it;
- require explicit permission profiles for risky execution.

## Examples

```text
Worker:
  can read
  can edit assigned workspace
  can run verification
  cannot merge to main

Reviewer:
  can read diff
  can read docs
  can produce report
  cannot edit files
  cannot run merge commands

Integrator:
  can merge only after required gates pass
  can stop on conflict
  cannot ignore BLOCK verdicts without human override
```

## Design Rule

If a behavior is never allowed, remove the capability.

If a behavior is sometimes allowed, make the permission explicit, visible, and logged.

## Relationship To Trust

Capability boundaries do not mean agents are untrusted in a hostile sense.

They mean the habitat is designed so that agent mistakes do not become system damage.

## Why It Matters

A biotope becomes stable when desirable behavior is supported by the environment and dangerous behavior is constrained by structure.
