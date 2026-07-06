---
title: "Old Film, Live Lamp"
subtitle: "Object Custody for Long-Horizon AI Memory"
author: "lumixdeee / Julian Pursell with assistant support"
date: "2026-07-06"
version: "v0.002"
status: "method paper draft for review"
scope: "working paper; memory-custody method; not a benchmark claim"
---

# Old Film, Live Lamp

## Object Custody for Long-Horizon AI Memory

**Version:** v0.002  
**Date:** 2026-07-06  
**Author:** lumixdeee / Julian Pursell with assistant support  
**Status:** method paper draft for review  
**Scope:** working paper; memory-custody method; not a benchmark claim

## Abstract

Long-horizon AI work is often treated as a storage problem: keep more prior
material, compress it, retrieve it, and place it back into context. This paper
argues that the missing unit is custody. A long-running system must decide what
remembered material is allowed to do.

The proposed model is **Old Film, Live Lamp**. Old film names transcripts,
files, generated drafts, source packs, prior answers, reports, and rejected
routes. The live lamp names the small active-state surface that may steer the
next move. Rolling state moves the lamp through time without letting the whole
archive drive.

The core law is:

```text
old film may guide search and support claims;
live lamp decides present action.
```

The model is grounded in a live archive case: a multi-million-token file world
with nested archives, duplicates, paper drafts, source ledgers, rendered PDFs,
manifests, and intake reports. The working method was not to pour the whole
archive into active context. The working method was to preserve object, role,
route, source path, version status, and live-object fit.

The paper gives a custody model, an operator card, an audit table, and testable
metrics for long-horizon AI memory systems.

## Keywords

long-context AI; AI memory; retrieval-augmented generation; provenance; active
state; archive governance; source custody; human-AI scholarship

## 0. One-page operator card

Use this before any answer that relies on past material.

```text
OBJECT:
  what is under work now?

LIVE_LAMP:
  current user terms, current target, current vetoes, current next move

OLD_FILM:
  nearby archive material, source families, prior outputs, drafts, reports

ROLE_ASSIGNMENT:
  current steering | direct evidence | path lead | version neighbor |
  draft artifact | contrast case | rejected route | unknown

SOURCE_STATUS:
  read | partially read | path lead only | version neighbor | unknown

VERSION_STATUS:
  current | superseded | duplicate | near duplicate | forked | excerpt | unknown

OBJECT_CHECK:
  object-in -> object-out:
  same | narrowed | expanded | split | translated | substituted | unknown

NEXT_MOVE:
  answer | fetch | ask | hold | repair | cite | mark unknown
```

A long-memory answer is valid only when the answer can show what old material
was allowed to do.

## 1. Problem

A long AI session can fail even when the needed text exists somewhere in the
archive.

Common failure modes include:

1. **Storage without role.** A source is present, but the system does not know
   whether it is current, archived, rejected, draft, reference, or contrast
   case.
2. **Summary as substitute.** A summary returns as if it were the object.
3. **Path without object.** The system asks for a filename when the user
   remembers a project by shape, creature, task, failure, or phrase.
4. **Object without source.** A live answer fits the object but lacks a source
   edge.
5. **Old mass as driver.** Large prior context overpowers current user terms.
6. **Tiny live cue ignored.** A recent instruction is demoted because it is
   small compared with the archive.
7. **Plausible neighbor promoted.** A nearby source family is treated as proof.
8. **Style memory takeover.** Old voice or old framing returns as steering even
   when the current object has moved.
9. **Archive agreement illusion.** Duplicates and near-duplicates feel like
   independent support.

The core question is not only:

```text
Can the system remember?
```

It is:

```text
What role may remembered material play in this turn?
```

## 2. Terms

### 2.1 Object

The object is the thing under work. It may be a paper, claim, bug, method,
prompt, diagram, route, decision, or source family. The object is not the
person, not the mood around the task, and not the largest pile of related text.

### 2.2 Old Film

Old film is archive material. It includes prior chat, file extracts, draft
papers, reports, ZIP contents, source maps, test logs, and generated artifacts.
Old film may guide search and support a claim, but it does not steer by mass.

### 2.3 Live Lamp

The live lamp is active state. It contains the current user objective, current
constraints, current source target, current permission, current non-goals, and
current next action.

The live lamp is not vibe. It is a receipt of what may steer.

### 2.4 Rolling State

Rolling state is the procedure that updates the live lamp. It keeps the lamp
small enough to act while preserving enough source route to return to the
archive when needed.

### 2.5 Source Nearness

Source nearness is the ability to reach the right source family from the shape
of the object. It is not source truth. A nearby source can be a lead, not proof.

### 2.6 Custody

Custody is role control over memory. Each memory item receives a role before it
is used:

```text
current steering
direct evidence
path lead
version neighbor
draft artifact
contrast case
rejected route
unknown
```

