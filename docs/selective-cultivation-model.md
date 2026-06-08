# Selective Cultivation Model

Agent Biotope is not industrial agriculture.

It does not harvest output volume. It is closer to selective cultivation: koi breeding, goldfish selection, or bonsai cultivation.

The habitat generates variation. Selection pressure removes weak or misaligned forms. The gardener prunes and shapes promising growth. The final harvest is durable quality, not quantity.

## Why Agriculture Is Not Enough

Agriculture often suggests a quantity model:

```text
input
  -> growth
  -> more output
  -> harvest
```

This is useful for thinking about nutrients, substrate, and return loops, but it can mislead agent system design.

Agent Biotope should not optimize for:

- more code;
- more pull requests;
- more documents;
- more review comments;
- more agent activity;
- more accumulated artifacts.

Volume can become pollution when selection and decomposition are weak.

## Core Cycle

```text
context + compute + agents
  -> variation
  -> selection
  -> pruning
  -> shaping
  -> fixation
```

The value is not in producing many candidates. The value is in selecting, shaping, and fixing the rare forms worth preserving.

## Koi And Goldfish Selection

Selective breeding begins with many individuals, but value appears through selection.

```text
many young fish
  -> early selection
  -> growth observation
  -> color, form, vitality, and future potential
  -> further selection
  -> a small number of valuable individuals remain
```

Agent work behaves similarly:

```text
many candidate implementations
  -> tests and watchdogs reject obvious failures
  -> reviewers reject misaligned forms
  -> architecture and product doctrine select for coherence
  -> human taste selects what is worth preserving
  -> a small number of durable artifacts remain
```

A worker output is not automatically harvest. It is a candidate individual.

## Bonsai Cultivation

Bonsai adds another important element: shaping.

The gardener does not create every branch. The tree grows. The gardener intervenes through timing, pruning, wiring, pot choice, root work, water, light, and restraint.

Agent Biotope works the same way:

- agents generate growth;
- the gardener chooses which direction to preserve;
- large diffs are pruned;
- goals are split;
- boundaries are tightened;
- promising branches are shaped through follow-up instructions;
- some growth is left alone until it reveals its form.

The final value is not raw growth. It is shaped form.

## Roles In This Model

```text
Worker
  Variation generator.
  Produces candidate forms through exploration, mutation, and trial.

Reviewer
  Selection membrane.
  Decides whether a candidate can move to the next stage from a narrow responsibility perspective.

Watchdog
  Hard constraint.
  Eliminates candidates that violate deterministic boundaries.

Decomposer
  Nutrient recovery.
  Converts rejected, failed, or pruned work into future constraints, tests, prompts, or rulebook improvements.

Human / Gardener
  Taste and direction.
  Decides what is beautiful, useful, coherent, promising, and worth preserving.
```

## Law, Life, Love

Selective cultivation makes the Three Ls concrete.

```text
Life
  Candidates emerge. Branches grow. Variation appears. Unexpected forms become possible.

Law
  Tests, schemas, watchdogs, reviewer gates, architecture rules, and product doctrine constrain growth.

Love
  The gardener decides what to keep, what to prune, and what future form is worth cultivating.
```

Without Life, there is no variation.

Without Law, variation becomes uncontrolled growth.

Without Love, selection becomes cold scoring without taste or purpose.

## Harvest Reframed

Harvest is not the extraction of all outputs.

Harvest is the fixation of selected quality into durable form.

Examples:

```text
many implementation attempts
  -> one good commit

many UI proposals
  -> one product decision

failed branch
  -> one watchdog rule

ambiguous request
  -> three clear issues

long discussion
  -> one durable principle
```

A good harvest may reduce volume. It often compresses many possibilities into one useful form.

## Pruning Is Not Failure

Rejecting, retrying, archiving, and decomposing are not failures of the habitat.

They are selection and pruning operations.

A healthy habitat must be able to:

- reject weak candidates;
- cut oversized diffs;
- archive abandoned directions;
- decompose failed work;
- preserve useful lessons;
- retry with sharper constraints;
- prevent every generated artifact from surviving.

A system that keeps everything becomes incoherent.

## Design Rule

```text
Do not measure agent biotope health by output volume.
Measure it by the quality of selected, shaped, durable forms.
```

The goal is not to make agents produce more.

The goal is to create a habitat where valuable forms can emerge, be selected, be shaped, and be preserved.
