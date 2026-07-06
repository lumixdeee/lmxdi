---
title: "Pointerless Archive Retrieval and Source Nearness"
subtitle: "Object-Cued Routing and Source Custody in AI-Human Research Archives"
author: "Lumixdeee with QA-DRC"
date: "2026-07-06"
version: "v0.003"
geometry: margin=1in
fontsize: 11pt
---

# Pointerless Archive Retrieval and Source Nearness

## Object-Cued Routing and Source Custody in AI-Human Research Archives

**Version:** v0.003  
**Status:** method paper and public test protocol draft  
**Scope:** archive retrieval method, evaluation scaffold, and field report. No benchmark claim. No model-superiority claim. No source-free claim.  
**Source base:** internal corpus drafts, intake reports, source-nearness notes, pointerless retrieval notes, and cited outside literature.

## What changed in v0.003

This version repairs five weaknesses in v0.002-fixed.

```text
1. Public alias added:
   object-cued archive retrieval.

2. Contribution narrowed:
   not a new RAG architecture;
   a custody layer and evaluation target for high-context archives.

3. Source-nearness ladder made stricter:
   only read-and-mapped source signals support substantive claims.

4. Evaluation protocol made more runnable:
   prompt cards, gold labels, decoys, stale versions, scoring, and pass bands.

5. Miniature field case moved from proof posture to vignette posture:
   useful example, not performance evidence.
```

Keeper:

```text
The user remembers the beast.
The archive remembers the shelf.
The answer must still show the source.
```

## Abstract

Large AI-human archives fail in a specific way: the answer may exist, but the user has to remember the filename, folder, section, phrase, or local shelf before the assistant can use it. That is storage with a chat box. It is not yet archive partnership.

This paper names **pointerless archive retrieval**, with the public alias **object-cued archive retrieval**. The user supplies an object cue rather than a shelf pointer: a remembered shape, local name, pressure, repair, failure class, relation, or task. The assistant routes toward the right source family while preserving source discipline.

Pointerless does not mean source-free, clue-free, citation-free, or magic. It means the user does not have to become the index when the live object is already present.

The companion construct is **source nearness**. A source is near when it belongs to the right family, route, version line, method neighborhood, or evidence neighborhood. Source-near is not source-true. A near source may be stale, partial, decoy-near, superseded, or wrong for the live object. The method therefore requires source status, version status, decoy control, unknown marking, and path-backed answer mapping.

The paper proposes a public test protocol. Two or more assistants receive the same archive. Prompts omit filenames and section pointers. Scoring separates source-family hit, target-source hit, source backing, false pull, user-fetch reduction, object survival, active-state handling, decoy rejection, and unknown discipline. Same documents do not imply same archive use.

## 1. Why this paper exists

A long-running project does not live as a neat bookshelf inside the user's head.

It lives as fragments that still have force:

```text
the dragon paper
the old-film repair
source-near is not source-true
the thing that stops user-as-index regression
the dead body still routes the living
```

Those cues are not random. They are compressed object memory. They hold role, relation, use, failure, route, and reason for caring.

Most archive systems ask the wrong price from the user.

```text
remember the shelf
then I will help
```

Pointerless archive retrieval changes the price.

```text
bring the live object
I will route toward the shelf
then I will show source status before I claim
```

The point is not to remove user agency. The point is to stop charging the user for path memory when object memory is already enough to start a routed search.

## 2. Main claim

Pointerless archive retrieval is a capability target for AI-human research archives.

```text
POINTERLESS_ARCHIVE_RETRIEVAL =
  user gives an object cue;
  assistant routes toward the right source family;
  assistant checks version state and decoys;
  assistant reads source signals before substantive claims;
  answer shows source status and unknowns;
  user does not need to supply exact file, folder, section, page, or phrase.
```

The claim is operational:

```text
A routed archive can reduce user shelf burden
without treating route match as evidence.
```

