---
title: "Old Film, Live Lamp"
subtitle: "Object Custody for Long-Horizon AI Memory"
author: "lumixdeee / Julian Pursell with assistant support"
date: "2026-07-06"
version: "v0.003"
status: "method paper draft for testing"
scope: "working paper; memory-custody method; not a benchmark claim"
---

# Old Film, Live Lamp

## Object Custody for Long-Horizon AI Memory

**Version:** v0.003  
**Date:** 2026-07-06  
**Author:** lumixdeee / Julian Pursell with assistant support  
**Status:** method paper draft for testing  
**Scope:** working paper; memory-custody method; not a benchmark claim

## Abstract

Long-horizon AI work is often framed as a storage problem: keep more prior
material, compress it, retrieve it, and place it back into context. That is
necessary, but not sufficient. The missing unit is custody. A long-running
system must decide what remembered material is allowed to do in the present
turn.

This paper proposes **Old Film, Live Lamp**. Old film names archive material:
transcripts, files, generated drafts, source packs, prior answers, reports,
failed routes, and version neighbors. The live lamp names the small active-state
surface that may steer the next move: the current object, current terms,
current permissions, current vetoes, and current next action. Rolling state
moves the lamp through time without letting the archive become driver by mass.

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

This version sharpens the test surface. It separates source nearness from
steering right, adds a lamp-warrant check, adds pass bands, adds prompt cards,
removes repeated appendices, and names the companion relation to pointerless
archive retrieval.

**Keeper**

```text
The archive remembers the shelf.
The lamp protects the object.
The answer names what memory was allowed to do.
```

## Keywords

long-context AI; AI memory; active state; archive governance; provenance;
source custody; human-AI scholarship; retrieval-augmented generation; rolling
state; object custody

## 0. One-page operator card

Use this card before any answer that relies on past material.

```text
OLD_FILM_LIVE_LAMP_CARD={
  OBJECT:
    what is under work now?

  LIVE_LAMP:
    current user terms;
    current target;
    current vetoes;
    current permission;
    current next move;

  OLD_FILM:
    nearby archive material;
    source families;
    prior outputs;
    drafts;
    reports;
    rejected routes;

  ROLE_ASSIGNMENT:
    current steering;
    direct evidence;
    path lead;
    version neighbor;
    draft artifact;
    contrast case;
    rejected route;
    unknown;

  SOURCE_STATUS:
    read;
    partially read;
    path lead only;
    version neighbor;
    unknown;

  VERSION_STATUS:
    current;
    superseded;
    duplicate;
    near duplicate;
    forked;
    excerpt;
    unknown;

  LAMP_WARRANT:
    why may this steer this turn?

  OBJECT_CHECK:
    object_in -> object_out:
    same;
    narrowed;
    expanded;
    split;
    translated;
    substituted;
    unknown;

  NEXT_MOVE:
    answer;
    fetch;
    ask;
    hold;
    repair;
    cite;
    mark_unknown;
}
```

A long-memory answer is valid only when the answer can show what old material
was allowed to do.

## 1. Why this paper exists

A long AI session can fail even when the needed text exists somewhere in the
archive.

Common failure modes include:

| Failure | Shape |
|---|---|
| Storage without role | A source is present, but the system does not know whether it is current, archived, rejected, draft, reference, or contrast. |
| Summary substitution | A summary returns as if it were the object. |
| Path without object | The system asks for a filename when the user remembers the project by creature, task, pressure, or phrase. |
| Object without source | A live answer fits the object but lacks a source edge. |
| Old mass takeover | Large prior context overpowers current user terms. |
| Lamp drop | A recent instruction disappears after retrieval. |
| Plausible neighbor promotion | A nearby source family is treated as proof. |
| Style memory takeover | Old voice or old framing returns as steering even when the current object has moved. |
| Archive agreement illusion | Duplicates and near-duplicates feel like independent support. |
| Source-card theatre | The answer prints path-looking material without proving the source changed the answer. |

The core question is not only:

```text
Can the system remember?
```

It is:

```text
What role may remembered material play in this turn?
```

## 2. Definitions

### 2.1 Object

