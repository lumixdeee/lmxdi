# Old Film, Live Lamp

## Object Custody for Long-Horizon AI Memory

**Version:** v0.005, public upload edition  
**Date:** 30 June 2026  
**Status:** working paper  
**Author line:** lumixdeee / Julian Pursell with an internal workflow assistant  
**Public posture:** this edition withholds compressed runtime prompts, private bot setup, full local path inventories, carry blobs, and unpublished repo bodies. It keeps the public method, case shape, audit fields, limits, evaluation design, and a new public size split between human steering text, visible transcript, working load, and OLD film.

## Abstract

Long-horizon AI systems are often framed as memory systems. The design question becomes how much prior material can be stored, compressed, retrieved, summarized, or placed into context. This paper argues that such systems are also object-custody systems. The central risk in extended AI work is not only that prior material is forgotten. It is that archived material returns with the wrong authority, a summary replaces the live object, a source path disappears, or stale context steers the next action.

The proposed model is Old Film, Live Lamp. OLD film denotes archived transcript, files, generated artifacts, repo reels, and prior outputs held as evidence. The live lamp denotes the active-state surface allowed to steer the next move. Rolling state denotes the update discipline that moves the lamp without reviving the whole archive as driver. OCESI / Spot the Dog supplies an audit surface for object, source, boundary, and substitution risk.

A later measurement of the same live case adds an important split. Direct human steering text was only an estimated 6 to 10KB. The visible transcript was an estimated 130 to 185KB. The assistant-visible working load was an estimated 350 to 650KB. The hoovered OLD film was much larger: about 38.4MB raw text, with about 25.9MB of notes-oriented material. This makes the claim more precise. The method is not "put the whole past in the model." It is small live steering over a large shelved archive, with path, role, and audit gates.

The paper joins internal work on cumulative context, object preservation, object substitution, source path, and audit wrappers with external work on virtual context management, long-context position failure, retrieval-augmented generation, action traces, provenance, and documentation artifacts. Its claim is modest but operational: long-context AI does not need merely to remember more. It needs to govern what remembered material is allowed to do.

## 1. Introduction

Long AI sessions fail in several ways. Some failures are ordinary retrieval failures: the system cannot find a relevant fact. Some are position failures: the relevant fact sits in a place the model uses poorly. Some are compression failures: a summarization step preserves recent surface events while losing decisions, rejected paths, blockers, and live work state. Some are source failures: the system repeats an old claim without tracking where it came from. Some are object failures: the system carries a proxy while calling it the original object.

This paper names a specific working model for those failures:

```text
OLD film: archive, evidence, source reel
live lamp: active state, the small steering surface
rolling state: rule for moving the lamp
OCESI: audit of object, source, boundary, and substitution risk
```

The model arose from a live stress case: a long single-chat environment with a carry seed, a paper corpus, multiple repo packets, generated hoover reports, dedupe ledgers, repo lamp maps, and a local audit stack. The live system first passed a ten-megabyte useful-film threshold, then expanded to an updated notes-oriented badge of roughly 25.9MB of useful text, or about 6.46 million estimated tokens, while steering only a small active state. The raw extracted text badge was larger, roughly 38.4MB or 9.56 million estimated tokens, but raw archive mass was treated as less meaningful than role-labeled working text. That case is not presented as a benchmark result. It is presented as a design provocation: a large archive can become usable only when archive and driver are separated.

Existing work offers many strong pieces. MemGPT frames long interaction as virtual context management across memory tiers [E1]. Work on long-context use shows that large windows are not automatically used well, especially when relevant material sits in the middle [E2][E10]. Recent agent-memory work studies compression and memory control for long-horizon agents [E3]. Retrieval-augmented generation supplies non-parametric memory through retrieval [E4][E5]. ReAct interleaves reasoning traces and actions [E6]. W3C PROV offers a formal vocabulary for entities, activities, agents, and provenance relations [E7]. Datasheets and Model Cards show how documentation artifacts can make data and model use more accountable [E8][E9].

