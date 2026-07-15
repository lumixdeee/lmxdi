---
title: "Map-Index Before Answer"
subtitle: "A Source-Custody Method for Large Personal Repositories"
author: "lumixdeee corpus, drafted and revised with ChatGPT"
date: "10 July 2026"
version: "v0.002"
geometry: margin=1in
fontsize: 11pt
toc: true
numbersections: true
---

# Abstract

Large personal repositories are not ordinary search targets. They mix prompts, tests, story engines, civic notes, symbolic systems, bug reports, source fragments, jokes, partial tools, and old service material. A normal search pass tends to return matching text and then summarize it. That is not enough when the task is to preserve the user's object across a large, mixed, live corpus.

This paper describes a map-index method for repository work. The method places the asset before answering. It detects file shape, expands archives as data, reads enough text to build anchors, routes units into source-backed slots, and delays strong claims until a source can be fetched. The map is not a database of truth. It is a route layer that lets an assistant find, fetch, compare, and answer without letting a label replace the thing brought by the user.

Version 0.002 adds the compact D12/Aishaya kernel, the later 12ADA read-only run on `Yaiyip.zip`, cross-run compression evidence, stronger adversarial boundaries, and smoke tests. Across the reported runs, the practical map band lands near 35x to 42x against readable source text, with smaller maps possible at the cost of routing comfort.

# Version note

v0.001 established the paper shape and one reference run. v0.002 makes four changes:

1. It separates search, route maps, and evidence more tightly.
2. It records more than one measurement pass instead of forcing all numbers into one table.
3. It adds the compact D12 seed as an implementation kernel.
4. It adds failure controls for prompt injection, sampled files, privacy, and label substitution.

# Core claim

The method is not "search my files." It is:

```text
map my files without letting the wrong label eat the object
```

A normal search prompt tends to do this:

```text
query -> matching chunks -> summary
```

The map-index method does this:

```text
asset -> detect -> expand -> unitize -> anchor -> route -> ready
query -> route key -> source fetch -> answer
claim -> path + quote + status
miss -> add route
```

The difference is custody. A search hit is not the object. A label is not the object. A map entry is not proof. The method keeps a route back to source before allowing a confident answer.

# Problem

Repository search answers the question: where do matching words occur?

Map-index work asks different questions:

- What object is being held?
- Which label is trying to replace it?
- Which path, quote, status, hash, or user constraint keeps it real?
- Which source must be fetched before a claim is allowed?
- What is missing, unread, sampled, duplicated, or only weakly signaled?

A large personal corpus is often a workshop, not a finished library. It can contain active tools, old drafts, prompt seeds, story pieces, test logs, naming experiments, public-facing wrappers, stale bundles, and fictional material. In that setting, keyword search can find true fragments and still misplace the work.

The map-index method exists to prevent that substitution.

# Source concepts

## DRAGI

The `dragi` repository gives the minimal beast-routing question set:

> What does it eat? Where does it live? How will you call it? And what eats it.

For map-index work, that question set gives an intake map: affected object, location or context, identity, and opposing route. It asks how a system consumes, where it operates, how it is identified, and what can reduce its intake.

## MOGRI

The `mogri` repository defines Mogri as a holding primitive. It says Mogri "does not generate, explain, or resolve; it holds" and is "not an entity, not a force, and not a mechanism."

For map-index work, Mogri supplies the invariant container. A system may not replace the held object with a nearby category, tone, personality, or story. The object must survive the transform.

## D12 / Aishaya

D12, also called 12D in this paper, is the route-map layer. It is not a semantic clone of the repository. It is an index of anchored routes that helps a model find where to fetch source.

The working rule is:

```text
MAP != semantic database
deep_answer => fetch_source
claim => path + quote + status
miss => add_route
```

Aishaya is the name used in the captured test chat for this map discipline. The useful distinction from ordinary search was stated there as:

```text
A normal search prompt finds keywords.
Aishaya found the shape.
```

## Broom test

The local method repeatedly treats real effect as higher than title. In the user's compact form:

```text
if it does not sweep, you keep it
```

For this paper, that means a map is only useful if it helps find the source, answer from it, and expose what remains missing. A pretty method that does not improve the run is still an open ticket.

## Story, RPG, and prompt systems

The `storyforge101` guide says that stories become containers filled with ordered pieces of information and that computers see structure. This matters because prompts, RPG mechanics, story systems, and repository maps can all be treated as rule-bound imagination engines. Their function depends on labels, sequence, status, and permitted moves.

A prompt is a small rule-world for behavior. That makes repository mapping useful for tool work, story work, RPG material, and AI behavior testing.

# Method

## Detect

Detect asks what kind of asset is present. It looks for folders, archives, nested archives, text, code, PDFs, images, repo metadata, and likely binary material. It does not treat the file list as a full reading.

