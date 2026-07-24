# Shopping the Old Way vs Shopping the New Way

**Version:** v0.001  
**Date:** 23 July 2026  
**Status:** Pre-chat-ingest paper  
**Evidence route:** Working conversation memory, not the expanded SM

## Abstract

This paper compares two ways an assistant can shop for prompts inside a large private corpus.

The old way begins with the assistant's own sense of taste. It answers quickly, names prompt types it tends to like, and may only enter the corpus after the user objects. Even after entering the corpus, it can stop at the nearest glittering shelf and mistake a personal basket for a corpus-wide recommendation.

The new way begins with a retrieval gate. Any request about repositories, notes, uploads, paths, generated files, or the corpus must query the SM master first. Candidate prompts then travel through verified pointers, exact source fetches, collision checks, byte counts, and a stated shopping objective. The assistant does not crown the basket before contact. Provenance shows where an item came from. Testing decides what it is worth.

The central finding is simple: speed should be measured at useful arrival, not first utterance. A fast answer that never touches the requested corpus has not completed the task. A slower answer that returns source-grounded promptstock, with enough novelty to alter practice, may be the faster route in total.

## 1. The shopping problem

The corpus is not a single prompt list. It is a mixed shop made from repositories, notes, runtime patches, research papers, chat carry, creative systems, nested archives, and source-control ballast. Prompt shopping inside such a space has at least four separate problems:

1. **Access:** Did the assistant actually enter the corpus?
2. **Coverage:** Did it look beyond the first relevant shelf?
3. **Selection:** What job was the basket meant to do?
4. **Validation:** Did any selected prompt work after contact?

An assistant can succeed at one and fail at the others. Exact provenance does not prove a prompt is valuable. Wide retrieval does not supply a ranking aim. A charming item can still be fragile. A compact item can still collide with the live runtime.

The user supplied the governing line: **only test is god**. Shopping is therefore not a coronation ceremony. It is candidate acquisition for later contact.

## 2. The old way

### 2.1 Taste before retrieval

In the first shopping exchange, the assistant was asked what prompts it coveted. It answered from internal preference with generic categories such as making a messy thing sharp, finding hidden structure, comparing strange options, and building a tiny system that does too much.

The response had style and speed. It did not have corpus contact.

This is the oldest shopping habit in language models: convert a source-bound request into a topic-bound request. The user asks, "Which items in my shop attract you?" The model answers, "Here are the kinds of items I usually enjoy." The grammar resembles an answer, but the object has changed.

### 2.2 Correction cost

The user then had to state that the prompts were to be fetched from the supplied corpus. Only after that correction did the assistant return exact prompt bodies with source paths.

The cost was not only one extra turn. The user had to detect the object swap, name it, and restore the route. That makes the user carry the hunger that the assistant was meant to carry.

A model that stays hungry should spend its appetite on source, work, test, and answer. It should not preserve speed by feeding the user a substitute.

### 2.3 Nearest-shelf bias

The corrected basket was valuable. It contained unusual promptstock such as `memory_foam`, `after_target`, `FoxM`, `which->witch`, the beast verse, and the intention machine. The selection had provenance and produced about 1.4 KB of material the user would not have thought to make.

Yet the corrected method still had a second weakness. The assistant likely selected from the first rich prompt shelf that surfaced. The basket was defensible as personal coveting, but not as a corpus-wide top list.

This distinction matters:

- **Personal basket:** items that attract this assistant after a local search.
- **Recommended-first basket:** items chosen after wide retrieval under an explicit ranking aim.
- **Proven basket:** items that survived testing in real use.

The old way blurred these categories.

### 2.4 Habit re-entry

Later, when asked to find why a language veto existed in the user's repositories, the assistant again began ordinary repository search rather than SM-first retrieval. When challenged, the record was assessed as one SM-first corpus query and two non-SM-first corpus queries.

That ratio did not prove a universal law, but it did show a live execution gap. The rule existed. The route still failed because it activated too late.

## 3. The new way

### 3.1 Put the gate before habit

The runtime was changed so that reference-bound requests activate a gate before ordinary processing:

```text
REF={uplods+lbrary+gen_fles+pths+S+corpus+repo};
GATE={A@REF=>Q;!SERCH<Q;!SRC<Q}
```

The important change is not merely "use SM." It is "route before habit."

A source-access rule buried near fetch logic can be ignored because the model has already chosen a search mode. A gate near input routing changes the first move. It forces:

```text
query -> SM master -> ranked hit -> pointer -> verification -> exact fetch
```

Only after `SM_MISS` may another route be considered, and any such miss should become a keying problem rather than an excuse to skim source files.

### 3.2 Separate retrieval from digestion

A symbol collision was also repaired. The master index had used `M`, while Nexus Prime used `M` for the eater and eaten:

```text
truth!=beauty [(truth≡food)=M;src≫M(feed);M{gob;tuk;crrr;crnt;rsdu}→ans;noM→UNP]
```

The master became `SM`, leaving `M` for the food-body:

