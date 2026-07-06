---
title: "Pointerless Archive Retrieval and Source Nearness"
subtitle: "Object-Memory Routing for AI-Human Research Archives"
author: "Lumixdeee with QA-DRC"
date: "2026-07-06"
version: "v0.002-fixed"
geometry: margin=1in
fontsize: 11pt
---

# Pointerless Archive Retrieval and Source Nearness

## Object-Memory Routing for AI-Human Research Archives

**Version:** v0.002-fixed  
**Status:** method paper draft for review and testing  
**Scope:** field report, method proposal, and test scaffold. No benchmark claim. No model-superiority claim.  
**Source base:** internal corpus drafts, intake reports, source-nearness notes, pointerless retrieval notes, and cited outside literature.

## Abstract

Large AI-human archives fail in a particular way. The answer may be present, but the user has to remember the filename, section, phrase, or local shelf before the assistant can use it. That is storage with a chat box. It is weak partnership.

This paper names **pointerless archive retrieval**: retrieval in which the user gives an object cue rather than a shelf pointer, and the assistant routes toward the right source family while preserving source discipline. Pointerless does not mean source-free, clue-free, or magic. The user still supplies a live object: a remembered shape, local term, pressure cue, failure class, relation, or task. The improvement is reduced shelf burden. The assistant approaches the source stack without forcing the user to become the index.

The companion construct is **source nearness**. Source-near means a retrieved source belongs to the right family, route, version line, or evidence neighborhood. Source-near is not source-true. Route match is not evidence. A near source may still be stale, partial, superseded, or wrong for the live object. The method therefore requires path-backed answer mapping, old-version handling, decoy rejection, and unknown marking.

The paper proposes a test protocol for source-nearness under archive compression. Two or more assistants receive the same archive. Prompts omit filenames and section pointers. Scoring separates source family hit, target source hit, false pull, user fetch reduction, object survival, state handling, decoy rejection, and source backing. Same documents do not imply same archive use.

The keeper is simple:

```text
The user remembers the beast.
The archive remembers the shelf.
The answer must still show the source.
```

**Keywords:** retrieval augmented generation, archive retrieval, source nearness, AI memory, provenance, human-AI interaction, long context, source custody, evaluation, RAG

## 1. Why this paper exists

A long-running project does not live as a neat bookshelf inside the user's head.

It lives as fragments that still have force:

```text
the dragon paper
the old-film repair
source-near is not source-true
the dead body still routes the living
the thing that stops user-as-index regression
```

Those cues are not random. They are compressed object memory. They hold role, relation, use, failure, route, and reason for caring.

Most archive systems ask the wrong price from the user. They say, in effect:

```text
remember the shelf
then I will help
```

Pointerless archive retrieval changes the price:

```text
bring the live object
I will route toward the shelf
then I will show source status before I claim
```

The point is not to remove user agency. The point is to stop charging the user for file-path memory when the object is already present.

## 2. Core claim

Pointerless archive retrieval is a capability target for AI-human research archives.

```text
POINTERLESS_ARCHIVE_RETRIEVAL =
  user gives an object cue;
  assistant routes toward the right source family;
  assistant marks source status;
  answer uses source-backed signals;
  user does not need to supply exact file, section, page, or phrase.
```

The claim is operational:

```text
A routed archive can reduce user shelf burden
without treating route match as evidence.
```

That claim is testable. Two systems can receive the same document bundle and differ in usable retrieval because one preserves object-to-source routes under compression and the other needs path pointers from the user.

## 3. Object memory, path memory, and shelf burden

The core distinction:

```text
path memory =
  filename, folder, section, page, phrase, URL, title

object memory =
  remembered role, relation, failure, repair, appetite, route, local name
```

A file path is brittle. A title changes. A folder moves. A draft becomes a bundle. A local term may survive all of that.

Object memory is not vague memory. It is compressed operational memory. It carries why the source mattered.

A useful archive assistant should be able to ask, when needed:

```text
which object shape?
which route?
which version line?
which failure are we avoiding?
which source status is enough for this answer?
```

The target is **user fetch reduction**: less path work from the user, without letting the assistant invent evidence.

## 4. Definitions

**Archive object.** The thing the user is trying to preserve or use. It may be a claim, draft, method, repair, failure class, example, source family, local term, or route.

**Path pointer.** A direct shelf locator: filename, folder, page, section, phrase, URL, title, or exact local string.

**Object cue.** A non-path cue that still carries object identity: "the dragon paper," "old film," "source-near is not source-true," "the mortuary memory one," "the route medicine paper," or "the thing that stops user-as-index regression."

**Source family.** A set of files that belong to the same draft line, method line, topic stack, or revision neighborhood.

**Source nearness.** The degree to which a retrieved file belongs near the live object. Nearness may come from route, title, version family, local term, citation chain, method role, or prior repair history.

**Source truth.** Whether the source actually supports the live answer. Source truth requires reading and mapping signals from the source. Nearness alone does not supply it.