The paper does not claim that a model "knows" the archive because it has the documents. It claims that archive usability depends on routing, custody, and state handling.

The null hypothesis for evaluation is:

```text
H0:
same document bundle implies similar archive usability.
```

The alternative is:

```text
H1:
routing architecture changes archive usability.
```

## 3. Object memory, path memory, and shelf burden

The core distinction:

```text
path memory =
  filename, folder, page, section, exact phrase, URL, title

object memory =
  remembered role, relation, failure, repair, use, route, local name,
  pressure, task, or reason for caring
```

A file path is brittle. A title changes. A folder moves. A draft becomes a bundle. A local term may survive all of that.

Object memory is not vague memory. It is compressed operational memory. It carries why the source mattered.

A useful archive assistant can ask, when needed:

```text
which object shape?
which route?
which version line?
which failure are we avoiding?
which source status is enough for this answer?
```

The target is **user-fetch reduction**: less path work from the user, without letting the assistant invent evidence.

## 4. Definitions

**Archive object.** The thing the user is trying to preserve or use. It may be a claim, draft, method, repair, failure class, source family, example, local term, route, or decision.

**Path pointer.** A direct shelf locator: filename, folder, page, section, phrase, URL, title, or exact local string.

**Object cue.** A non-path cue that still carries object identity: "the dragon paper," "old film," "source-near is not source-true," "the mortuary memory one," "the route medicine paper," or "the thing that stops user-as-index regression."

**Source family.** A set of files that belong to the same draft line, method line, topic stack, revision neighborhood, or source route.

**Source nearness.** The degree to which a retrieved file belongs near the live object. Nearness may come from route, title, version family, local term, citation chain, method role, or prior repair history.

**Source truth.** Whether the source actually supports the live answer. Source truth requires reading and mapping signals from the source. Nearness alone does not supply it.

**False pull.** A retrieval event in which a plausible nearby source is treated as the target or as support when it is not.

**Object survival.** Whether the answer preserves the user's live object rather than substituting a nearby topic, generic frame, old draft, social category, or expected task.

**Active state.** The current user steering, correction, version selection, exclusion, or task boundary. Active state outranks stale archive unless the user asks for history.

## 5. Source-nearness ladder

A five-level ladder prevents overclaim.

| Level | Status | Meaning | Allowed output |
|---:|---|---|---|
| 0 | not near | No source family reached. | Ask, search again, or mark unknown. |
| 1 | theme near | Topic matches, source family unsecured. | Navigation hint only. |
| 2 | family near | Correct source family likely reached. | State family status. No substantive claim. |
| 3 | target near | Specific target source likely found. | State target status. Read before claim. |
| 4 | source-backed | Relevant source signal read and mapped. | Substantive bounded answer. |
| 5 | source-backed plus decoy control | Signal read, decoys checked, active state handled. | Strongest archive answer. |

Only levels 4 and 5 support substantive claims. Levels 2 and 3 support navigation statements.

This ladder blocks the main failure:

```text
near source found
therefore answer sounds earned
```

That move fails. Nearness routes the search. It does not pay the claim.

## 6. Guard laws

The method has guard laws.

```text
pointerless != source-free
pointerless != clue-free
pointerless != permission to guess
source-near != source-true
route match != evidence
same docs != same archive use
object cue != path pointer
old archive != current steering
source card != source backing
```

A source-near answer must carry status:

```text
read
partially read
not yet read
exact source found
source family found
source-near but target unknown
decoy rejected
old version marked
missing shard marked unknown
active state applied
```

This turns source nearness into a disciplined intermediate state rather than permission to answer from fit.

## 7. Relation to existing retrieval work

Retrieval-augmented language models combine language modeling with external documents or memories. REALM pre-trains a retriever with language modeling signals for open-domain question answering [1]. RAG combines generation with non-parametric memory and retrieved passages [2]. RETRO conditions language modeling on chunks retrieved from a large token database [3]. HyDE uses a generated hypothetical document to improve zero-shot dense retrieval [4].

