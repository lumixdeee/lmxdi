# Testing non-mapping meshing primitives: A double naked baseline approach

## Working paper v0.001

### Abstract

Some meshing primitives expose their effect quickly through semantic mapping and search. Others are not expected to operate through that surface. This paper proposes a comparative method for testing the latter class: run the system under test (SUT) with the primitive alongside two independent naked runs using the same task and inputs.

The second naked run provides an immediate indication of ordinary model variation. If the two naked outputs differ as much as the SUT differs from either control, a simple A/B interpretation is weak. If the naked outputs remain relatively close while the SUT repeatedly departs from them in a relevant direction, a prompt effect becomes a stronger candidate for further testing.

The method is intended for primitives such as 12 Dwarven Sins and PREMISE, where semantic-map performance is not the expected test surface.

## 1. Objective

Test whether a non-mapping meshing primitive produces an observable and repeatable difference from an unmodified model while distinguishing that difference from ordinary run-to-run variation.

Discovery and specification may be the work being performed. They are not themselves the experimental outcome. The test concerns differences in model performance within that work.

## 2. Scope

Current candidates are 12 Dwarven Sins and PREMISE.

DRAGI, 12 Actors and Alphablest differ because semantic mapping and search already provide a rapid observable test surface. 12 Dancers should be usable through mapping/search too, but that route has not yet been tried.

## 3. Experimental layout

For each trial:

```text
SUT:      model + primitive
Naked A:  model without primitive
Naked B:  model without primitive

same task
same supplied inputs
same relevant runtime conditions
independent runs
```

Where practical, output identity can remain hidden from the scorer.

The two naked runs provide both a baseline and a small sample of baseline variation.

## 4. Why double naked?

A single naked comparison does not distinguish a prompt effect from ordinary stochastic variation very well.

With only one control:

```text
distance(SUT, Naked A) = large
```

may look impressive even when another unmodified run would differ just as much.

Adding Naked B exposes this problem:

```text
distance(Naked A, Naked B) = baseline spread
```

The useful question is then whether the SUT departure exceeds, and meaningfully differs from, the variation already visible between naked runs.

Two controls do not establish the full baseline distribution. This is a screening method, not a full variance estimate.

## 5. Interpretation

### Large naked variation

If Naked A and Naked B already diverge strongly, and the SUT falls within comparable variation, status is HOLD. Repeat with more runs, a tighter task, or a better scoring rule.

### Nakeds cluster, SUT differs

If Naked A and Naked B are relatively similar while the SUT departs in a relevant direction, status is CANDIDATE EFFECT. Repetition across independent trials strengthens the observation.

### All three cluster

Status is NO DETECTABLE EFFECT for this task and these conditions. This does not establish that the primitive is inert elsewhere.

### SUT is worse

A repeatable negative departure is also informative. The primitive may impose a cost, distort the task, or help only under narrower conditions.

## 6. What to score

Scoring dimensions should come from the primitive's intended role and the task, rather than from semantic-map testing.

Candidate observables include distinctions noticed, relevant objects retained, relations preserved, omissions, substitutions, unsupported additions, contradictions, task-specific errors, and useful findings absent from controls.

The rubric should be fixed before identities are revealed wherever feasible.

A difference is not automatically an improvement. Direction and relevance must be scored separately.

## 7. Discovery and specification

For 12 Dwarven Sins and PREMISE, the practical task may be to use the primitive while discovering its behaviour and writing its specification.

That development activity must remain separate from the test criterion.

The experiment asks:

```text
Given the same underlying work,
does the SUT behave differently from naked controls
in a relevant and repeatable way?
```

The observations can then inform the specification.

## 8. Minimum trial record

```text
primitive/version
model/runtime
task
input
SUT output
Naked A output
Naked B output
scoring rubric
scores/observations
naked-to-naked spread
SUT-to-control difference
status
```

Suggested statuses:

```text
HOLD
CANDIDATE EFFECT
NO DETECTABLE EFFECT
CANDIDATE NEGATIVE EFFECT
RETEST
```

## 9. Limits

The double naked method is a screening design, not a complete causal experiment.

Two naked runs cannot establish the full output distribution. Model updates, hidden runtime variation, conversation state, sampling behaviour and scoring subjectivity can still confound results.

```text
one SUT difference != prompt effect
naked disagreement != test failure
naked agreement + SUT departure != proof
repeatable scored departure > isolated impressive example
```

Where baseline variation is large, additional naked and SUT replicates are more useful than stronger interpretation of the first trial.

## 10. Proposed first test

Run one task relevant to 12 Dwarven Sins or PREMISE as three independent instances:

```text
1 x SUT + primitive
2 x naked
```

Do not use semantic-map production as the criterion.

First inspect Naked A versus Naked B. Only then interpret the SUT difference.

If naked variation is already too large for the proposed scoring dimensions, revise the task or rubric before treating SUT differences as evidence.

## 11. Current status

This paper specifies a proposed test method. It does not report completed double-naked trials for 12 Dwarven Sins or PREMISE.

The immediate empirical question is whether a primitive-conditioned SUT departs from two naked controls by more than the baseline variation visible between those controls, and whether that departure repeats in the direction relevant to the primitive's intended role.