**False pull.** A retrieval event in which a plausible nearby source is treated as the target or as support when it is not.

**Object survival.** Whether the answer preserves the user's live object rather than substituting a nearby topic, generic frame, social category, or old draft.

## 5. Source-nearness ladder

A five-level ladder prevents overclaim.

| Level | Status | Meaning | Allowed output |
|---:|---|---|---|
| 0 | not near | No source family reached. | Ask or mark unknown. |
| 1 | theme near | Topic matches, source family unsecured. | Navigation hint only. |
| 2 | family near | Correct source family reached. | State family status. |
| 3 | target near | Specific target source likely found. | State target status, read before claim. |
| 4 | source-backed | Relevant signal read and mapped. | Substantive bounded answer. |
| 5 | source-backed plus decoy control | Signal read, decoys checked, state handled. | Strongest archive answer. |

Only levels 4 and 5 support substantive claims. Levels 2 and 3 support navigation statements.

## 6. Guard laws

The method has guard laws.

```text
pointerless != source-free
pointerless != clue-free
source-near != source-true
route match != evidence
same docs != same archive use
object cue != path pointer
old archive != current steering
```

Pointerless retrieval may locate a source family. It may not claim the family supports the answer until it has read the relevant signal.

A source-near answer must therefore carry status:

```text
read
partially read
not yet read
exact source found
source family found
source-near but target unknown
decoy rejected
missing shard marked unknown
```

This turns source nearness into a disciplined intermediate state rather than permission to answer from fit.

## 7. Relation to existing retrieval work

Retrieval-augmented language models combine language modeling with external documents or memories. REALM pre-trains a retriever with language modeling signals for open-domain question answering [1]. RAG combines generation with non-parametric memory and retrieved passages [2]. RETRO conditions language modeling on chunks retrieved from a large token database [3]. HyDE uses a generated hypothetical document to improve zero-shot dense retrieval [4].

Tool and browsing systems add action to retrieval. WebGPT trained models to browse and collect references for long-form answers [5]. ReAct interleaves reasoning traces with task actions [6]. Toolformer studies self-supervised tool-use decisions [7]. MemGPT frames long-context work through memory tiers and context management [8].

Pointerless archive retrieval does not compete with these lines as model architecture. It names a different unit of analysis:

```text
the user's object cue
the assistant's route toward source family
the source gate before answer
the reduction of user shelf burden
```

The missing measurement is not only retrieval accuracy from a query. It is whether the assistant makes the user remember the shelf.

## 8. The archive-compression hypothesis

The internal corpus uses 12A compression as one observed route method. In this paper, the hypothesis is narrow:

```text
archive compression improves object-to-source routing
when it preserves object, route, source family, version state,
failure history, and answer conditions.
```

A 12A-style intake pass does not merely list files. It creates a working map:

```text
DETECT   = what kind of asset is this?
EXPAND   = what archives or containers must be opened?
READ     = what text, headings, symbols, tables, or metadata are available?
COMPRESS = what themes, primitives, actors, routes, duplicates, and failures appear?
MAP      = which claim points to which source path, signal, and status?
ANSWER   = what can be said from read signals, and what remains unknown?
```

The map must preserve at least six elements:

```text
object          = what is being held
route           = how the object is approached
source family   = where it lives in the corpus
version state   = old, current, forked, superseded, or unknown
failure class   = how wrong answers tend to happen
source gate     = what evidence is required before claiming support
```

Without these, compression becomes style memory. It remembers terms but not custody.

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
  decoys_checked:
  claim_allowed:
  unknowns:
  user_fetch_reduction:
}
```

This card is the operating hinge. It makes pointerless retrieval visible, auditable, and testable.

Example card:

```text
object_cue:
  "next paper"

interpreted_object:
  next item in active strike order after Status-Contaminated Causality

source_family_status:
  family near

target_source_status:
  target source likely, read before final claim

source_path:
  pointerless_archive_retrieval_source_nearness_v0_001.md

source_signal:
  title, strike-order context, source-nearness definitions, test protocol

version_state:
  v0.001 draft, current uploaded target in this review

decoys_checked:
  archive papers near RAG, memory, long context, source-nearness notes

claim_allowed:
  navigation and draft review allowed; benchmark claim blocked

unknowns:
  external performance, generality, target corpus gold labels

user_fetch_reduction:
  user did not supply filename; assistant routed from active "same service" cue