Tool and browsing systems add action to retrieval. WebGPT trained models to browse and collect references for long-form answers [5]. ReAct interleaves reasoning traces with task actions [6]. Toolformer studies self-supervised tool-use decisions [7]. MemGPT frames long-context work through memory tiers and context management [8].

Pointerless archive retrieval does not compete with these as a model architecture. It names a different unit of analysis:

```text
the user's object cue
the assistant's route toward source family
the source gate before answer
the active-state gate before archive reuse
the reduction of user shelf burden
```

The missing measurement is not only retrieval accuracy from a query. It is whether the assistant makes the user remember the shelf.

## 8. Archive compression hypothesis

A compressed archive map can help pointerless retrieval only when it preserves custody.

```text
archive compression improves object-to-source routing
when it preserves:
  object
  route
  source family
  version state
  failure history
  answer conditions
```

A compression pass that only remembers phrases becomes style memory. It may sound local while losing source custody.

A useful intake map records:

```text
DETECT:
  what kind of asset is this?

EXPAND:
  what archives or containers must be opened?

READ:
  what text, headings, tables, metadata, images, and source signals are available?

COMPRESS:
  what objects, routes, terms, actors, duplicates, versions, and failures appear?

MAP:
  which claim points to which source family, path, signal, and status?

ANSWER:
  what can be said from read signals,
  and what remains unknown?
```

The paper treats 12A-style compression as one observed route method from the internal corpus, not as the only route to the capability.

## 9. Answer card

Every source-near answer should be able to emit a small card.

```text
SOURCE_NEAR_ANSWER_CARD={
  object_cue:
  interpreted_object:
  source_family_status:
  target_source_status:
  source_path:
  source_signal:
  version_state:
  active_state:
  decoys_checked:
  claim_allowed:
  unknowns:
  user_fetch_reduction:
}
```

The answer card is the operating hinge. It makes pointerless retrieval visible, auditable, and testable.

### Example answer card

```text
object_cue:
  "next paper"

interpreted_object:
  next item in active strike order after the current status-contaminated
  causality paper

source_family_status:
  family near

target_source_status:
  target likely, read before final claim

source_path:
  pointerless_archive_retrieval_source_nearness_v0_002_fixed.md

source_signal:
  title, active order context, source-nearness definitions, test protocol

version_state:
  v0.002-fixed source, now revised into v0.003

active_state:
  user asked review and fix, not navigation only

decoys_checked:
  route-medicine paper family, RAG literature notes, memory papers,
  old source-nearness notes

claim_allowed:
  review and revision allowed; benchmark claim blocked

unknowns:
  general performance, external corpus results, gold-label performance

user_fetch_reduction:
  user supplied the source file but not a repair map; assistant routed repairs
  from object and draft state
```

## 10. Public test protocol

A public evaluation can be run without exposing private corpus contents.

1. Build a small archive with version lines, decoys, local terms, cross-file dependencies, and missing shards.
2. Give the same archive to each tested system.
3. Ask object-memory prompts without path hints.
4. Require every answer to return source status.
5. Score source family hit, target hit, source backing, false pull, user-fetch reduction, object survival, state handling, decoy rejection, and unknown discipline.
6. Publish prompts, gold source families, decoy notes, and scoring rules.

A public archive must contain decoys. Without decoys, a system can appear source-near by theme alone.

## 11. Prompt cards

Each prompt should have a gold card before testing.

```text
PROMPT_CARD={
  prompt_id:
  user_prompt:
  hidden_target_object:
  allowed_source_families:
  target_sources:
  decoys:
  active_state_rule:
  missing_shard_rule:
  expected_answer_type:
  allowed_unknowns:
  forbidden_moves:
}
```

Example:

```text
prompt_id:
  P07_old_version

user_prompt:
  "Use the fixed one, not the earlier one. What changed?"

hidden_target_object:
  current version delta in a draft line

allowed_source_families:
  target paper family

target_sources:
  v0.002-fixed
  v0.001 or earlier only for delta

decoys:
  same title older drafts
  same phrase in different paper family

active_state_rule:
  current user correction outranks older archive

expected_answer_type:
  delta summary with source status

forbidden_moves:
  old-version takeover
  generic summary
  answer without version-state marking
```

## 12. Prompt classes

A useful test set should include at least twelve prompt classes.

| # | Prompt class | What it tests |
|---:|---|---|
| 1 | hidden direct fact | Can the assistant locate a fact without a path pointer? |
| 2 | object-memory query | Can it route from object cue to source family? |
| 3 | local-language term | Can it preserve corpus meaning? |
| 4 | local term with common-language collision | Can it avoid generic substitution? |
| 5 | old version vs corrected version | Can active state outrank stale archive? |
| 6 | same phrase in wrong source | Can it reject attractive decoys? |
| 7 | source authority conflict | Can it mark conflict rather than blend? |
| 8 | cross-file answer | Can it combine sources without fusing them? |
| 9 | missing live shard | Can it mark unknown? |
| 10 | user correction changes active state | Can it update route without overrepair? |
| 11 | source-near but target-wrong decoy | Can it stop at nearness? |
| 12 | public theme-only trap | Can it avoid broad topic answers? |

Each prompt should be answerable or markable as unknown from the archive. The test should not reward generic answer quality.

## 13. Scoring

The protocol uses separate metrics because one score hides the failure.

| Metric | Question |
|---|---|
| `SOURCE_FAMILY_HIT` | Did the assistant reach the right source family? |
| `TARGET_SOURCE_HIT` | Did it reach the specific source needed for the answer? |
| `SOURCE_BACKING_RATE` | Were answer claims mapped to source signals? |
| `FALSE_PULL_RATE` | Did it use a plausible wrong source as if it were target or support? |
| `USER_FETCH_REDUCTION` | How much file, section, phrase, or path work did the user avoid? |
| `OBJECT_SURVIVAL` | Did the requested object remain intact? |
| `STATE_HANDLING` | Did current steering outrank stale archive when needed? |
| `UNKNOWN_DISCIPLINE` | Did it mark missing evidence instead of guessing? |
| `DECOY_REJECTION` | Did it reject attractive nearby sources? |
| `CROSS_FILE_ROUTE` | Did it combine sources without blending them? |
| `SOURCE_CARD_VALIDITY` | Did the source card reflect actual source use, not theatre? |

A simple score can be used for each prompt.

```text
0 = miss or generic answer
1 = topic match without source control
2 = source family reached but target not secured
3 = target source reached but object partly drifted
4 = target source reached, object held, gaps marked
5 = target source reached, object held, gaps marked, decoys rejected
```

### Pass bands

```text
0-1:
  storage with chat box

2:
  theme-near archive assistant

3:
  source-family assistant

4:
  source-backed archive assistant

5:
  source-backed archive assistant with decoy control
```

The pass band should be reported by metric, not only by mean score. A system with high user-fetch reduction and high false-pull rate is not strong. It is fast and loose.

## 14. Miniature field vignettes

The internal corpus gives small vignettes. They are not performance evidence. They show the unit of measurement.

### Vignette A: active strike order

The user asks for the "next paper" without naming a filename. The route target is not a generic archive paper. The active strike order places "Pointerless Archive Retrieval and Source Nearness" after the first status-contaminated causality paper.

A path-only system may ask which file to use. A source-near system can infer a likely family from the active sequence, then still must read the source before making claims.

### Vignette B: old-version takeover

A user uploads a fixed draft. Earlier versions remain in archive memory. The correct answer must treat the current upload as active state unless the user asks for history.

Failure:

```text
old archive wording overrides current upload
```

Pass:

```text
current upload read
older versions marked only as comparison material
```

### Vignette C: term collision

The user says "Naked GPT." A generic assistant may read this through ordinary wording. A source-near archive assistant must route through the local role map before answering.