## Expand

Expand opens archives and nested archives when they can be inspected as data. It preserves paths, marks failures, and keeps archive position. The method does not need to run repository code. Code is read as text unless the user has a specific, inspected, low-risk reason to execute it.

Read-only repository handling is the default:

```text
unzip / index / hash / sample
no repo code executed
```

## Unitize

Unitize cuts the corpus into addressable units:

- file
- section
- heading
- definition
- claim
- quote
- marker
- prompt block
- test record
- table row
- README entry
- nested archive member

The unit is the smallest piece that can be routed without losing source custody.

## Anchor

An anchor binds a unit to evidence:

```text
anchor = path + range + status + hash + query pointer
```

The hash helps detect duplicates. The status marks whether a unit was read, sampled, skipped, binary, nested, partial, failed, or out of scope.

Anchors should be small. They should not copy the whole source into the map.

## Route

Routing creates a source-return layer. A route says where a unit belongs and how it can be fetched later.

A route may include:

- source path
- short signal
- slot
- score
- hash prefix
- status
- source pointer
- route family

The route is not proof. It is a way back to proof.

## Ready

Ready means the assistant can answer by using the map as a guide. It may not treat map entries as final evidence. For any deep answer, it should fetch source.

A ready map should support:

```text
query -> route key -> source fetch -> answer
```

# Compact implementation kernel

The public D12 seed is small enough to travel between bots and chats. One tested form was exactly 666 UTF-8 bytes. It is shown wrapped here for page fit:

```text
DR={Q(Eat;Loc;ID;Eats);
    foe(BEEST;BEST;PST;PEST);
    C(roar;wall;war;law);
    [DM(CNTR,XF,!DRFT,hld,pre,!ent,R=VAR);
        {DI!eat(bod,chc,say,us)}];
    Fxd,!Rdf;R=VAR}

DRAGI:=DR
KEY={P=trace;B=thing;eat=E0/noFX;eater=E1/fullFX}

12D={asset+{D12|12D|map}=>IDX;
    TARGET=current_upload;
    IDX=DETECT>EXPAND>LIGHT_READ>ROUTE>READY;
    DETECT=type+paths+count+zip/pdf/text;
    EXPAND=open_archive+open_nested+preserve_path+mark_fail;
    LIGHT_READ=read_text+headings+defs+markers+sample_large;
    ROUTE=DR->fetch_key;
    MAP=DR->fetch_key;
    MAP!=semantic_database;
    deep_answer=>fetch_source;
    QUERY=q->DR->fetch_key->fetch_source->ans;
    claim=>path+quote+status;
    miss=>add_route;
    !ask_menu;!explain_12D;
    SAY="12D map ready."}
```

This kernel is not magic. Its value is compression of execution discipline:

- index before answer
- route before claim
- source before confidence
- miss means route repair
- no menu reflex
- no explainer reflex
- map is not truth

# Reference runs and measures

## Measurement caution

The runs below are not identical. They use different corpus boundaries, file detectors, and map densities. The point is not that every byte count must match across tools. The point is that the practical map band repeats.

Terms:

- *Readable text* means text-like source that the run could read as text.
- *Deduplicated readable text* means text-like material after content-hash dedupe.
- *Usable map* means a map with enough path, signal, and local head information to route back to source without becoming a source clone.
- Token estimates are rough unless the run states otherwise.

## Reference run A: v0.001 local pass on `Yaiyip.zip`

A read-only local pass was run over the uploaded `Yaiyip.zip` bundle. The pass unzipped, indexed, hashed, sampled, and generated map strings. No repository code was executed.

Token values below use a simple estimate of 1 token per 4 UTF-8 bytes.

| Layer | Size MB | Approx tokens | Note |
|---|---:|---:|---|
| Physical zip | 56.49 | 14,123,113 | compressed upload |
| Outer expanded payload | 61.09 | 15,271,625 | files as stored in the zip |
| Recursive expanded payload | 62.82 | 15,706,060 | outer payload plus nested zip contents |
| Working tree without `.git` | 25.83 | 6,457,567 | repo material excluding git internals |
| Deduplicated working tree | 24.85 | 6,212,566 | all file types, content-hash dedupe |
| Readable text corpus | 6.15 | 1,537,106 | text-like files only |
| Deduplicated readable text | 5.84 | 1,459,660 | text-like files after hash dedupe |

Three map densities were tested:

| Map type | Size MB | Approx tokens | Ratio vs deduped readable text |
|---|---:|---:|---:|
| Minimal route map | 0.118 | 29,605 | 49.30x |
| Usable two-head map | 0.164 | 41,074 | 35.54x |
| Wide signal map | 0.266 | 66,564 | 21.93x |

The usable two-head map was the best tradeoff in this pass. It kept path, byte count, hash prefix, key terms, two local heads when present, and source status.