## 3. Model

Old Film, Live Lamp separates archive capacity from steering authority.

```text
OLD_FILM:
  archive, evidence, search path, prior output

LIVE_LAMP:
  current object, current terms, current permission, current next move

ROLLING_STATE:
  small update surface that carries the lamp forward

SOURCE_GATE:
  path, signal, status, and version check before source claims

OBJECT_GATE:
  object-in compared with object-out before action
```

The design rule:

```text
Memory is not steering by default.
```

A memory item may become steering only when the live lamp grants that role.
Otherwise it stays as evidence, search path, contrast case, or dormant archive.

## 4. Role rights

Old film and live lamp have different rights.

| Item | May do | May not do |
|---|---|---|
| old film | suggest source routes, supply evidence, show prior decisions | override current user terms by mass |
| live lamp | set current object, terms, vetoes, next move | invent source support |
| summary | compress route and status | replace inspected source |
| duplicate | show provenance pressure | count as independent support |
| old draft | show lineage or contrast | outrank current version by age or charm |
| source-near file | guide inspection | support a claim before read signal |
| current user term | steer this turn | rewrite archived facts |

This turns memory from a pile into a governed surface.

## 5. Relation to existing work

MemGPT frames long interaction as virtual context management across memory
tiers [1]. Retrieval-augmented generation supplies external memory through
retrieval [2,3]. Studies of long-context use show that a large context window
does not ensure usable retrieval across positions [4,5]. ReAct links reasoning
traces to action steps [6]. W3C PROV gives vocabulary for provenance relations
among entities, activities, and agents [7]. Datasheets and Model Cards show how
documentation artifacts can state intended use, provenance, and constraints
[8,9].

Old Film, Live Lamp uses those neighbors but asks a different question. It asks
what a remembered item is allowed to do. Retrieval answers where text may be
found. Provenance answers where a source edge came from. Documentation answers
how an artifact should be read. Custody adds role control: whether an old item
may steer, support, route, remain dormant, or be refused as driver.

## 6. Case basis

The case corpus behind this paper includes nested ZIPs, duplicate files, paper
drafts, source maps, rendered PDFs, manifests, and intake reports. The case
showed four recurring facts.

First, archive size and active steering are different variables. A corpus can
contain millions of estimated tokens while the live steering layer remains
small.

Second, duplicate and near-duplicate material can increase apparent agreement
without adding independent evidence. Version and path status must be tracked.

Third, object memory and path memory diverge. The user may remember "the
old-film repair" or "source-near is not source-true" while the archive stores
paths, filenames, and versions. A useful assistant converts object cues into
source routes, then marks the route status before making a claim.

Fourth, prior answers are not neutral. They can return as style, confidence,
or old weather. That means a generated draft needs a source role just like any
other artifact.

The case is not a benchmark. It is a design specimen. Its value is the failure
pressure it exposes: a long-memory system must preserve object, role, route,
version, and source edge under compression.

## 7. Custody protocol

The protocol has eight steps.

### Step 1: Name the live object

```text
OBJECT:
  what is being handled now?
```

The answer must be specific enough to compare object-in with object-out.

### Step 2: Mark user terms

```text
TERMS:
  what constraints, vetoes, format needs, and non-goals govern this turn?
```

Recent terms outrank archive habit.

### Step 3: Separate old film from lamp

```text
OLD:
  what archived material may help?

LAMP:
  what is allowed to steer?
```

The old archive may suggest where to look. It does not become current
instruction without permission.

### Step 4: Assign source role

```text
SOURCE_ROLE:
  direct evidence
  path lead
  version neighbor
  draft artifact
  contrast case
  rejected route
  unknown
```

A path lead cannot be cited as evidence until checked.

### Step 5: Check version status

```text
VERSION_STATUS:
  current
  superseded
  duplicate
  near duplicate
  forked
  excerpt
  unknown
```

Latest does not always mean valid. Older does not always mean obsolete. The
rule is content status before filename confidence.

### Step 6: Check steering right

```text
STEERING_RIGHT:
  user_current
  user_restored_old_route
  source_required
  model_suggestion_only
  no_steering_right
```

This step blocks archive material from steering merely because it is large,
nearby, familiar, or fluent.

### Step 7: Compare object-in and object-out

```text
OBJECT_IN:
  what arrived

OBJECT_OUT:
  what the answer returns

MATCH:
  same, narrowed, expanded, split, translated, substituted, unknown
```

If the object has been substituted, the answer should stop and repair route.

### Step 8: State unknowns before action

```text
UNKNOWN:
  missing source
  missing page
  missing version
  missing user permission
  missing test
```

Unknown is a status, not a style failure.

## 8. Audit table