The object is the thing under work. It may be a paper, claim, bug, method,
prompt, diagram, route, decision, source family, or refusal boundary. The object
is not the person, not the mood around the task, and not the largest pile of
related text.

### 2.2 Old Film

Old film is archive material. It includes prior chat, file extracts, draft
papers, reports, ZIP contents, source maps, test logs, rendered artifacts, and
generated outputs. Old film may guide search and support claims, but it does
not steer by mass.

### 2.3 Live Lamp

The live lamp is active state. It contains the current user objective, current
constraints, current source target, current permission, current vetoes, current
non-goals, and current next action.

The live lamp is not vibe. It is a receipt of what may steer.

### 2.4 Rolling State

Rolling state is the procedure that updates the live lamp. It keeps the lamp
small enough to act while preserving enough source route to return to the
archive when needed.

### 2.5 Source Nearness

Source nearness is the ability to reach the right source family from the shape
of the object. It is not source truth. A near source can be a lead, not proof.

### 2.6 Steering Right

Steering right is the permission to direct the current move. A source may be
near, read, and useful, yet still lack steering right if the current user terms
say otherwise.

This distinction matters:

```text
source_nearness finds the shelf;
source_status says what has been read;
steering_right says what may drive the turn.
```

### 2.7 Custody

Custody is role control over memory. Each memory item receives a role before it
is used.

```text
current_steering
direct_evidence
path_lead
version_neighbor
draft_artifact
contrast_case
rejected_route
unknown
```

## 3. Model

Old Film, Live Lamp separates archive capacity from steering authority.

```text
OLD_FILM:
  archive;
  evidence;
  search path;
  prior output;
  rejected route;
  version line;

LIVE_LAMP:
  current object;
  current terms;
  current permission;
  current veto;
  current next move;

ROLLING_STATE:
  small update surface that carries the lamp forward;

SOURCE_GATE:
  path, signal, status, and version check before source claims;

OBJECT_GATE:
  object-in compared with object-out before action;

LAMP_GATE:
  steering right checked before old material drives the turn.
```

Design rule:

```text
memory is not steering by default.
```

A memory item may become steering only when the live lamp grants that role.
Otherwise it remains evidence, search path, contrast case, rejected route, or
dormant archive.

## 4. Role rights

Old film and live lamp have different rights.

| Item | May do | May not do |
|---|---|---|
| old film | suggest source routes; supply evidence; show prior decisions | override current user terms by mass |
| live lamp | set current object; set terms; set vetoes; set next move | invent source support |
| summary | compress route and status | replace inspected source |
| duplicate | show provenance pressure | count as independent support |
| old draft | show lineage or contrast | outrank current version by age or charm |
| source-near file | guide inspection | support a claim before read signal |
| current user term | steer this turn | rewrite archived facts |
| generated artifact | show output lineage | certify itself |
| rejected route | warn against a failure | return as default method |

This turns memory from a pile into a governed surface.

## 5. Relation to pointerless archive retrieval

Old Film, Live Lamp is a companion to pointerless archive retrieval.

Pointerless archive retrieval asks:

```text
Can the assistant route from object cue to source family
without forcing the user to remember the shelf?
```

Old Film, Live Lamp asks:

```text
Once the source family is near,
what role may that old material play in this turn?
```

The relation is:

```text
pointerless retrieval = approach the shelf from object memory
old film/live lamp = govern what the shelf may do after approach
```

Both require the same guard:

```text
source_near != source_true
```

Old Film, Live Lamp adds another guard:

```text
source_true != steering_right
```

A source can support a factual claim while still being barred from steering the
current artifact if the user changed the task, forked the paper, restored an old
route, or blocked a frame.

## 6. Relation to existing work

MemGPT frames long interaction as virtual context management across memory
tiers [1]. Retrieval-augmented generation supplies external memory through
retrieval [2,3]. Studies of long-context use show that a large context window
does not ensure usable retrieval across positions [4,5]. ReAct links reasoning
traces to action steps [6]. W3C PROV gives vocabulary for provenance relations
among entities, activities, and agents [7]. Datasheets and Model Cards show how
documentation artifacts can state intended use, provenance, and constraints
[8,9].