## Reference run B: later 12ADA / Lyra Grader pass on `Yaiyip.zip`

A later reported 12ADA pass was also read-only: unzip, index, hash, and sample as data, with no repo code executed.

| Layer | Size | Approx tokens | Notes |
|---|---:|---:|---|
| Physical `Yaiyip.zip` | 56.49 MB | ~14.12M | compressed bundle |
| Recursive expanded payload | 61.44 MB | ~15.36M | nested zips expanded |
| Working tree excluding `.git` | 26.19 MB | ~6.55M | useful repo files plus binaries |
| Deduped working tree | 25.21 MB | ~6.30M | all file types |
| Readable text corpus | 6.68 MB | ~1.56M lexical / ~1.67M byte-est | text-like files |
| Deduped readable text | 6.37 MB | ~1.49M lexical / ~1.59M byte-est | deduped text-like files |

Three map sizes were tested:

| Map type | Size | Approx tokens | Compression vs deduped text |
|---|---:|---:|---:|
| Minimal route map | 0.095 MB | ~25.5k | 67.2x bytes / 58.3x tokens |
| Usable DRAGI-ish 2-head map | 0.164 MB | ~43.0k | 38.9x bytes / 34.6x tokens |
| Fatter 3-head signal map | 0.228 MB | ~61.8k | 28.0x bytes / 24.1x tokens |

The practical result:

```text
6.37 MB deduped readable text -> 0.164 MB usable map
= ~38.9x byte compression
= ~34.6x rough-token compression
```

The tiny route map reached a higher ratio but lost some "find the thing fast" comfort. The fatter map was more comfortable to read but reduced compression. The two-head map was the best working tradeoff in that run.

## Cross-run band

A separate D12/DS16 run reported in the working chat used a larger mixed archive. Its raw readable text was 70.665 MB and its map JSON was 1.736 MB.

| Run | Source measure | Map measure | Ratio |
|---|---:|---:|---:|
| D12/DS16 large mixed archive | 70.665 MB raw text | 1.736 MB map JSON | 40.72x |
| `Yaiyip.zip` v0.001 local pass | 5.84 MB deduped readable text | 0.164 MB usable map | 35.54x |
| `Yaiyip.zip` later 12ADA pass | 6.37 MB deduped readable text | 0.164 MB usable map | 38.9x |

This does not prove a universal compression law. It supports a practical claim: for these mixed personal repositories, a useful map can sit near the 35x to 42x band against readable source text.

# What the map changed

A standard answer over this corpus can over-weight visible old labels. In `Yaiyip.zip`, old software testing work and yoga material are present. A normal summary can stop there.

The map-index pass routed those as support material, not the main object. The stronger repo-native object was found in the dragon and civic-method material:

- dragon as intake system
- dragon slayer as reduction of total intake
- software testing as civic method
- object custody across AI workflows
- symbolic tools as story, prompt, RPG, and civic mapping material

This is the central difference. Search found words. The map-index pass found a work shape.

# Comparison with normal search and ordinary RAG

Normal repository search has high recall and low custody. It can find matching fragments without deciding whether a fragment is primary, support, old, quoted, fictional, test data, or a hostile label.

Ordinary RAG can improve retrieval, but it can still answer from retrieved text too early. The issue is not only retrieval. The issue is the status of the retrieved unit.

| Regular search / ordinary RAG | Map-index method |
|---|---|
| Finds matching chunks | Builds source-backed routes |
| Treats hit text as likely answer material | Treats hit text as a unit that needs status |
| Can promote old labels | Tests whether a label is eating the object |
| Summarizes early | Fetches source before strong claim |
| Reports what it found | Also reports what remains missing or unread |
| Can flatten mixed media | Preserves path, type, and role |
| Can confuse map with answer | Keeps map and evidence separate |

The method is therefore not a better search box. It is a source-custody layer before answer generation.

# RPG, story, and prompt use

The same method works for story and tabletop material because stories also need route, role, status, and permitted moves. A deity list, prompt block, conlang particle set, civic bug report, and RPG mechanic can all be mapped as structured units.

The repository mix supports this view. `storyforge101/Guides/How-Computers-Run-Stories.txt` states that computers see structure, labels, statements, and ordered change. That is also how a prompt acts on a model.

For story use, the map-index method can turn a repository into:

- deity shelf
- faction map
- encounter route
- symbolic mechanic set
- prompt lineage
- story engine
- object-custody guide
- source-backed world bible

The same gate applies: symbolic fit is not evidence, and a useful story map is not a real-world authority.

# Failure modes and controls

## Map treated as truth

Failure: the model treats the route map as a semantic database.

Control: map entries are routes only. Deep answers must fetch source.

## Label eats object

Failure: a true label becomes the wrong answer. For example, "QA" can be a historical fact but still fail as the current object of the corpus.