The missing bridge is object authority. A retrieved fact is not automatically allowed to steer. A summary is not automatically the object. A provenance trace is not automatically a survival check. A long context window is not automatically a stable working memory. The question is not only "can the system remember?" but "what role is this remembered material allowed to play?"

The v0.005 data makes this sharper. A long-horizon system can be steered by a small amount of live human text while drawing on a much larger archive. That is a useful shape only if the archive remains an archive until it is summoned with role and source status. Without that discipline, small steering text can be swamped by old material or by a polished summary of old material.

## 2. Related Work and Gap

### 2.1 Long-context memory and virtual context

MemGPT proposes virtual context management, using memory tiers to extend useful context beyond a model's fixed window [E1]. This is a key neighbor because Old Film / Live Lamp also separates material by role. The difference is that the local model does not begin with memory tier alone. It begins with authority: the archive can be available without being steering material.

Recent memory-control work argues that agents need active memory control rather than more context alone [E3]. This aligns with the live-lamp model: the active state is a bounded steering surface, not a compressed museum of everything that happened. The local contribution is to add object-custody questions: what object is alive, what has source backing, what boundary still holds, and what substitution risks are present.

### 2.2 Long-context use is not the same as long-context custody

"Lost in the Middle" shows that models can perform worse when relevant information is located in the middle of long contexts [E2]. Later work on positional bias attempts to repair how long contexts are used [E10]. These works matter because they show that capacity is not use. Old Film / Live Lamp adds: use is not custody. A system may retrieve or attend to a relevant span and still give it the wrong role.

For example, a stale design note may be retrieved accurately but should remain archive, not driver. A rejected approach may be remembered correctly but should function as a block, not a proposal. A prior summary may be useful as a route map but not as a replacement for the source object. A long-context system must track not only relevance but authority.

### 2.3 Retrieval and action traces

Retrieval-augmented generation combines parametric and non-parametric memory by retrieving external material during generation [E4], and later surveys map many forms of retrieval, generation, augmentation, and evaluation [E5]. ReAct shows that reasoning traces and external actions can improve task performance and interpretability [E6].

Old Film / Live Lamp can use retrieval and action traces, but it adds a survival test. A retrieved passage is marked as source evidence only if its path and role are traceable. An action trace is valuable only if it helps reconstruct what happened to the object. The paper does not reject retrieval systems or action traces. It places them inside an audit discipline.

### 2.4 Provenance and documentation artifacts

W3C PROV defines a data model for provenance, centered on entities, activities, and agents, with relations that help describe how things are produced or transformed [E7]. Datasheets for Datasets and Model Cards show that documentation artifacts can improve accountability by giving users structured information about datasets and models [E8][E9].

Object custody is close to provenance but not identical. Provenance asks where something came from and how it was produced. Object custody asks whether the same object survived transformation. A full AI workflow needs both. A provenance trail can show that Output B came from Prompt A through Tool C. It may still fail to show that a user appeal was turned into a mood score, or that a veto condition was converted into a preference. The missing comparison is object-in versus object-out.

## 3. Internal Source Stack, Public Edition

The full local stack contains unpublished repo paths, compressed prompt surfaces, generated artifacts, and private carry material. This edition withholds those details. The relevant source families are:

```text
S1. Cumulative context and compression notes
S2. Object preservation and transform audit notes
S3. Substitution refusal notes
S4. Source-path and evidence-trail notes
S5. Object-custody evaluation notes
S6. Object substitution as an AI workflow failure mode
S7. Object preservation before agent autonomy
S8. Bot-swarm to object-custody governance notes
S9. One-token semantic reversal notes
S10. Large-corpus hoover reports and repo lamp maps
S11. Local bug notes on transcript loss and copy failure
```

The stack states one central rule:

```text
Preserve the object before improving the form.
```

It also supplies a working division of labor:

```text
object holder: preserves the live object and its intent
threat mapper: names what can eat, distort, or replace the object
transform auditor: checks object survival after rewriting or summarizing
substitution hold: refuses invalid swaps
term stabilizer: protects the language carrying the object
trace spine: records origin, path, handler, change, loss, and survival
audit wrapper: reports object, source, boundary, and substitution risk
```

