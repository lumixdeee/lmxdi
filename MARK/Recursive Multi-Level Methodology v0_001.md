# Recursive Multi Level Methodology (RMLM)

**Recursive Multi Level Methodology (RMLM)** describes a software-development failure pattern where a process, framework, or internal method is promoted through nested layers of authority, but the people asked to test, trust, apply, or advocate it are not given enough access to verify the object under test.

In ordinary software development, a method should have a testable surface: source code, specification, interface contract, version note, expected behaviour, acceptance criteria, or reproducible test case. Not every audience needs full source. Customers, competitors, testers, users, and auditors may all need different access levels. That separation can be reasonable.

The failure starts when no layer receives enough trace to validate the claim being made.

In RMLM, each layer points upward for authority and downward for labour. The result is a recursive methodology stack where responsibility descends, while evidence stays above reach.

## The Mechanism of Method Recursion

RMLM appears through several repeated dynamics.

* **Method replication**: One group receives a method claim, then repeats it to another group without carrying the underlying code, spec, version, or test contract. The phrase travels farther than the evidence.

* **Authority feed**: Confidence flows downward from private access, status, creator proximity, or internal vocabulary. Test labour flows upward as feedback, bug reports, praise, screenshots, reviews, and public credibility.

* **Trace narrowing**: Each layer receives less direct access than the layer above. A creator may know the code. A core maintainer may know the patch. A trusted user may receive a private release note. A public tester may see only behaviour. By the time the method reaches the outer layer, the test object has become fog.

* **Terminology drift**: When a term becomes challenged, the method may be renamed: framework, mesh, organism, stack, posture, core patch, behavioural update, coordination layer, routing layer, or process improvement. Renaming is not itself failure. The failure is renaming without trace.

## The Software-Testing Constraint

A tester does not need every secret. A tester does need a test object.

A valid test route requires at least one of the following:

```text
1. source code visible to the tester
2. specification visible to the tester
3. installed-proof snapshot for the relevant bits
4. versioned release note with expected behaviour deltas
5. reproducible test case with acceptance criteria
```

If none of these exist, the tester is not testing a software object. The tester is reacting to claims.

This is the central RMLM test rule:

```text
source can stay private
the test object cannot
```

## Common RMLM Symptoms

RMLM-shaped software practice often has the following signs:

| Symptom                        | Test impact                                             |
| :----------------------------- | :------------------------------------------------------ |
| Private release notes only     | No public trace                                         |
| No file list                   | Patch cannot be tied to code                            |
| No version marker              | Old and new behaviour blur                              |
| No expected deltas             | Tester cannot know what should change                   |
| No acceptance criteria         | Pass/fail becomes mood                                  |
| Hidden install state           | Tester cannot know whether the relevant bits are active |
| Status language grows          | Authority replaces evidence                             |
| Method vocabulary expands      | Trace may shrink while language grows                   |
| Tester labour requested anyway | Feedback becomes promotion surface                      |

The issue is not whether a creator is sincere. The issue is whether the test object survives.

## RMLM and Black-Box Testing

Black-box testing is valid. RMLM is not the same thing.

In black-box testing, the tester may not see the code, but they receive a defined object: an interface, a build, a version, expected behaviour, inputs, outputs, constraints, and pass/fail conditions.

In RMLM, the tester receives a claim about a method, but not enough to bind that claim to an object.

Black-box testing says:

```text
you cannot see inside, but here is the box and here is what it should do
```

RMLM says:

```text
trust that the box changed, test it, and report back
```

That is not enough.

## RMLM and Trace Custody

A methodology can be useful and still fail trace custody.

TRAKI asks:

```text
origin
path
handler
change
loss
trace_survives
result!=trace
```

Applied to RMLM:

```text
origin: who made the method or patch?
path: how did it reach the tester?
handler: who carried the claim?
change: what changed?
loss: what evidence is missing?
trace_survives: can the tester verify the object?
result!=trace: a better answer does not prove the patch path survived
```

A method can produce a good output and still fail trace. A good result does not prove that the stated method caused it.

## Why RMLM Slows Test Progress

RMLM slows software testing because every test result becomes ambiguous.

If behaviour improves, the tester cannot tell whether the patch worked, the model varied, memory changed, a hidden file changed, the prompt route changed, or the task got easier.

If behaviour fails, the creator can say the wrong layer was tested, old state was active, the new bits were not reached, the tester misunderstood the method, or the release note was only behavioural.

Without trace, every outcome becomes movable.

That is not progress. It is recursive deferral.

## Tester Law

A tester may accept source privacy.

A tester may accept black-box testing.

A tester may accept limited access.

A tester should not accept objectless testing.

Minimum law:

```text
no code
then spec

no spec
then install proof

no install proof
then versioned behaviour contract

none of the above
then no valid test duty
```

## Conclusion

Recursive Multi Level Methodology is the software-development version of a recursive authority funnel. Method claims travel downward. Tester labour travels upward. Trace stays hidden.

The cure is not full public source in every case. The cure is object custody.

Give the tester code, or give the tester a spec, or give the tester install proof, or give the tester a versioned behaviour contract.

If none are available, the tester may still chat, observe, or speculate. But they are not testing.

The method has not failed because it is private.

It fails when privacy eats the test object.