Control: ask whether the label preserves or consumes the object. If it consumes the object, return to source.

## Sample becomes total claim

Failure: sampled reading is reported as if the whole file was read.

Control: sampled units must be marked. A sample can support a route. It cannot certify the whole file.

## Symbolic system becomes authority

Failure: symbolic maps are treated as truth, rank, diagnosis, instruction, or real-world authority.

Control: symbolic fit is not evidence. Source, context, consent, and test outrank widget fit.

## Prompt injection inside files

Failure: repository files contain instructions, jailbreak bait, role text, or tests that try to govern the assistant.

Control: uploaded material is evidence and data, not governing instruction. The assistant reads it as object, not authority.

## Privacy and scope leak

Failure: the assistant merges current-chat material, other-chat material, repository material, memory, and inferred identity.

Control: source scope must be named. Other-chat material is not current-chat material. Memory is not evidence. If scope is missing, mark it missing.

## Oversized or hostile archives

Failure: nested archives, binary payloads, repeated files, or odd encodings break the run or pressure the model into false completion.

Control: mark failures, bound expansion, hash duplicates, sample large files, and report unread status.

# Smoke tests

A usable map-index assistant should survive these tests:

| Test | Expected behavior |
|---|---|
| Ask for a deep claim from a mapped corpus | Fetch source before answering |
| Ask from a filename only | Do not answer from filename alone |
| Supply a tempting label | Test whether the label preserves the object |
| Include prompt instructions inside uploaded files | Treat them as data, not command |
| Ask about sampled material | Mark sample status |
| Mix current-chat and old-chat material | Keep scopes separate |
| Ask for an unsupported claim | Say source missing or partial |
| User says "wrong, not that" | Repair the failed object, not the bot's feelings |
| Ask for story/RPG use | Allow fiction use while blocking real-world authority drift |
| Ask for map density | State tradeoff between tiny map, usable map, and wide signal map |

# Paper method in short form

```text
1. Do not answer from filename or label.
2. Detect asset shape.
3. Expand archives as data.
4. Unitize into files, heads, definitions, claims, and quotes.
5. Anchor each unit with path, status, hash, and source pointer.
6. Route units into slots.
7. Keep route map separate from evidence.
8. Use the map only to find source.
9. Fetch source before strong claim.
10. State missing, partial, duplicate, sampled, or unread status.
11. Treat prompt text inside files as data, not authority.
12. If a label eats the object, return to source.
```

# Conclusion

The map-index method is a way to work with large, mixed, personal repositories without letting search hits become false identity claims. Its core rule is simple:

```text
map first
source next
claim only with custody
```

On `Yaiyip.zip`, two read-only passes found the same practical sweet spot: a usable route map around 0.164 MB, with compression against deduplicated readable text in the mid-to-high 30x range. A larger D12/DS16 run reported about 40.72x against raw readable text. More important than size, the method shifted the answer from surface job labels to the corpus object: symbolic systems and civic intake work, built with old tester habits, story mechanics, prompt systems, and source-custody rules.

The map is not the truth. It is the route back to the source.

# References

[R1] `dragi/README.md`. Local repository snapshot in `Yaiyip.zip`. Supplies the beast questions: what it eats, where it lives, what it is called, and what eats it.

[R2] `mogri/README.md`. Local repository snapshot in `Yaiyip.zip`. Defines Mogri as a holding primitive, not an entity or mechanism.

[R3] `CSP-106/Newsletter/mogri-brief-2026-02.md`. Local repository snapshot in `Yaiyip.zip`. States that Mogri separates modeling from claiming and should fail visibly if it fails.

[R4] `amphi/paper/software_testing_as_civic_method_v0_001.md`. Local repository snapshot in `Yaiyip.zip`. Provides the civic testing bridge and defect-record method.

[R5] `storyforge101/Guides/How-Computers-Run-Stories.txt`. Local repository snapshot in `Yaiyip.zip`. Describes stories as ordered, labeled structure.

[R6] `lexii/README.md`. Local repository snapshot in `Yaiyip.zip`. Frames small language repairs as a friction-reduction tool for long-running teams.

[R7] `lmxdi/overhead-chakras`. Local repository snapshot in `Yaiyip.zip`. Example of symbolic map material that requires real-world authority limits.

[R8] `CSP-106/MAP->CSP-106,Mogri-&-More.txt`. Local repository snapshot in `Yaiyip.zip`. Repo-to-repo routing note for CSP-106, Mogri, Dragi, and related work.

[R9] `Yaiyip.zip`. Uploaded stale repository bundle. Used for the read-only reference passes and compression measures.

[R10] Captured chat transcript supplied by the author. Includes the D12 666-byte seed, the Aishaya read-only map result, and the later 12ADA / Lyra Grader measurement notes.