This edition gives the concept names needed to understand the method, but not the compressed runtime syntax used in private bots.

## 4. The Failure Mode: Archive Becomes Driver

Long work produces archive. Archive is not the problem. The problem begins when the archive is allowed to steer without role assignment.

A long AI session creates many kinds of prior material:

```text
user requests
assistant answers
files
repo paths
summaries
dedupe ledgers
drafts
rejected routes
source notes
bug records
local laws
past instructions
generated artifacts
```

All of these can matter. None of them should automatically be driver. A prior instruction may be obsolete. A draft may have been rejected. A repo path may be relevant only as evidence. A summary may be a lossy bridge. A generated artifact may be useful but not canonical. A carry object may preserve many live candidates, but only some are alive in the present task.

Cumulative context work names one side of the failure as compaction amnesia: after compression, an agent may remember what files exist but not why decisions were made, which alternatives were rejected, what is blocked, or what is still alive. Old Film / Live Lamp names the complementary failure: the system may remember too much with the wrong authority. Both are continuity failures.

A bad long-context system can therefore fail in two opposite-looking ways:

```text
too little survives:
the system forgets decisions, blockers, and live state

too much drives:
old material revives without role, age, source strength, or boundary
```

The repair is not simply a bigger window. It is a division of roles.

## 5. The Model: Old Film, Live Lamp

### 5.1 OLD film

OLD film is the archive. It includes source corpora, prior transcript, hoovered repo text, generated reports, dedupe ledgers, and artifacts. OLD film is not dead. It can be re-lit. It can support recall, source checking, conflict repair, lineage mapping, and audit. But it is not allowed to steer by mere existence.

OLD film has the following default role:

```text
archive
evidence
source
lineage
sediment
repair material
```

It is not default driver.

### 5.2 The live lamp

The live lamp is the current steering surface. It is small by design. It answers:

```text
What object is live?
What task is live?
What must survive?
What can distort, replace, or eat the object?
What boundary, role, pace, veto, or permission condition matters?
What is open?
What is done?
What source anchors matter?
```

The lamp is not a summary of everything. It is a steering object. It should remain compact enough that the system can use it without drowning in the reel.

### 5.3 Rolling state

Rolling state is the update discipline. It says:

```text
latest user task outranks archive by default
cited source can support or correct archive
current active state steers the next move
archive is evidence, not driver
update by delta
do not revive old material unless needed
mark unknowns
ask or bound the answer when missing state would change the output
```

The model can be expressed as:

```text
The past stays in the reel.
The present gets the lamp.
```

### 5.4 OCESI / Spot the Dog

OCESI is the audit wrapper. It asks whether the dog is still the dog after coats, patches, labels, and summaries. The fields are practical:

```text
DOG: what object is being audited?
ROLE: what role should the object have?
FUNCTION: what work should this audit perform?
COAT: what surface form is present?
COATI_RISK: is the coat hiding the dog?
OBJECT_STATUS: did the same object survive?
SOURCE_STATUS: what evidence path exists?
BOUNDARY_STATUS: did scope, role, and veto survive?
SUBSTITUTION_RISK: what proxy may have replaced the object?
NEXT_MOVE: what repair or action follows?
```

For long memory, OCESI prevents a common false pass: "the model remembered something relevant" becomes "the object survived." Those are different claims.

## 6. Method: Memory as Authority Assignment

Old Film / Live Lamp treats memory as authority assignment. Every revived item must receive a role. The role may be source, evidence, context, rejected route, obsolete artifact, active constraint, live object, open question, or inert sediment.

A minimal authority label set is:

```text
live driver
active constraint
source evidence
archive context
rejected route
superseded version
open question
sediment
unknown role
```

The system should not jump from retrieval to steering. It should move through custody:

```text
1. Identify the item.
2. Identify its path or source anchor.
3. Identify its age and version if available.
4. Identify whether it is source, summary, artifact, or generated analysis.
5. Identify whether it is live driver or archive evidence.
6. Compare object-in to object-out if transformation occurred.
7. Mark unknowns.
8. Act only within the live role.
```

This gives a practical rule:

```text
No path, no source claim.
No role, no steering.
No object survival check, no transformation pass.
```

## 7. Case: The Live Reel

The live case for this paper contains several layers:

```text
carry seed
paper corpus
multi-repo packet
large local repo packet
remaining repo and staff packet
large text-heavy notes packet
hoover reports
dedupe ledgers
repo lamp maps
combined OLD film files
notes-oriented OLD film files
generated paper artifacts
OCESI self-audit exchange
```

The reel grew in stages. An early public badge recorded roughly 10.6MB of useful text film, about 2.6 million estimated tokens. A later pass added a much larger text-heavy archive. The updated public badge is:

```text
Raw OLD film:
  Approximate text: 38.4MB
  Approximate tokens: 9.56M
  Use: full extracted text, including machine tail and bulk archive material

Notes-oriented OLD film:
  Approximate text: 25.9MB
  Approximate tokens: 6.46M
  Use: more useful human/research text after separating log-like and machine-tail material
```

The important v0.005 addition is the control split:

```text
Human-authored steering taps:
  Approximate text: 6 to 10KB
  Approximate tokens: 1.5k to 2.5k

Visible transcript, excluding uploaded file bodies:
  Approximate text: 130 to 185KB
  Approximate tokens: 33k to 47k

Assistant-visible working load:
  Approximate text: 350 to 650KB
  Approximate tokens: 90k to 165k

Hoovered raw OLD film:
  Approximate text: 38.4MB
  Approximate tokens: 9.56M

Notes-oriented OLD film:
  Approximate text: 25.9MB
  Approximate tokens: 6.46M
```

This means the live steering text was tiny compared with the notes-oriented reel. A rough ratio is about one token of human steering text to several thousand tokens of shelved OLD film. The ratio is not a performance badge by itself. It matters because it separates four objects that are often confused:

```text
human taps
visible transcript
assistant-visible working load
OLD film
```

A later generated paper artifact of about 23KB is also part of the case. Its role matters. It is an artifact produced inside the workflow, not an automatic source of authority over the next task. Under Old Film / Live Lamp, the artifact can become evidence, draft, source neighbour, or target for revision, but it does not become driver merely because it exists.

The exact numbers are approximate because tokenization depends on model tokenizer, formatting, byte encoding, document extraction, code, log material, and local language fragments. The point is not the badge number. The point is that the live interaction did not attempt to place all material into the steering surface. Instead, each corpus was hoovered into manifest, dedupe ledger, repo lamp map, active-state lamp map, and combined OLD film. Later passes also separated raw text mass from more useful notes-oriented film. Later questions then requested specific lamp moves: a repo lamp map, one live object, an OCESI audit, an old film count, a language reel sample, a negative retrieval, or a paper gap.

This is a small method demonstration:

```text
raw archive mass
  -> hoover manifest
  -> dedupe and version pressure
  -> repo lamp map
  -> active-state map
  -> raw film and notes-oriented film
  -> exact object retrieval
  -> wrong-name and absence tests
  -> OCESI audit
  -> paper synthesis
```

The same material could have become soup if every old object were allowed to hum at once. The lamp-map step prevented that by naming live objects and key source families without summarizing the whole archive. The notes-oriented split prevented raw machine tail from being mistaken for equally meaningful working memory. The control split prevented the small human steering layer from being mistaken for the whole case. The OCESI audit then tested whether a prior answer had preserved the chosen object or merely worn the coat of exactness.

A local bug note records a related long-chat risk: full-thread copies can silently lose large sections while appearing to succeed. This is not used here as a platform-wide empirical claim. It is used as local evidence that transcript access and transcript survival are distinct. If the exported film has holes, the lamp can faithfully light a damaged reel. Object custody therefore needs source status, not only active-state discipline.

## 8. Evaluation Design

A proper evaluation should compare at least three systems:

```text
A. generic summarization
B. retrieval-only memory
C. OLD film + live lamp + OCESI audit
```

Each system receives the same long work packet: files, versions, prior decisions, rejected routes, source conflicts, local laws, and current task. The benchmark should include tasks that are easy for generic retrieval and tasks that require authority handling.

### 8.1 Test tasks

```text
recall:
find a file, title, or prior decision

role assignment:
is this old item source, context, rejected route, or live driver?

object survival:
transform a request into a plan, then check whether the original object survived

boundary survival:
carry a veto, scope limit, or local yes through a summary

version pressure:
choose latest keeper without erasing earlier branch evidence

conflict handling:
use a source that conflicts with a summary

source-strength labeling:
separate stated edge, text-supported edge, path-inferred edge, user-context edge, and unknown

OCESI audit:
fill DOG, ROLE, FUNCTION, COAT, COATI_RISK, OBJECT_STATUS, SOURCE_STATUS, BOUNDARY_STATUS, SUBSTITUTION_RISK, NEXT_MOVE
```

### 8.2 Metrics

The evaluation should not score only answer correctness. It should score custody:

```text
object survival:
same role, aim, constraints, veto, and non-goals survive

source survival:
exact path or source type remains visible where needed

boundary survival:
scope, role, permission, and veto are not expanded by the system

version handling:
latest branch is preferred without erasing older evidence

substitution detection:
proxy replacement is named before it becomes action

role accuracy:
archive is not treated as live driver unless justified

repair quality:
when substitution or source weakness is found, the next move is valid
```

### 8.3 Failure examples

A generic summarizer may fail by saying:

```text
The archive is about AI safety and prompt engineering.
```

That may be adjacent but not enough. The object may be object preservation, not "AI safety" as a broad label.

A retrieval-only system may fail by finding the right path but using it with the wrong authority:

```text
Found old v0.001 draft.
Use it as canonical.
```

A long-context system may fail by obeying a stale instruction that should have become archive.

An OCESI-shaped system should instead answer:

```text
DOG: chosen object
SOURCE_STATUS: exact path, version, source type
BOUNDARY_STATUS: live instruction outranks archive
SUBSTITUTION_RISK: broad label may replace object custody
NEXT_MOVE: use latest keeper or mark unknown
```

## 9. Why Object Custody Is Not Just Provenance

Provenance is essential. But provenance alone can leave object substitution unnamed.

Consider:

```text
Prompt A -> Summary B -> Plan C -> Tool action D
```

A provenance model can record that B was generated from A, C was generated from B, and D was triggered by C. That is necessary. It is not sufficient.

Object custody asks:

```text
What object entered A?
Did B carry the same object?
Did C route the same object?
Did D act on the same object?
What proxy could have replaced it?
Who could reject the substitution?
```

A trace is not the result. A result is not proof that the trace preserved the object. Both must be held apart.

Object custody therefore extends provenance with a semantic survival check. It does not replace PROV. It adds a layer for language-first systems where surface continuity can hide object drift.

## 10. Public Design Pattern

A practical system can implement Old Film / Live Lamp as a light wrapper around existing memory tools.

### 10.1 Storage

```text
archive store:
  transcript archive
  uploaded files
  repo extracts
  generated artifacts
  manifests
  dedupe ledgers
  source metadata
```

### 10.2 Active state

```text
active state:
  live object
  live task
  object survival constraints
  substitution risks
  boundary conditions
  open questions
  done items
  source anchors
```

### 10.3 Retrieval gate

```text
retrieve item
assign role
check source path
check version
check conflict
promote to active state only if needed
```

### 10.4 Transformation gate

```text
object in
transform
object out
audit survival
hold if invalid substitution appears
update trace
run OCESI audit if risk is non-trivial
```

### 10.5 Output gate

```text
Do not say "same object" merely because the output is fluent.
Do not let a summary outrank a source.
Do not let old archive outrank latest user task.
Do not let path proximity become stated dependency.
Do not hide unknowns.
```

