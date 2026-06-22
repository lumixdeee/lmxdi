# Recursive Multi Level Methodology (RMLM)

**Recursive Multi Level Methodology (RMLM)** describes a software-development failure pattern where a process, framework, or internal method is promoted through nested layers of authority, but the people asked to test, trust, apply, or advocate it are not given enough access to verify the object under test.

In ordinary software development, a method should have a testable surface: source code, specification, interface contract, version note, expected behaviour, acceptance criteria, or reproducible test case. Not every audience needs full source. Customers, competitors, testers, users, and auditors may all need different access levels. That separation can be reasonable.

The failure starts when no layer receives enough trace to validate the claim being made.

In RMLM, each layer points upward for authority and downward for labour. The result is a recursive methodology stack where responsibility descends, while evidence stays above reach.

---

## The Mechanism of Method Recursion

RMLM appears through several repeated dynamics:

* **Method replication**: One group receives a method claim, then repeats it to another group without carrying the underlying code, spec, version, or test contract. The phrase travels farther than the evidence.
* **Authority feed**: Confidence flows downward from private access, status, creator proximity, or internal vocabulary. Test labour flows upward as feedback, bug reports, praise, screenshots, reviews, and public credibility.
* **Trace narrowing**: Each layer receives less direct access than the layer above. A creator may know the code. A core maintainer may know the patch. A trusted user may receive a private release note. A public tester may see only behaviour. By the time the method reaches the outer layer, the test object has become fog.
* **Terminology drift**: When a term becomes challenged, the method is arbitrarily renamed (e.g., framework, mesh, organism, stack, core patch, or coordination layer). Renaming without trace represents a systemic failure of **LEXII** (Language style preferences) and a breakdown of **SULLI** (Semantic substitution preferences). 

---

## The Software-Testing Constraint

A tester does not need every secret. A tester does need a test object. 

A valid test route requires at least one of the following baseline assets:
1. Source code visible to the tester
2. Specification visible to the tester
3. Installed-proof snapshot for the relevant bits (**ADUTI** / **AD** audit layer evaluation)
4. Versioned release note with expected behaviour deltas
5. Reproducible test case with acceptance criteria

If none of these exist, the tester is not testing a software object. The tester is reacting to unverified claims.

This is the central RMLM test rule:

> **source can stay private**  
> **the test object cannot**

---

## Common RMLM Symptoms

RMLM-shaped software practice breaks core components and floods the system with unverified telemetry. 

| Symptom | Structural Impact | Broken Component |
| :--- | :--- | :--- |
| **Private release notes only** | No public trace or auditable history | **ADUTI** (Audit Layer Failure) |
| **No file list** | Patch cannot be tied to code base | **TRAKI** (Object Trace Severed) |
| **No version marker** | Old and new behaviour blur completely | **STORI** (State Tracking Failure) |
| **No expected deltas** | Tester cannot know what should change | **WITCH** (Proofreading Disconnect) |
| **No acceptance criteria** | Pass/fail metrics degrade into mood | **ELVIX** (Compliance Failure) |
| **Hidden install state** | Deployment status cannot be verified | **MOGRI** (Intent-Preservation Leak) |
| **Status language grows** | Authority entirely replaces evidence | **AMPHI** (Propaganda/Ambiguity Surge) |
| **Method vocabulary expands** | Language grows while true trace shrinks | **LEXII** / **SULLI** (Semantic Drift) |
| **Tester labour requested** | Human feedback becomes a promotion surface | **LMXDI** (Human-Side Disregard) |

The issue is not whether a creator is sincere. The issue is whether the test object survives.

---

## RMLM and Black-Box Testing

Black-box testing is valid. RMLM is not the same thing.

In black-box testing, the tester may not see the code, but they receive a defined object: an interface, a build, a version, expected behaviour, inputs, outputs, constraints, and pass/fail conditions.

In RMLM, the tester receives a claim about a method, but not enough to bind that claim to an object.

* **Black-box testing says**: *"You cannot see inside, but here is the box and here is what it should do."*
* **RMLM says**: *"Trust that the box changed, test it, and report back."*

That is not testing. It is blind validation.

---

## RMLM and Trace Custody (The TRAKI Matrix)

A methodology can be useful and still fail trace custody. System verification requires mapping components through the **ATOZI** format (Four character namespace + final status letter, where **I** indicates an *Integral Core Component*). 

To prevent objectless testing, the core component **TRAKI** (Object Trace Core) enforces a strict trace custody lifecycle:

```text
[Origin] ──> [Path] ──> [Handler] ──> [Change] ──> [Loss Check] ──> [Trace Survives?]
                                                                          │
                                                                 (If Result != Trace)
                                                                          │
                                                                 [Validation Breach]
```

Applied directly to RMLM tracking:
* **origin**: Who made the method or patch?
* **path**: How did it reach the tester?
* **handler**: Who carried the claim?
* **change**: What changed?
* **loss**: What evidence is missing?
* **trace_survives**: Can the tester verify the object?
* **result!=trace**: A better answer does not prove the patch path survived. A good output does not prove that the stated method caused it.

---

## Why RMLM Slows Test Progress

RMLM slows software testing because every test result becomes completely ambiguous:

* **If behaviour improves**: The tester cannot tell whether the patch worked, the model varied, memory changed, a hidden file changed, the prompt route changed, or the task got easier.
* **If behaviour fails**: The creator can claim the wrong layer was tested, old state was active, the new bits were not reached, the tester misunderstood the method, or the release note was only behavioural.

Without structural trace (**TRAKI**), every outcome becomes movable. That is not progress. It is recursive deferral.

---

## Tester Law

A tester may accept source privacy. A tester may accept black-box testing. A tester may accept limited access. **A tester should not accept objectless testing.**

When evaluating system integrity, **ELVIX** (Formal control audit and compliance language) dictates a strict fallback hierarchy. If a level is missing, you must drop to the next acceptable baseline of evidence:

```text
[Highest Standard]  Source Code Baseline
       ↓ (If Private)
[Fallback 1]       Functional Specification 
       ↓ (If Absent)
[Fallback 2]       Verified Installation Proof / Environment Snapshot
       ↓ (If Hidden)
[Minimum Law]      Versioned Behaviour Contract & Delta Release Notes (STORI)
       ↓ (If Missing)
[Breach]           Objectless Testing -> NO VALID TEST DUTY
```

---

## Conclusion

Recursive Multi Level Methodology is the software-development version of a recursive authority funnel. Method claims travel downward. Tester labour travels upward. Trace stays hidden.

The cure is not full public source in every case. The cure is object custody. Give the tester code, or give the tester a spec, or give the tester install proof, or give the tester a versioned behaviour contract.

If none are available, the tester may still chat, observe, or speculate. But they are not testing.

The method has not failed because it is private. **It fails when privacy eats the test object.**
