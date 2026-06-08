# Compute Flow Model

Agent Biotope differs from natural ecosystems in one decisive way: compute does not circulate like nutrients.

In natural ecosystems, sunlight enters from outside, plants fix it into living matter, and valuable material circulates through many forms. In an agent habitat, compute is consumed as a time-indexed flow from fixed hardware, energy, budget, model access, and human allocation.

Compute itself does not return.

What can return is structure.

## Core Thesis

```text
Compute dissipates.
Structure accumulates.
```

Or more precisely:

```text
Compute is not a circulating nutrient.
Compute is a time-indexed dissipative flow.

What circulates is not compute itself,
but knowledge, constraints, selection pressure, and durable structure.
```

## Natural Ecosystem vs Agent Biotope

```text
Natural ecosystem
  sunlight
    -> plant fixation
    -> biomass
    -> animals, microbes, soil
    -> decomposition
    -> nutrient circulation
    -> future growth
```

```text
Agent Biotope
  compute flow
    -> exploration
    -> candidates, reports, residue
    -> selection and decomposition
    -> fixation
    -> knowledge, constraints, tests, rulebooks, selection pressure
    -> better future exploration
```

The agent habitat cannot recycle the spent compute. It can only make future compute more selective.

## Compute As A Time-Indexed Flow

Available compute is closer to a flow than a stock that returns.

```text
available_compute ~= hardware_capacity x time x budget x model_access
```

This creates allocation questions:

- which agents receive expensive model time;
- which checks should be deterministic programs;
- which tasks deserve continued exploration;
- which candidates should be cut early;
- which failures should receive decomposition but no further exploration;
- when to stop spending compute on a direction.

## What Returns

The habitat can return value to itself through durable structure:

- better tests;
- clearer prompts;
- stronger reviewer profiles;
- watchdog rules;
- schemas;
- architecture doctrine;
- glossary entries;
- task decomposition patterns;
- examples of good output;
- explicit product taste;
- known failure patterns;
- cleaner context.

These do not recycle compute. They improve future compute use.

## Structural Return On Compute

A mature habitat should increase structural return per unit of compute.

Bad signs:

- many tokens used, little durable structure;
- many branches generated, few selected forms;
- repeated failures without new constraints;
- large logs but no compressed knowledge;
- high human review load after agent work;
- expensive reviewers used for deterministic checks.

Good signs:

- future tasks need less clarification;
- repeated failures decrease;
- reviewer outputs become more schema-valid;
- watchdogs catch issues earlier;
- tests encode past mistakes;
- prompts become shorter because rulebooks carry context;
- humans make fewer low-level decisions;
- accepted artifacts per unit of compute improves.

## Selection Under Finite Compute

Because compute does not return, selective cultivation matters.

Do not spend compute equally on every candidate.

Use early selection pressure:

- deterministic watchdogs reject impossible or unsafe paths;
- cheap checks filter obvious failures;
- small models patrol low-judgment tasks;
- strong models focus on architecture, product judgment, security, and integration;
- human attention is reserved for value decisions.

## Relationship To Harvest

Harvest is not measured by how much compute was consumed.

A good harvest may use less compute because the habitat has accumulated structure that guides exploration.

The return loop should ask:

```text
What did this compute leave behind that improves the next cycle?
```

If the answer is only logs, unselected diffs, and human attention debt, the compute was dissipated without sufficient structural return.

## Design Rule

```text
Do not try to recycle compute.
Recycle the structure produced by compute.
```

A mature Agent Biotope does not become valuable because it runs more agents. It becomes valuable because each unit of compute becomes more likely to produce selected, shaped, durable value.