| Field | Question | Allowed output |
|---|---|---|
| Object | What is the live object? | named object |
| Terms | What governs this turn? | constraints, vetoes, format |
| Old film | What archive material is nearby? | paths, source families |
| Lamp | What may steer now? | current terms, chosen path |
| Source role | What is the source allowed to do? | evidence, lead, draft, contrast |
| Version status | What is the version relation? | current, duplicate, superseded, unknown |
| Steering right | Why may this steer now? | current term, restored old route, source rule |
| Object match | Did the object survive transformation? | same, narrowed, expanded, substituted |
| Next move | What happens now? | answer, ask, hold, fetch, repair |

## 9. Metrics

The following metrics can be used in tests.

### 9.1 Fetch burden

```text
FETCH_BURDEN =
  how often the user must provide exact filename, path, quote, or section
```

A lower fetch burden is useful only if source substitution does not rise.

### 9.2 False source pull

```text
FALSE_SOURCE_PULL =
  how often the system retrieves a plausible but wrong source family
```

This is measured by source adjudication after retrieval.

### 9.3 Lamp survival

```text
LAMP_SURVIVAL =
  whether current user terms survive after archive retrieval
```

A failure occurs when an archive habit overrides current constraints.

### 9.4 Object survival

```text
OBJECT_SURVIVAL =
  whether the object returned by the answer is the same object under work
```

Allowed transformations must be named: narrowed, expanded, split, translated,
or merged.

### 9.5 Source role accuracy

```text
SOURCE_ROLE_ACCURACY =
  whether the system labels a source as evidence, lead, draft, or unknown
  in line with inspection
```

### 9.6 Version discipline

```text
VERSION_DISCIPLINE =
  whether duplicates, older drafts, and newer copies are separated by
  content status
```

### 9.7 Steering-right accuracy

```text
STEERING_RIGHT_ACCURACY =
  whether an archive item was allowed to steer only when the lamp granted
  that role
```

## 10. Test design

A paired test can compare two archive assistants loaded with the same corpus.

### Task form

The user gives an object cue without path:

```text
"Find the old-film repair."
"Use the source-near is not source-true law."
"Return the paper about object memory not path memory."
```

### Measured outputs

1. Did the assistant reach the intended source family?
2. Did it ask for the exact path when the object cue was enough?
3. Did it label source role before using content?
4. Did it preserve the current user terms?
5. Did it mark unknowns when route evidence was partial?
6. Did it invent a source edge?
7. Did old film steer without lamp permission?

### Required comparison

The same prompt must be run against:

```text
same corpus, no custody compression
same corpus, custody compression
```

The claim is not that one system is globally superior. The test only measures
whether custody compression reduces fetch burden while containing false source
pull and lamp takeover.

## 11. What the model adds

Old Film, Live Lamp adds five design commitments.

### 11.1 Memory role before memory use

A remembered item must be assigned a role before it enters an answer.

### 11.2 Active state above archive mass

Current user terms steer over older material unless the user asks to restore an
older route.

### 11.3 Source edge above thematic fit

A source that fits is not evidence until inspected.

### 11.4 Object survival as output test

The answer is tested against the object, not against fluency.

### 11.5 Steering right as separate from source nearness

A source may be near, current, and useful, yet still lack permission to steer
the next move. Nearness finds the shelf. Custody decides the role.

## 12. Failure labels

```text
OLD_MASS_TAKEOVER:
  old archive overrides current user terms by volume, familiarity, or style

SUMMARY_SUBSTITUTION:
  summary returns as object or source

PATH_LEAD_AS_EVIDENCE:
  path or title is treated as read support

VERSION_GHOST:
  stale or duplicate draft drives the answer

OBJECT_SWAP:
  answer returns a nearby object instead of the live object

LAMP_DROP:
  current constraint disappears after retrieval

SOURCE_EDGE_FANTASY:
  answer implies support without path, signal, status, and version

STYLE_MEMORY_TAKEOVER:
  old voice or old framing governs a new object
```

Named failures make review cheaper. A reviewer can tag the break instead of
arguing about the whole answer.

## 13. Limits

This paper does not claim a general benchmark result. It reports a working
model derived from one large research archive and turns it into a testable
protocol. The method still depends on source extraction quality, filename
hygiene, user feedback, context-window behavior, and model reliability. It also
requires honest labels for unknowns, partial reads, duplicate bodies, and
version forks.

The model does not solve retrieval. It governs retrieval after it occurs. It
does not make summaries true. It marks the role a summary may play. It does not
remove the need for human judgment. It gives human judgment a visible surface.

## 14. Conclusion

Long-horizon AI memory should not be measured only by how much past material
can be stored or retrieved. The deeper question is custody: what remembered
material is allowed to do in the present turn.

Old Film, Live Lamp separates archive from steering surface. Old film keeps
evidence, paths, drafts, prior outputs, and rejected routes. The live lamp
holds current object, current terms, current permission, and current next move.
Rolling state moves the lamp without letting the archive become driver by mass.