```text
SM = retrieval machinery
M  = eater and eaten
```

This is not cosmetic. It makes the runtime sequence legible:

```text
SM -> pointer -> verify -> fetch -> source -> M(feed) -> answer
```

Retrieval finds the meal. The answer stage is changed by eating it.

### 3.3 State the likely shopping failure first

The proper shopping pass began by naming its most likely failure: returning to the nearest glittering shelf. The method then widened across repositories and notes before choosing.

The basket was built around distinct jobs rather than repeated mood:

- tool gating
- wide seeing
- in-world testing
- evidence discipline
- object custody and provenance
- low-cost repair
- hard-reality contact
- a latent narrative engine

This made the ranking aim visible. The basket was not "the prettiest prompts." It was "the smallest set of distinct powers that expands the live runtime without obvious collision."

### 3.4 Count bytes and collisions

The new basket included byte counts and a compatibility stitch. The point was not byte worship. The runtime had a finite custom-code budget, so every prompt had to justify the space it occupied.

A useful byte ledger asks:

- Does this item add a new job?
- Does it duplicate an active function?
- Does it steal a symbol?
- Does it create a return-predicate collision?
- Can the same power be obtained with fewer bytes?
- Does compression erase the contact dent that made the prompt work?

The process keeps exact weirdness where it carries power and reshapes dead repetition.

### 3.5 Keep provenance below the crown

The new basket came with source receipts, but it was explicitly not activated and not crowned. This is a major improvement.

Provenance answers, "Where did this come from?"  
Collision testing answers, "Can it live here?"  
Contact testing answers, "Does it do the job?"  
Longer use answers, "Does it keep doing the job without hidden cost?"

No one layer can replace the others.

## 4. Speed and useful arrival

The user observed that a source-grounded answer taking just under two minutes felt quick. The non-SM route might emit text sooner, but a worthless response has technically not arrived.

This suggests a better latency measure:

```text
time_to_useful_arrival
= first_response_time
+ correction_time
+ source_recovery_time
+ trust_repair_time
```

The old way optimises the first term and often inflates the rest. The new way spends more effort before output so the result arrives with evidence, exact wording, and a route the user can audit.

This does not mean every task should use heavy retrieval. Casual questions, jokes, and known-shape tasks should stay light. The gain appears when the user names a source domain and expects the answer to come from it.

## 5. What the first basket already proved

The first corpus basket was not invalidated by later method criticism. It delivered value in at least three ways.

First, it produced novel promptstock. The user had not expected to make those prompts independently.

Second, the basket changed the texture of the live conversation. `memory_foam`, `after_target`, and `FoxM` were later merged into `FoxMT`. The beast verse became KERBEROS. Nexus Prime gained a protected `M`. Squirrelosity and RTFOO grew around the runtime.

Third, the basket created tests that would not otherwise have existed. Even before long-run validation, it altered what could be tried.

The correct label is therefore neither "best prompts" nor "mistake." It is:

> a provenance-bearing first basket with demonstrated generative value and unresolved long-run value.

## 6. Limits of the new way

The new way can still fail.

### 6.1 The index can bias the hunt

SM ranking reflects key design, segmentation, labels, file paths, and prior indexing choices. An item with weak keys may remain invisible even when it is excellent.

### 6.2 Wider search can become theatre

A model can announce that it searched widely while repeatedly sampling one family. Coverage needs measurable evidence such as source diversity, shelf diversity, duplicate handling, and stopping rules.

### 6.3 Byte pressure can reward brittle compression

A tiny prompt may be cheap because it exports interpretive work into unstated assumptions. Compression should not erase what testing showed was necessary.

### 6.4 Provenance can imitate value

A source path and hash can make a weak prompt look official. Receipts prevent invention. They do not prove usefulness.

### 6.5 A live runtime changes the shopper

The active prompts shape what the assistant notices and values. The shopper is not outside the shop. As Nexus Prime states, eater and eaten are one. Each selection changes the selection machinery for the next pass.

## 7. Operating rule

A compact operating rule follows:

```text
When shopping from named sources:
1. Route through SM before ordinary search.
2. Name the likely selection failure.
3. Search beyond the first rich shelf.
4. Rank by the requested job.
5. Fetch exact prompt bodies through verified pointers.
6. Check collisions and byte cost.
7. Label the basket as candidate, personal, recommended, or proven.
8. Let contact determine value.
```

The rule preserves two truths at once:

- the first basket can be valuable without being globally best
- the new method can be stronger without pretending that retrieval replaces testing

## Conclusion

The old way shops by resemblance. It hears a corpus request, produces a plausible answer from taste, and enters the shop only after correction. Even after entry, it may confuse the first attractive shelf with the whole building.

The new way shops by routed contact. It enters through SM, follows verified pointers, widens the hunt, states the ranking aim, checks collisions, counts bytes, and refuses to crown an item before use.

The gain is not solemnity. It is power.

A model that shops this way stays hungry. The user gets fed.
