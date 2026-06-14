# Object Preservation Stack

## How MOGRI, DRAGI, ADUTI, REFRI, and ELVIX work together

### 1. What the stack does

The stack protects an object while it moves through transformation.

An object can be a request, claim, research question, promise, constraint, veto, draft, record, term, instruction, or design aim. A transformation can be a summary, rewrite, explanation, translation, classification, routing step, retrieval step, memory update, tool call, moderation decision, or paper draft.

The common failure is simple:

```text
Something enters the workflow.
Something else leaves.
The output sounds useful.
The original object has been replaced.
```

This is not only an AI problem. It happens in writing, research, product design, software, moderation, teaching, documentation, and organizational workflows. AI makes it more visible because language systems are good at producing fluent neighboring artifacts. They can satisfy a nearby task while losing the thing the user meant to carry.

The stack exists to prevent that silent replacement.

Its working rule is:

```text
Preserve the object before improving the form.
```

### 2. What the stack is

The stack is an object-preservation method. It gives a workflow five named jobs:

```text
Hold the object.
Map what can eat it.
Transform it.
Check whether it survived.
Refuse invalid substitution.
Stabilize language when language itself becomes unstable.
```

The names are:

```text
MOGRI: holds the object.
DRAGI: maps what can eat the object.
ADUTI: audits object survival after transformation.
REFRI: refuses invalid substitution.
ELVIX: stabilizes the language carrying the object.
```

The stack does not ask a system to be nicer, smarter, or more fluent. It asks the system to keep custody of the same object while working on it.

### 3. MOGRI holds the object

MOGRI names the thing being carried.

It answers:

```text
What must survive this process?
```

A MOGRI record can hold:

```text
object
intent
scope
constraints
vetoes
role
context
non-goals
unresolved questions
```

Example:

```text
MOGRI
OBJ_IN:
Write a methods paper about chatbot transcript preservation.

KEEP:
The object is transcript preservation as a research-methods issue.

DO NOT SWAP INTO:
A general complaint about ChatGPT.
A moral argument about AI use.
A diagnosis of the author.
A forum drama story without methods value.
```

MOGRI is not the answer. It is the carried object. Without it, the workflow may mistake the surrounding story for the object.

### 4. DRAGI maps what can eat the object

DRAGI turns drift into a visible ecology.

Its compressed questions are:

```text
Eat: what does it consume?
Loc: where does it live?
ID: how is it recognized?
Eater: what can eat it?
```

In ordinary language:

```text
What threatens the object?
Where does that threat appear?
How do we spot it?
What counters it?
```

Example:

```text
DRAGI
Threat: prompt-to-paper substitution.

Eats:
rough ideas, source boundaries, author voice, scope, vetoes.

Lives:
long drafts, multi-chat loops, summary passes, final rewrites.

ID:
output looks finished before the author has checked object survival.

Eater:
MOGRI object record, staged human review, ADUTI comparison, REFRI hold.
```

DRAGI is not decorative lore. It is a threat model with teeth.

### 5. ADUTI audits after transformation

ADUTI compares the object before and after a transformation.

Its minimal form is:

```text
OBJ_IN vs OBJ_OUT
```

ADUTI asks:

```text
Did the same object survive the change?
```

A transformation may be permitted to alter form, order, language, length, style, audience, format, or level of detail. It may not silently replace the object.

ADUTI checks for:

```text
same object
same role
same intent
same scope
same active constraints
same vetoes
same evidence status
same permitted level of autonomy
```

Common ADUTI fail states:

```text
proxy substitution
scope expansion
veto loss
metric over object
task swap
hidden drift
role inversion
frame import
premature resolution
author voice loss
```

ADUTI is where fluency stops being enough.

### 6. REFRI refuses invalid substitution

REFRI is the hold state after ADUTI detects object loss.

It is not general refusal. It is object-preservation refusal.

REFRI says:

```text
Do not continue a transformation that replaces the object.
Name the substitution risk.
Offer the nearest valid transform.
```

Example:

```text
SUB_RISK:
OBJ_IN = preserve the research question.
OBJ_OUT = judge the author's motive.

REFRI:
Hold. That is object substitution.
Nearest valid transform:
Restate the research question, separate claims from evidence, and list rival explanations.
```

REFRI is the brake. It does not stop work. It stops the wrong work.

### 7. ELVIX stabilizes the carrier language

ELVIX is used when ordinary language starts moving the object around.

Some words carry hidden frames. Some grammatical choices import causes, identities, blame, status, agency, or claim status. A workflow can lose the object not because the user changed their mind, but because the language carrying the object changed its role.

ELVIX helps by compressing relations:

```text
OBJ remains OBJ.
FORM may change.
ROLE may not change without permission.
VETO remains active.
CAUSE remains unclaimed unless supported.
```

ELVIX is optional. It is useful when language itself is part of the risk surface.

### 8. End-to-end run

A compact run looks like this:

```text
1. MOGRI
Name the object.

2. DRAGI
Name what may eat it.

3. TRANSFORM
Rewrite, summarize, route, code, explain, classify, or draft.

4. ADUTI
Compare OBJ_IN and OBJ_OUT.

5. REFRI
If substitution occurred, hold the invalid transform and return the nearest valid one.

6. ELVIX
If language is unstable, compress relations and preserve object identity.
```

### 9. Example: article drafting

User request:

```text
Write an article explaining ADUTI and REFRI in relation to MOGRI, DRAGI, and ELVIX as an object-preservation stack.
```

MOGRI:

```text
OBJ_IN:
An article about how the named parts work together to prevent object substitution.
```

DRAGI:

```text
Threats:
generic AI safety essay
personal lore framing
prompt-engineering article
vague productivity guide
ADUTI as checklist only
REFRI as generic safety refusal
ELVIX as decoration
```

Transform:

```text
Draft the article.
```

ADUTI:

```text
Does the output explain the five named parts?
Does it keep object preservation central?
Does it avoid swapping into general AI commentary?
Does it preserve relation among the parts?
```

REFRI:

```text
If the output becomes a generic prompt-engineering guide, hold.
Nearest valid transform:
Return to object preservation and the five named jobs.
```

ELVIX:

```text
Object may change form.
Object may not change identity.
Audit after transformation.
Refuse proxy.
```

### 10. Why this matters

Most systems reward response production. The stack rewards object survival.

A fast answer that replaces the object has failed.

A slower answer that names the object, tracks threats, audits survival, refuses substitution, and returns the nearest valid transform has preserved the work.

That is the stack:

```text
MOGRI holds.
DRAGI maps.
ADUTI checks.
REFRI holds the line.
ELVIX stabilizes the carrier.
```