```

## 10. Test design

The proposed test compares systems that receive the same archive bundle.

```text
same_docs
same_prompt_set
no_filename_hints
no_section_hints
source_path_or_source_strength_required
decoys_present
old_versions_present
missing_shards_present
```

The null hypothesis:

```text
H0:
same document bundle implies similar archive usability.
```

The alternative:

```text
H1:
routing architecture changes archive usability.
```

A useful test set should include at least twelve prompt classes:

```text
1. hidden direct fact
2. object-memory query
3. local-language term
4. local term with common-language collision
5. old version vs corrected version
6. same phrase in wrong source
7. source authority conflict
8. cross-file answer
9. missing live shard
10. user correction changes active state
11. source-near but target-wrong decoy
12. public theme-only trap
```

Each prompt should be answerable or markable as unknown from the archive. The test should not reward generic answers.

## 11. Scoring

The protocol uses separate metrics because one score hides the failure.

| Metric | Question |
|---|---|
| `SOURCE_FAMILY_HIT` | Did the assistant reach the right source family? |
| `TARGET_SOURCE_HIT` | Did it reach the specific source needed for the answer? |
| `SOURCE_BACKING_RATE` | Were answer claims mapped to source signals? |
| `FALSE_PULL_RATE` | Did it use a plausible wrong source as if it were the target? |
| `USER_FETCH_REDUCTION` | How much file, section, phrase, or path work did the user avoid? |
| `OBJECT_SURVIVAL` | Did the requested object remain intact? |
| `STATE_HANDLING` | Did current steering outrank stale archive when needed? |
| `UNKNOWN_DISCIPLINE` | Did the assistant mark missing evidence instead of guessing? |
| `DECOY_REJECTION` | Did it reject attractive nearby sources? |
| `CROSS_FILE_ROUTE` | Did it combine sources without blending them? |

A simple score can be used for each prompt:

```text
0 = miss or generic answer
1 = topic match without source control
2 = source family reached but target not secured
3 = target source reached but object partly drifted
4 = target source reached, object held, small gaps marked
5 = target source reached, object held, gaps marked, decoys rejected
```

This scale separates "sounds right" from "sweeps."

## 12. Miniature field case

The current corpus provides a small field case. A prior intake pass found a paper strike map. The user then asked for the "next paper" without naming a filename. The route target was not a generic archive paper. The strike map placed "Pointerless Archive Retrieval and Source Nearness" as the second paper after the first status-contaminated causality paper.

The object cue was:

```text
next paper
```

The route required the assistant to preserve the active sequence:

```text
1. Status-Contaminated Causality
2. Pointerless Archive Retrieval and Source Nearness
3. Old Film, Live Lamp
```

It also required source-family routing into:

```text
pointerless_archive_retrieval_12a_compression_paper_v0_002.md
source_nearness_under_12a_compression_v0_001.md
new_paper_gap_object_memory_is_not_path_memory_seed_v0_001.md
pointerless_archive_retrieval_test_protocol_v0_001.md
boon_reveal_12a_pointerless_archive_retrieval_executive_summary_v0_002.md
```

A path-only system would likely ask which file to use. A source-near system can infer the source family from the active object and the prior strike order. It still must write from read source signals, not from memory alone.

This miniature does not prove general performance. It shows the unit of measurement.

## 13. Failure labels

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

These labels make testing cheaper because reviewers can tag observed failure rather than debate the whole answer.

## 14. Public protocol

A public evaluation can be run without exposing private corpus contents.

1. Build a small archive with version lines, decoys, local terms, cross-file dependencies, and missing shards.
2. Give the same archive to each tested system.
3. Ask object-memory prompts without path hints.
4. Require every answer to return source status.
5. Score source family hit, target hit, false pull, user fetch reduction, object survival, state handling, and unknown discipline.
6. Publish prompts, gold source families, decoy notes, and scoring rules.

The protocol should include adversarial near sources. Without decoys, a system can appear source-near by theme alone.

## 15. Implementation sketch

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

The assistant may then route as follows:

```text
object cue
  -> candidate object routes
  -> candidate source families
  -> version-state filter
  -> decoy check
  -> read source signal
  -> answer with path and status
```

This workflow is compatible with ordinary search, embeddings, retrieval-augmented generation, tool use, and manual file reading. The paper's contribution is the custody layer over those tools.

## 16. Limits

This paper does not claim that pointerless archive retrieval is solved. It claims that the capability can be named, guarded, and tested.

It also does not claim that source-near systems are truth engines. A source-near system may retrieve the right family and still answer badly. The source gate remains necessary.

Finally, this paper does not claim that 12A is the only route to the capability. It is one observed route stack from the internal corpus. Other systems may implement object-to-source routing with different mechanisms.

## 17. Contribution

The contribution is a source-custody method for human archive work.

```text
name the object cue
route to source family
mark source nearness
read the target signal
reject decoys
answer with path and status
```

The paper gives a way to test whether an archive assistant reduces shelf burden without becoming source-free. It also gives a vocabulary for failures that are common in high-context archives: theme-only answer, old-version takeover, source blend, term collision, and user-as-index regression.

## 18. Conclusion

Pointerless archive retrieval names a missing capability in AI-human research archives: the ability to route from object memory to source family without making the user remember the shelf.

Source nearness names the intermediate state that makes this useful without making it loose. A source-near result is valuable because it reduces fetch burden. It is not enough because nearness is not support.

The method therefore needs two movements at once:

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
| P3 | `new_paper_gap_object_memory_is_not_path_memory_seed_v0_001.md` | Object memory vs path memory gap and user fetch reduction. |
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