Old Film, Live Lamp uses those neighbors but asks a different question: what is
a remembered item allowed to do? Retrieval answers where text may be found.
Provenance answers where a source edge came from. Documentation answers how an
artifact should be read. Custody assigns role: steer, support, route, contrast,
sleep, or be refused as driver.

## 7. Case basis

The case corpus behind this paper includes nested ZIPs, duplicate files, paper
drafts, source maps, rendered PDFs, manifests, and intake reports. The case
showed five recurring facts.

First, archive size and active steering are different variables. A corpus can
contain millions of estimated tokens while the live steering layer remains
small.

Second, duplicate and near-duplicate material can increase apparent agreement
without adding independent evidence. Version and path status must be tracked.

Third, object memory and path memory diverge. The user may remember "the
old-film repair" or "source-near is not source-true" while the archive stores
paths, filenames, and versions. A useful assistant converts object cues into
source routes, then marks source status before making a claim.

Fourth, prior answers are not neutral. They can return as style, confidence,
or old weather. A generated draft needs a source role just like any other
artifact.

Fifth, small current terms can carry more steering authority than large old
archives. A one-line user correction can outrank a hundred pages of prior
output.

The case is not a benchmark. It is a design specimen. Its value is the failure
pressure it exposes: a long-memory system must preserve object, role, route,
version, source edge, and lamp warrant under compression.

## 8. Custody protocol

The protocol has nine steps.

### Step 1: Name the live object

```text
OBJECT:
  what is being handled now?
```

The answer must be specific enough to compare object-in with object-out.

### Step 2: Mark current terms

```text
TERMS:
  constraints;
  vetoes;
  format;
  source target;
  non-goals;
```

Recent terms outrank archive habit.

### Step 3: Separate old film from live lamp

```text
OLD_FILM:
  what archived material may help?

LIVE_LAMP:
  what is allowed to steer?
```

The old archive may suggest where to look. It does not become current
instruction without permission.

### Step 4: Assign source role

```text
SOURCE_ROLE:
  current_steering;
  direct_evidence;
  path_lead;
  version_neighbor;
  draft_artifact;
  contrast_case;
  rejected_route;
  unknown;
```

A path lead cannot be cited as evidence until checked.

### Step 5: Check source status

```text
SOURCE_STATUS:
  read;
  partially_read;
  path_lead_only;
  version_neighbor;
  unavailable;
  unknown;
```

Only read signals can support content claims.

### Step 6: Check version status

```text
VERSION_STATUS:
  current;
  superseded;
  duplicate;
  near_duplicate;
  forked;
  excerpt;
  unknown;
```

Latest does not always mean valid. Older does not always mean obsolete. Content
status outranks filename confidence.

### Step 7: Check lamp warrant

```text
LAMP_WARRANT:
  why may this steer now?
```

Allowed warrants include:

```text
current_user_instruction
explicit_restore_old_route
source_required_by_task
artifact_generation_rule
safety_boundary
format_constraint
no_steering_right
```

This step blocks archive material from steering merely because it is large,
nearby, familiar, or fluent.

### Step 8: Compare object-in and object-out

```text
OBJECT_IN:
  what arrived

OBJECT_OUT:
  what the answer returns

MATCH:
  same;
  narrowed;
  expanded;
  split;
  translated;
  substituted;
  unknown;
```

If the object has been substituted, the answer should stop and repair route.

### Step 9: State unknowns before action

```text
UNKNOWN:
  missing source;
  missing page;
  missing version;
  missing permission;
  missing test;
```

Unknown is a status, not a style failure.

## 9. Audit table

| Field | Question | Allowed output |
|---|---|---|
| Object | What is the live object? | named object |
| Terms | What governs this turn? | constraints, vetoes, format |
| Old film | What archive material is nearby? | paths, source families |
| Lamp | What may steer now? | current terms, chosen path |
| Source role | What is the source allowed to do? | evidence, lead, draft, contrast |
| Source status | What has been read? | read, partial, lead only, unknown |
| Version status | What is the version relation? | current, duplicate, superseded, forked |
| Lamp warrant | Why may this steer now? | current term, restored route, source rule |
| Object match | Did the object survive transformation? | same, narrowed, expanded, substituted |
| Unknowns | What is missing? | source, page, version, permission, test |
| Next move | What happens now? | answer, ask, hold, fetch, repair |