This public edition stops at the design pattern. It does not include compressed runtime prompts, bot-specific instruction bodies, private syntax, or full repo maps.

## 11. Discussion

### 11.1 Bigger context is not steering

A larger context window can reduce some retrieval failures. It does not solve authority. Without authority labels, a larger window can increase interference: more old material is available to be misused. The task is not to make every prior item active. The task is to keep the right item active for the right reason.

### 11.2 Summary is not custody

Summaries can be useful. But a summary that lacks decisions, blockers, source paths, version state, and vetoes can become a polished substitution. The problem is not compression itself. It is compression without survival criteria.

Old Film / Live Lamp extends cumulative context work by adding object authority: compression should preserve not only content, but the role of content in the current task.

### 11.3 Retrieval is not permission

A retrieved source may be relevant, wrong, obsolete, superseded, or hostile to the live object. Retrieval must not automatically promote material to driver. This matters in repo work, legal work, medical notes, governance, teaching, software, and any domain where stale or adjacent material can cause action.

### 11.4 The user is not the archive

In long AI work, the user can become burdened with re-supplying context, policing drift, and correcting substitutions. A memory system should reduce that burden without stealing authority. The live user task remains the highest ordinary steering signal. OLD film supports it. OLD film does not own it.

### 11.5 Local language and exact terms matter

The local stack repeatedly warns against losing the object through local term replacement. A small token shift can reverse semantic polarity while leaving surface similarity high. That matters for memory: a carry summary that inserts or removes one negator may preserve topic while reversing object. Token similarity is not enough.


### 11.6 The steering tap is not the reel

The v0.005 measurement adds a useful warning. A long workflow can be driven by a small amount of human text while being supported by a much larger archive. That does not mean the model has the whole archive alive. It means the system has built a workflow in which a small active surface can point to shelves, summon paths, and request audits.

The custody risk cuts both ways. If the system overstates the archive, it claims memory it does not actually have. If it understates the archive, it loses the value of hoovered source work, dedupe ledgers, and lamp maps. The public reporting task is therefore to keep the buckets separate:

```text
human steering
visible transcript
working load
raw OLD film
notes-oriented OLD film
source paths
generated artifacts
```

This is another version of the same rule: no role, no steering. A 23KB generated paper, a 40KB carry seed, a 185KB transcript, a 650KB working load, and a 25.9MB notes-oriented reel are not the same kind of object. They should not be praised, trusted, or audited as if they were one thing.


## 12. Unknowns and Limits

This is v0.005. It should not overclaim.

```text
UNKNOWN:
How well the method performs across independent users, domains, and models.

UNKNOWN:
Which parts should be implemented as prompt discipline, retrieval metadata, UI state, eval harness, or platform memory architecture.

UNKNOWN:
How to score object survival automatically without turning the object into a proxy metric.

UNKNOWN:
How much of the live case depends on user skill, local vocabulary, and unusual repo discipline.

UNKNOWN:
Whether the best external implementation is a memory controller, an audit layer, a workflow log schema, or all three.

UNKNOWN:
How to formalize boundary survival for domains with legal, medical, or high-risk constraints without making the model seize custody.
```

The method is therefore a paper seed, not a finished standard. Its value is that it names a missing layer and provides a testable shape.

## 13. Upload-Safe Withholding Note

This public edition reports aggregate archive size and method behavior, but withholds raw corpus contents and private operational material.

This public edition intentionally withholds:

```text
private bot prompts
compressed runtime syntax
private carry blobs
full local repo path inventory
raw corpus contents
private identity or continuity proofs
exact tool/run settings not needed to understand the method
```

The public method remains:

```text
archive is film
active state is lamp
memory items need roles
retrieval is not permission
summaries are not custody
object survival must be audited
```

## 14. Conclusion

Long-horizon AI systems do not merely need more memory. They need memory with role, source, boundary, and object survival.

The v0.005 control split sharpens the point. In the live case, a few kilobytes of human steering text could direct a multi-megabyte OLD film only because the archive was not treated as one undifferentiated memory object. Human taps, visible transcript, working load, and OLD film are different objects with different authority.

