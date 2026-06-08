# Pattern: Reviewer Gate

A Reviewer Gate is a narrow review role that must pass before work can proceed.

Reviewer gates are most useful when they are responsibility-specific instead of general-purpose.

## Problem

A single general reviewer tends to collapse many questions into one fuzzy judgment:

```text
Looks good overall.
Tests pass.
No major issues.
```

This can miss the exact failures that cause long-term drift:

- boundary creep;
- architecture erosion;
- product doctrine violations;
- weak verification;
- security-sensitive changes without review.

## Pattern

Use multiple narrow gates:

- Boundary Gate: did the change stay in scope?
- Architecture Gate: did the change preserve responsibility boundaries?
- UX/Product Gate: did the change preserve the product doctrine?
- Test/Regression Gate: is verification credible?
- Security Gate: did risk-sensitive behavior change safely?
- Integrator Gate: what should the human do next?

Each gate should have:

- a durable role profile;
- required inputs;
- explicit non-responsibilities;
- a fixed verdict vocabulary;
- concrete evidence requirements.

## Verdicts

A common vocabulary keeps reports comparable:

```text
PASS
PASS_WITH_NOTES
BLOCK
NEEDS_HUMAN
```

## Rule

Reviewers should report. They should not silently fix.

A reviewer that starts implementing becomes another worker and must move to a different capability profile.

## Why It Matters

Narrow reviewers are easier to refresh.

Their judgment can be reconstructed from a rulebook instead of preserved inside a long-lived conversation.