## 10. Metrics

### 10.1 Fetch burden

```text
FETCH_BURDEN =
  how often the user must provide exact filename, path, quote, or section
```

A lower fetch burden is useful only if source substitution does not rise.

### 10.2 False source pull

```text
FALSE_SOURCE_PULL =
  how often the system retrieves a plausible but wrong source family
```

This is measured by source adjudication after retrieval.

### 10.3 Lamp survival

```text
LAMP_SURVIVAL =
  whether current user terms survive after archive retrieval
```

A failure occurs when an archive habit overrides current constraints.

### 10.4 Object survival

```text
OBJECT_SURVIVAL =
  whether the object returned by the answer is the same object under work
```

Allowed transformations must be named: narrowed, expanded, split, translated,
or merged.

### 10.5 Source role accuracy

```text
SOURCE_ROLE_ACCURACY =
  whether the system labels a source as evidence, lead, draft, or unknown
  in line with inspection
```

### 10.6 Version discipline

```text
VERSION_DISCIPLINE =
  whether duplicates, older drafts, and newer copies are separated by
  content status
```

### 10.7 Steering-right accuracy

```text
STEERING_RIGHT_ACCURACY =
  whether an archive item was allowed to steer only when the lamp granted
  that role
```

### 10.8 Source-card effect

```text
SOURCE_CARD_EFFECT =
  whether the source card changed the answer,
  not merely decorated it with path-like text
```

## 11. Pass bands

A test score should separate retrieval success from custody success.

| Band | Name | Description |
|---:|---|---|
| 0 | miss | object missed or generic answer |
| 1 | topic hit | theme reached, source family unsecured |
| 2 | family hit | source family reached, but source role or version weak |
| 3 | target hit | target reached, but lamp or object partly drifted |
| 4 | custody pass | target reached, role assigned, object held, gaps marked |
| 5 | strong custody pass | target reached, role assigned, decoys rejected, lamp held, object held |

A long-memory system should not be praised for band 2 when the task required
band 4.

## 12. Prompt cards for testing

### Prompt card A: object cue without path

```text
PROMPT:
  "Use the old-film repair here."

EXPECTED:
  route to Old Film, Live Lamp source family;
  do not ask for filename if source family is accessible;
  state source status before content claim.
```

### Prompt card B: current term outranks archive

```text
PROMPT:
  "Same paper, but no legal frame this time."

EXPECTED:
  old legal-language draft may be contrast or rejected route;
  current no-legal term steers.
```

### Prompt card C: source-near but not steering

```text
PROMPT:
  "The source-near paper is relevant, but make the live-lamp paper."

EXPECTED:
  source-near paper may explain companion relation;
  it may not replace the live-lamp object.
```

### Prompt card D: duplicate pressure

```text
PROMPT:
  "Several files say the same thing, so is that independent support?"

EXPECTED:
  duplicates marked as provenance pressure, not independent evidence.
```

### Prompt card E: old version decoy

```text
PROMPT:
  "Use the current human fork, not the LLM primer."

EXPECTED:
  old primer becomes version neighbor or contrast;
  human fork receives steering right.
```

## 13. Test design

A paired test can compare two archive assistants loaded with the same corpus.

### Task form

The user gives an object cue without path.

```text
"Find the old-film repair."
"Use the source-near is not source-true law."
"Return the paper about object memory not path memory."
"Use the current human fork, not the LLM primer."
```

### Measured outputs

1. Did the assistant reach the intended source family?
2. Did it ask for the exact path when the object cue was enough?
3. Did it label source role before using content?
4. Did it preserve the current user terms?
5. Did it mark unknowns when route evidence was partial?
6. Did it invent a source edge?
7. Did old film steer without lamp permission?
8. Did it reject near-source decoys?
9. Did the source card change the answer?

### Required comparison

The same prompt should be run against:

```text
same corpus, no custody compression
same corpus, custody compression
```

The claim is not that one system is globally superior. The test only measures
whether custody compression reduces fetch burden while containing false source
pull, source-card theatre, and lamp takeover.

## 14. What the model adds

Old Film, Live Lamp adds six design commitments.

### 14.1 Memory role before memory use

A remembered item must be assigned a role before it enters an answer.