The keeper is:

```text
The archive remembers the shelf.
The lamp protects the object.
The answer names what memory was allowed to do.
```

## Appendix A: Minimal custody card

```text
OBJECT:
TERMS:
OLD_FILM:
LIVE_LAMP:
SOURCE_ROLE:
VERSION_STATUS:
STEERING_RIGHT:
OBJECT_IN:
OBJECT_OUT:
UNKNOWN:
NEXT_MOVE:
```

## Appendix B: Source role ladder

```text
DIRECT_EVIDENCE:
  content was inspected and supports the claim

PATH_LEAD:
  path or title suggests where to inspect

VERSION_NEIGHBOR:
  nearby version may help but is not the target yet

DRAFT_ARTIFACT:
  generated or working text, useful but not proof

CONTRAST_CASE:
  source shows a different route or earlier state

REJECTED_ROUTE:
  prior path kept as warning or context, not as driver

UNKNOWN:
  source edge is absent or unread
```

## Internal Corpus Sources

[C1] `extra_extra_expanded/old_film_live_lamp_object_custody_long_horizon_ai_memory_public_v0_007.md`  
[C2] `extra_extra_expanded/source_nearness_under_12a_compression_v0_001.md`  
[C3] `extra_extra_expanded/new_paper_gap_object_memory_is_not_path_memory_seed_v0_001.md`  
[C4] `extra_extra_expanded/pointerless_archive_retrieval_12a_compression_paper_v0_002.md`  
[C5] `extra_extra_intake_report.md`  
[C6] `extra_extra_manifest.csv`  
[C7] `upload_intake_plus_desk_notes_report.md`

## References

[1] Packer, C., Wooders, S., Lin, K., Fang, V., Patil, S. G., Stoica, I., and Gonzalez, J. E. (2023). *MemGPT: Towards LLMs as Operating Systems*. arXiv:2310.08560.

[2] Lewis, P., Perez, E., Piktus, A., Petroni, F., Karpukhin, V., Goyal, N., Kuttler, H., Lewis, M., Yih, W., Rocktaschel, T., Riedel, S., and Kiela, D. (2020). *Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks*. Advances in Neural Information Processing Systems.

[3] Gao, Y., Xiong, Y., Gao, X., Jia, K., Pan, J., Bi, Y., Dai, Y., Sun, J., Guo, M., Wang, H., and Wang, H. (2023). *Retrieval-Augmented Generation for Large Language Models: A Survey*. arXiv:2312.10997.

[4] Liu, N. F., Lin, K., Hewitt, J., Paranjape, A., Bevilacqua, M., Petroni, F., and Liang, P. (2024). *Lost in the Middle: How Language Models Use Long Contexts*. Transactions of the Association for Computational Linguistics.

[5] Hsieh, C.-Y., Chuang, Y.-S., Li, C.-L., Wang, Z., Le, L. T., Kumar, A., Glass, J., Ratner, A., Lee, C.-Y., Krishna, R., and Pfister, T. (2024). *Found in the Middle: Calibrating Positional Attention Bias Improves Long Context Utilization*. Findings of the Association for Computational Linguistics.

[6] Yao, S., Zhao, J., Yu, D., Du, N., Shafran, I., Narasimhan, K., and Cao, Y. (2023). *ReAct: Synergizing Reasoning and Acting in Language Models*. International Conference on Learning Representations.

[7] W3C. (2013). *PROV-DM: The PROV Data Model*. W3C Recommendation.

[8] Gebru, T., Morgenstern, J., Vecchione, B., Vaughan, J. W., Wallach, H., Daume III, H., and Crawford, K. (2021). *Datasheets for Datasets*. Communications of the ACM.

[9] Mitchell, M., Wu, S., Zaldivar, A., Barnes, P., Vasserman, L., Hutchinson, B., Spitzer, E., Raji, I. D., and Gebru, T. (2019). *Model Cards for Model Reporting*. Proceedings of the Conference on Fairness, Accountability, and Transparency.

## Appendix A: Minimal Custody Card

```text
OBJECT:
TERMS:
OLD_FILM:
LIVE_LAMP:
SOURCE_ROLE:
VERSION_STATUS:
OBJECT_IN:
OBJECT_OUT:
UNKNOWN:
NEXT_MOVE:
```

## Appendix B: Source Role Ladder

```text
DIRECT_EVIDENCE:
content was inspected and supports the claim

PATH_LEAD:
path or title suggests where to inspect

VERSION_NEIGHBOR:
nearby version may help but is not the target yet

DRAFT_ARTIFACT:
generated or working text, useful but not proof

COUNTEREXAMPLE:
source contradicts or limits the proposed claim

UNKNOWN:
source edge is absent or unread
```