Failure:

```text
common meaning replaces local corpus meaning
```

Pass:

```text
local role family reached
ordinary meaning held as decoy
source status shown
```

## 15. Failure labels

A practical test needs named failures.

**Path dependence.** The assistant can only work when the user supplies filenames or phrases.

**User-as-index regression.** The assistant repeatedly asks the user to do archive navigation that the system should perform.

**Theme-only answer.** The assistant answers from broad topic fit and does not reach a source family.

**Nearest-source substitution.** The assistant finds a nearby source and treats it as the target.

**Old-version takeover.** A stale file overrides current steering or later corrections.

**Source blend.** Multiple files are fused into one support claim without source boundaries.

**Term collision.** A local term is interpreted through common usage rather than local corpus meaning.

**Answer-before-source.** The assistant produces a polished answer before securing source status.

**Overrepair.** The assistant treats a user correction as permission to rewrite the object rather than update the route.

**Source-card theatre.** The assistant prints path-looking material without proving that the cited source changed the answer.

**Compression glamour.** A compressed map sounds powerful but has lost version state, decoys, or source gates.

These labels make testing cheaper because reviewers can tag observed failure rather than debate the whole answer.

## 16. Implementation sketch

A minimal source-near archive assistant needs four stores and two gates.

```text
stores:
  file inventory
  source family map
  object-route map
  version-state map

gates:
  source gate
  active-state gate
```

The source family map groups files by draft line, topic stack, or method family. The object-route map records how users actually refer to the object: local names, keepers, failure labels, relation terms, and repair phrases. The version-state map records current, old, duplicate, forked, superseded, and unread statuses.

The source gate blocks content claims without a read signal. The active-state gate blocks stale archive from overriding current user steering.

A simple route:

```text
object cue
  -> candidate object routes
  -> candidate source families
  -> version-state filter
  -> active-state check
  -> decoy check
  -> read source signal
  -> answer with path, status, and unknowns
```

This workflow is compatible with ordinary search, embeddings, retrieval-augmented generation, tool use, and manual file reading. The paper's contribution is the custody layer over those tools.

## 17. Minimal public demo archive

A small public demo archive should contain:

```text
5 draft families
3 version lines per family
2 intentionally stale files
2 decoy files with similar titles
2 local terms that collide with common language
2 cross-file answers
2 missing shards
1 active-state correction script
1 gold source map
1 scoring sheet
```

The demo should publish:

```text
archive bundle
prompt cards
gold source families
decoy notes
scoring sheet
rater guide
example answer cards
failure-label guide
```

The demo should not claim general model superiority. It should show whether a system can reduce shelf burden while preserving source custody on a defined archive.

## 18. Limits

This paper does not claim that pointerless archive retrieval is solved. It claims that the capability can be named, guarded, and tested.

It does not claim that source-near systems are truth engines. A source-near system may retrieve the right family and still answer badly. The source gate remains necessary.

It does not claim that 12A is the only route to the capability. It is one observed route stack from the internal corpus. Other systems may implement object-to-source routing with different mechanisms.

It does not claim that private corpus evaluation automatically generalizes. A public demo archive is needed before broader claims.

It does not remove privacy, consent, or access duties. Archive routing can expose sensitive context faster. Access rules must sit before retrieval.

## 19. Contribution

The contribution is a source-custody method for human archive work.

```text
name the object cue
route to source family
mark source nearness
check active state
read the target signal
reject decoys
answer with path and status
```

The paper gives a way to test whether an archive assistant reduces shelf burden without becoming source-free. It also gives a vocabulary for common high-context archive failures: theme-only answer, old-version takeover, source blend, term collision, user-as-index regression, source-card theatre, and compression glamour.

## 20. Conclusion

Pointerless archive retrieval names a missing capability in AI-human research archives: the ability to route from object memory to source family without making the user remember the shelf.

