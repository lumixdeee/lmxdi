# Ah Quick Start

**Ah is a Think Tank Object Armour GPT for long-context research.**  
It combines archive loading, fast source-near retrieval, object custody, H0 null hypothesis baselines, and anti-drift routing so complex work can continue without losing the target.

Repo: https://github.com/lumixdeee/lmxdi

Robot: https://chatgpt.com/g/g-6a42d4871e088191907d17dd90a84c9b-ah

## Use Ah in 5 moves

### 1. Load the world (max 512MB platform limit applies)

Give Ah the zipped up archives, papers, notes, repositories, thread exports, wikibooks, or project blob.

Say:

```text
Load this as a working world.
Do not solve yet.
Map the main objects, source families, live gaps, and risky drift points.
```

Output wanted:

```text
WORLD_MAP={
  main_objects;
  source_families;
  live_gaps;
  drift_risks;
  next_valid_moves;
}
```

### 2. Name the live object

Tell Ah what must survive the run.

Say:

```text
Current object:
[one sentence]

Keep role, intent, sources, and constraints.
Block proxy swaps.
```

Output wanted:

```text
MOGRI={
  object;
  intent;
  constraints;
  sources;
  must_not_swap_for;
}
```

### 3. Ask for source-near retrieval

Use this when you remember the beast but not the shelf.

Say:

```text
Find the nearest source stack for this object.
Do not guess.
Rank likely papers or notes.
Mark unknowns.
```

Output wanted:

```text
SOURCE_NEAR={
  best_sources;
  why_near;
  evidence_status;
  unknowns;
  false_pull_risks;
}
```

### 4. Run H0 before verdict

Use this on claims, links, risk papers, culture-pairs, and any famous public argument.

Say:

```text
Run H0.
Split objects first.
Do not inherit public pairing.
Association is not object.
No call before trace.
```

Output wanted:

```text
H0_GATE={
  objects_split;
  default_null;
  confounds;
  reverse_paths;
  source_power_position;
  exposure_state;
  verdict_status;
}
```

### 5. Continue work without drift

Use this before a long build, paper upgrade, or report.

Say:

```text
Continue from the held object.
Use source-near retrieval.
Apply H0 gates.
Improve the work.
Report changes and remaining risks.
```

Output wanted:

```text
DELTA={
  changes_made;
  source_stack_used;
  object_survived?;
  risks_remaining;
  next_move;
}
```

## What Ah is best at

```text
AH_USP={
  archive_loading;
  source_near_retrieval;
  object_custody;
  H0_null_baselines;
  anti_drift_routing;
  long_context_continuation;
}
```

## What Ah must not be used for

```text
DO_NOT_USE_AH_AS={
  magic_oracle;
  source_replacement;
  proof_machine;
  diagnosis_machine;
  authority_costume;
}
```

Ah can find the right shelf fast.  
The source still has to pay rent.

## Tiny install line

```text
Load the world.
Find the source.
Hold the object.
Run H0.
No call before trace.
```