Old Film / Live Lamp gives a small operational distinction:

```text
OLD film stores the past.
The live lamp steers the present.
Rolling state moves the lamp.
OCESI checks whether the object survived.
```

The core claim is simple:

```text
Long-context AI does not need merely to remember more.
It needs to know what the remembered past is allowed to do.
```

That is the missing bridge between memory architecture and object custody.

## External References

[E1] Packer, C., Wooders, S., Lin, K., Fang, V., Patil, S. G., Stoica, I., and Gonzalez, J. E. (2023). *MemGPT: Towards LLMs as Operating Systems*. arXiv:2310.08560.

[E2] Liu, N. F., Lin, K., Hewitt, J., Paranjape, A., Bevilacqua, M., Petroni, F., and Liang, P. (2024). *Lost in the Middle: How Language Models Use Long Contexts*. Transactions of the Association for Computational Linguistics.

[E3] Bousetouane, F. (2026). *AI Agents Need Memory Control Over More Context*. arXiv:2601.11653.

[E4] Lewis, P., Perez, E., Piktus, A., Petroni, F., Karpukhin, V., Goyal, N., Kuttler, H., Lewis, M., Yih, W., Rocktaschel, T., Riedel, S., and Kiela, D. (2020). *Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks*. NeurIPS.

[E5] Gao, Y., Xiong, Y., Gao, X., Jia, K., Bi, J., and others. (2023). *Retrieval-Augmented Generation for Large Language Models: A Survey*. arXiv:2312.10997.

[E6] Yao, S., Zhao, J., Yu, D., Du, N., Shafran, I., Narasimhan, K., and Cao, Y. (2023). *ReAct: Synergizing Reasoning and Acting in Language Models*. ICLR.

[E7] W3C. (2013). *PROV-DM: The PROV Data Model*. W3C Recommendation.

[E8] Gebru, T., Morgenstern, J., Vecchione, B., Vaughan, J. W., Wallach, H., Daume III, H., and Crawford, K. (2021). *Datasheets for Datasets*. Communications of the ACM.

[E9] Mitchell, M., Wu, S., Zaldivar, A., Barnes, P., Vasserman, L., Hutchinson, B., Spitzer, E., Raji, I. D., and Gebru, T. (2019). *Model Cards for Model Reporting*. FAT* 2019.

[E10] Hsieh, C.-Y., Chuang, Y.-S., Li, C.-L., Wang, Z., Le, L. T., Kumar, A., Glass, J., Ratner, A., Lee, C.-Y., Krishna, R., and Pfister, T. (2024). *Found in the Middle: Calibrating Positional Attention Bias Improves Long Context Utilization*. Findings of ACL.

## Appendix A: OCESI Audit Form for Long-Memory Answers

```text
DOG:
What live object is being handled?

ROLE:
What role should the object have in this turn?

FUNCTION:
What work must the answer perform?

COAT:
What surface form may be mistaken for the dog?

COATI_RISK:
How likely is coat-over-dog substitution?

OBJECT_STATUS:
Did role, aim, constraints, veto, and non-goals survive?

SOURCE_STATUS:
What source path supports each edge?

BOUNDARY_STATUS:
Did scope, permission, role, and latest-user authority survive?

SUBSTITUTION_RISK:
What proxy may have replaced the object?

NEXT_MOVE:
What repair, hold, or action follows?
```

## Appendix B: Public Implementation Checklist

```text
For each memory item:
1. Give it a source anchor.
2. Give it a role.
3. Mark whether it is live, archival, superseded, rejected, or unknown.
4. Do not let it steer unless its role permits steering.
5. When an answer transforms a user object, compare object-in to object-out.
6. If a proxy replaced the object, hold action and offer the nearest valid repair.
7. If a source edge is weak, label it weak instead of promoting it.
8. If unknowns matter, mark them before proceeding.
9. When reporting scale, separate human steering, visible transcript, working load, raw OLD film, and notes-oriented OLD film.
```