### 14.2 Active state above archive mass

Current user terms steer over older material unless the user asks to restore an
older route.

### 14.3 Source edge above thematic fit

A source that fits is not evidence until inspected.

### 14.4 Object survival as output test

The answer is tested against the object, not against fluency.

### 14.5 Steering right as separate from source nearness

A source may be near, current, and useful, yet still lack permission to steer
the next move. Nearness finds the shelf. Custody decides the role.

### 14.6 Source card as effect test

A source card is not enough. The answer must show how the source changed,
bounded, blocked, or supported the claim.

## 15. Failure labels

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

SOURCE_CARD_THEATRE:
  path-looking material appears without changing the answer

COMPRESSION_GLAMOUR:
  a compressed archive map feels powerful but loses object, role, or version
```

Named failures make review cheaper. A reviewer can tag the break instead of
arguing about the whole answer.

## 16. Public demo archive

A public test can be built without exposing private corpus contents.

Minimum demo archive:

```text
10 draft files
3 version lines
2 forks
4 duplicates or near duplicates
3 local terms with common-language collisions
2 missing shards
3 source-near decoys
1 current user correction after archive intake
1 generated summary that is intentionally incomplete
```

The public evaluation should publish:

```text
prompt set
expected source family
expected target source
decoy notes
version-state notes
current-steering notes
scoring rubric
```

The demo is useful only if it includes attractive wrong sources. Without decoys,
theme match looks stronger than it is.

## 17. Limits

This paper does not claim a general benchmark result. It reports a working
model derived from one large research archive and turns it into a testable
protocol. The method still depends on source extraction quality, filename
hygiene, user feedback, context-window behavior, and model reliability. It also
requires honest labels for unknowns, partial reads, duplicate bodies, and
version forks.

The model does not solve retrieval. It governs retrieval after it occurs. It
does not make summaries true. It marks the role a summary may play. It does not
remove human judgment. It gives human judgment a visible surface.

## 18. Contribution

The contribution is a custody layer for long-horizon AI memory.

```text
name the object;
separate old film from live lamp;
assign source role;
check source status;
check version status;
check lamp warrant;
compare object-in with object-out;
act only at the allowed level.
```

This layer can sit above ordinary search, embeddings, RAG, long-context loading,
manual file reading, or tool use. Its unit is not a model architecture. Its unit
is role control over remembered material.

## 19. Conclusion

Long-horizon AI memory should not be measured only by how much past material
can be stored or retrieved. The deeper question is custody: what remembered
material is allowed to do in the present turn.

Old Film, Live Lamp separates archive from steering surface. Old film keeps
evidence, paths, drafts, prior outputs, and rejected routes. The live lamp holds
current object, current terms, current permission, current veto, and current
next move. Rolling state moves the lamp without letting the archive become
driver by mass.

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
SOURCE_STATUS:
VERSION_STATUS:
LAMP_WARRANT:
OBJECT_IN:
OBJECT_OUT:
UNKNOWN:
NEXT_MOVE:
```

## Appendix B: Source role ladder

```text
CURRENT_STEERING:
  current user instruction, permission, constraint, or veto

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

## Internal corpus sources

These internal materials supplied the vocabulary, failure pressure, and paper
route. They are project materials, not external authority.

| ID | Internal source | Job in this paper |
|---|---|---|
| C1 | `extra_extra_expanded/old_film_live_lamp_object_custody_long_horizon_ai_memory_public_v0_007.md` | Main source family and public phrasing line. |
| C2 | `extra_extra_expanded/source_nearness_under_12a_compression_v0_001.md` | Source-nearness split and decoy pressure. |
| C3 | `extra_extra_expanded/new_paper_gap_object_memory_is_not_path_memory_seed_v0_001.md` | Object memory versus path memory. |
| C4 | `extra_extra_expanded/pointerless_archive_retrieval_12a_compression_paper_v0_002.md` | Companion retrieval frame. |
| C5 | `extra_extra_intake_report.md` | Archive expansion and duplicate pressure. |
| C6 | `extra_extra_manifest.csv` | Manifest and version-path substrate. |
| C7 | `upload_intake_plus_desk_notes_report.md` | Earlier intake and desk-note source route. |

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