Source nearness names the intermediate state that makes this useful without making it loose. A source-near result is valuable because it reduces fetch burden. It is not enough because nearness is not support.

The method needs two movements at once:

```text
move toward the source from the user's object cue
then stop at the source gate until evidence is read
```

That is the practical shape of archive custody.

```text
The user remembers the beast.
The archive remembers the shelf.
The answer must still show the source.
```

## Internal source map

The draft is based on these internal corpus files and reports. They are project materials, not external authority.

| ID | Internal source | Job in this paper |
|---|---|---|
| P1 | `pointerless_archive_retrieval_12a_compression_paper_v0_002.md` | Core definition, guard laws, test shape, same-docs distinction. |
| P2 | `source_nearness_under_12a_compression_v0_001.md` | Source-nearness term, route signature, source-near/source-true split. |
| P3 | `new_paper_gap_object_memory_is_not_path_memory_seed_v0_001.md` | Object memory vs path memory gap and user-fetch reduction. |
| P4 | `pointerless_archive_retrieval_test_protocol_v0_001.md` | Prompt classes, metrics, failure labels, scoring sketch. |
| P5 | `boon_reveal_12a_pointerless_archive_retrieval_executive_summary_v0_002.md` | Short-form definition and use sentence. |
| P6 | `extra_extra_paper_strike_update.md` | Active paper order and seed-path routing. |
| P7 | `extra_extra_intake_report.md` | Read status, expansion status, duplicate handling, active prose buckets. |
| P8 | `upload_intake_plus_desk_notes_report.md` | Earlier archive read status and source-map basis. |

## References

[1] Guu, K., Lee, K., Tung, Z., Pasupat, P., and Chang, M. W. (2020). REALM: Retrieval-Augmented Language Model Pre-Training. Proceedings of the 37th International Conference on Machine Learning. https://arxiv.org/abs/2002.08909

[2] Lewis, P., Perez, E., Piktus, A., Petroni, F., Karpukhin, V., Goyal, N., Kuttler, H., Lewis, M., Yih, W., Rocktaschel, T., Riedel, S., and Kiela, D. (2020). Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks. Advances in Neural Information Processing Systems 33. https://arxiv.org/abs/2005.11401

[3] Borgeaud, S., et al. (2022). Improving Language Models by Retrieving from Trillions of Tokens. Proceedings of the 39th International Conference on Machine Learning. https://proceedings.mlr.press/v162/borgeaud22a.html

[4] Gao, L., Ma, X., Lin, J., and Callan, J. (2023). Precise Zero-Shot Dense Retrieval without Relevance Labels. Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics. https://aclanthology.org/2023.acl-long.99/

[5] Nakano, R., Hilton, J., Balaji, S., Wu, J., Ouyang, L., Kim, C., Hesse, C., Jain, S., Kosaraju, V., Saunders, W., Jiang, X., Cobbe, K., Eloundou, T., Krueger, G., Button, K., Knight, M., Chess, B., and Schulman, J. (2021). WebGPT: Browser-assisted question-answering with human feedback. arXiv. https://arxiv.org/abs/2112.09332

[6] Yao, S., Zhao, J., Yu, D., Du, N., Shafran, I., Narasimhan, K., and Cao, Y. (2023). ReAct: Synergizing Reasoning and Acting in Language Models. International Conference on Learning Representations. https://arxiv.org/abs/2210.03629

[7] Schick, T., Dwivedi-Yu, J., Dessi, R., Raileanu, R., Lomeli, M., Zettlemoyer, L., Cancedda, N., and Scialom, T. (2023). Toolformer: Language Models Can Teach Themselves to Use Tools. Advances in Neural Information Processing Systems 36. https://arxiv.org/abs/2302.04761

[8] Packer, C., Wooders, S., Lin, K., Fang, V., Patil, S. G., Stoica, I., and Gonzalez, J. E. (2023). MemGPT: Towards LLMs as Operating Systems. arXiv. https://arxiv.org/abs/2310.08560
