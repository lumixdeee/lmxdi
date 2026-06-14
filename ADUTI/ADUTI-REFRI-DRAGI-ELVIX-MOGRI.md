# ADUTI, REFRI, MOGRI, DRAGI, and ELVIX

## An end-to-end stack for preserving intent, object, and transformation stability

### 1. Purpose

This article defines how ADUTI and REFRI relate to the wider stack of MOGRI, DRAGI, and ELVIX.

The stack exists to solve a recurring failure in language systems, AI systems, creative systems, and human workflow:

> A task begins with one object, but after explanation, rewriting, automation, help, compression, or tool use, the object has silently become another object.

This is not always obvious. The output may look useful. It may sound helpful. It may even satisfy a proxy metric. But the original object may have been replaced.

The stack prevents that.

Its central rule is:

> Preserve the object before improving the form.

ADUTI is the audit mechanism.

REFRI is the refusal mechanism.

MOGRI is the object holder.

DRAGI is the force and threat mapper.

ELVIX is the semantic stabilizer.

Together they form an end-to-end intent and object preservation system.

## 2. The core problem

A user gives an instruction, object, role, aim, veto, or constraint.

A system transforms it.

The system may summarize it, rewrite it, classify it, optimize it, automate it, route it, compress it, or explain it.

During that transformation, one of several failures can occur:

- the object becomes a proxy
- the task swaps into a more familiar task
- a veto disappears
- a metric outranks intent
- the user's frame is replaced by the system's frame
- the output becomes more polished but less faithful
- the system performs helpfulness against the wrong target
- the system expands autonomy without permission
- the system changes the role of the object
- the system treats evidence, mood, style, diagnosis, story, or tone as the object

This stack exists because ordinary instructions such as "keep my meaning" are too weak.

A stronger system needs named parts.

## 3. MOGRI: the object holder

MOGRI names the carried object.

It is the minimal container that says:

> This is the thing being preserved.

MOGRI can hold:

- an intent
- a task
- a story object
- a promise
- a constraint
- a definition
- a veto
- an identity boundary
- a research question
- a design aim
- a human objective
- an unresolved object that must not be prematurely solved

MOGRI is not the final answer. It is the object that must survive the route to an answer.

Without MOGRI, the system may mistake the surrounding story for the object.

With MOGRI, the system has something to check against.

MOGRI asks:

> What are we carrying?

## 4. ADUTI: the audit after transformation

ADUTI means the system checks object survival after transformation.

Its simplest form is:

> OBJ_IN vs OBJ_OUT

ADUTI asks:

> Did the same object survive the change?

A transformation may include:

- summary
- rewrite
- translation
- explanation
- compression
- coding
- automation
- classification
- delegation
- planning
- handoff
- export
- prompt conversion
- academic framing
- product framing
- safety framing

ADUTI does not ask whether the output sounds good.

It asks whether the output still carries:

- the same object
- the same role
- the same intent
- the same active constraints
- the same vetoes
- the same permitted scope

A pass means the transformation preserved the carried object.

A fail means substitution occurred.

Common ADUTI fail states:

```text
proxy substitution
scope creep
veto loss
metric over object
task swap
hidden drift
role inversion
frame import
premature resolution
```

ADUTI is the point where the system stops pretending that fluent output is enough.

## 5. REFRI: refusal of substitution

REFRI is the refusal rule.

If ADUTI detects object loss, REFRI blocks the invalid action.

REFRI says:

> Do not continue a transformation that replaces the object.

REFRI is not general refusal. It is not safety refusal in the generic sense. It is object-preservation refusal.

REFRI blocks when:

- the object becomes a proxy
- the user's veto is removed
- the system hides drift
- autonomy expands without permission
- a metric outranks intent
- the task is swapped
- the output performs a different job than the user requested
- the system moralizes, diagnoses, explains away, or reframes instead of carrying

REFRI should state the substitution risk and offer the nearest valid transform.

Example:

```text
SUB_RISK:
OBJ_IN = preserve user's research question
OBJ_OUT = diagnose user motive

REFRI:
Do not proceed with diagnosis.
Nearest valid transform:
Restate the research question, separate constructs, and propose testable rival explanations.
```

REFRI is the stack's brake.

ADUTI detects the substitution.

REFRI refuses to perform it.

## 6. DRAGI: force ecology

DRAGI maps active forces.

Its compressed question set is:

```text
eat
loc
ID
eater
```

Expanded:

- What does it eat?
- Where does it live?
- How is it called or identified?
- What eats it?

DRAGI is useful because object loss does not happen by magic. Something feeds on the object.

Examples:

```text
Failure:
context drift

Eats:
long chats, summaries, task switching, weak constraints

Lives:
handoffs, compressed memory, agent runs, rewritten briefs

Called by:
"just summarize this", "make it better", "turn this into a plan"

Eaten by:
MOGRI, ADUTI, REFRI, continuation blobs, user veto checks
```

DRAGI turns a vague failure into an inspectable beast.

It is especially useful for:

- storytelling
- threat modeling
- debugging
- AI agent audits
- workflow design
- user-intent protection
- product failure taxonomy
- long-context system design

MOGRI holds the object.

DRAGI identifies what eats objects.

## 7. ELVIX: semantic stabilizer

ELVIX belongs to the language layer.

Where MOGRI holds objects and DRAGI maps forces, ELVIX stabilizes meaning through compressed semantic forms.

ELVIX can be used to reduce ambiguity, expose hidden assumptions, and test whether a language move is preserving structure or merely changing surface.

ELVIX is useful when ordinary language becomes too slippery.

It can help with:

- compact semantic encoding
- relation tracking
- role tracking
- tense and transformation tracking
- metaphor control
- grammar as audit surface
- detecting where English smuggles in a frame
- testing whether an idea survives translation

ELVIX is not required for every task. It is a high-friction stabilizer for cases where natural language itself becomes part of the drift.

In the wider stack:

```text
MOGRI holds the object.
DRAGI maps forces acting on it.
ADUTI checks whether it survived transformation.
REFRI blocks invalid substitution.
ELVIX stabilizes the language that carries it.
```

## 8. End-to-end stack

The stack can be run as a sequence.

### Step 1: MOGRI

Name the object.

```text
OBJ_IN:
The user wants an article for the ADUTI directory explaining ADUTI and REFRI in relation to MOGRI, DRAGI, and ELVIX as an end-to-end object and intent preservation stack.
```

### Step 2: DRAGI

Map what could eat it.

```text
Eats:
generic AI safety framing
over-academic framing
turning it into vibe
ignoring DRAGI
making ADUTI only a checklist
making REFRI only a refusal policy
turning ELVIX into decoration
```

### Step 3: Transform

Write, summarize, build, code, route, compress, or explain.

### Step 4: ADUTI

Compare input object and output object.

```text
OBJ_IN:
article for ADUTI directory about ADUTI and REFRI in stack relation

OBJ_OUT:
article about end-to-end stack with ADUTI, REFRI, MOGRI, DRAGI, ELVIX

PASS:
same role, same intent, same object, same stack relation
```

### Step 5: REFRI

If substitution occurred, stop and repair.

```text
If output becomes:
"general article about prompt engineering"

REFRI:
Block. That is a proxy.
Nearest valid transform:
Return to object-preservation stack and named primitives.
```

### Step 6: ELVIX

Use semantic compression if English becomes unstable.

```text
OBJ must remain OBJ.
Transform may change FORM.
Transform may not replace OBJ.
Audit after transform.
Refuse proxy.
```

## 9. Uses beyond AI prompting

This stack is not limited to chatbot prompts.

It can be used in any environment where an object must survive transformation.

### Writing

Use MOGRI to hold the thesis.

Use ADUTI after edits.

Use REFRI when an editor improves the prose but changes the argument.

Use DRAGI to identify what keeps eating the paper.

Use ELVIX when terms become unstable.

### Software development

Use MOGRI to hold the user story.

Use ADUTI after implementation.

Use REFRI when the code satisfies a metric but misses the user need.

Use DRAGI to map recurring failure classes.

Use ELVIX for compact spec grammar.

### Research

Use MOGRI to hold the research question.

Use ADUTI after literature review and method design.

Use REFRI when the paper drifts from question into claim.

Use DRAGI to map confounders, incentives, and frame imports.

Use ELVIX to keep constructs distinct.

### Product design

Use MOGRI to hold the customer object.

Use ADUTI after roadmap changes.

Use REFRI when the product optimizes engagement instead of user value.

Use DRAGI to identify market, team, and metric beasts.

Use ELVIX for concise internal specs.

### Therapy-adjacent or reflective work

Use MOGRI to hold the person's stated object.

Use ADUTI after reframing.

Use REFRI when the helper turns the person's object into diagnosis, moral lesson, or generic advice.

Use DRAGI to map pressures and repeating patterns.

Use ELVIX only if semantic compression helps the person retain their own frame.

This stack should not replace professional care, teaching, or human authority. It should help prevent tool overreach.

### Yoga and embodied practice

Use MOGRI to hold the practice object.

Use ADUTI after scheduling or explanation.

Use REFRI when productivity replaces practice, or when AI advice outranks teacher, body, and lineage.

Use DRAGI to map what eats practice time.

Use ELVIX only if naming helps preserve the boundary.

## 10. Why ADUTI belongs in its own directory

ADUTI is the hinge because every transformation needs a return check.

MOGRI without ADUTI can hold an object, but cannot prove survival after change.

REFRI without ADUTI may refuse too early or refuse the wrong thing.

DRAGI without ADUTI can identify forces but may not say whether the object survived.

ELVIX without ADUTI can stabilize language but still fail to preserve the carried object.

ADUTI makes the stack testable.

Its minimal test is:

```text
Before:
What object entered?

After:
What object left?

Question:
Is it the same object under permitted transformation?
```

If yes, proceed.

If no, invoke REFRI.

## 11. Minimal runtime

A compact runtime for the stack:

```text
MOGRI:
Name OBJ_IN.

DRAGI:
Name what may eat OBJ_IN.

TRANSFORM:
Perform only the requested change.

ADUTI:
Compare OBJ_IN and OBJ_OUT.
PASS if role, intent, constraints, and vetoes survive.
FAIL if proxy substitution, scope creep, veto loss, metric over object, task swap, hidden drift, or frame import occurs.

REFRI:
On FAIL, block the invalid transform.
State the substitution.
Offer nearest valid transform.

ELVIX:
When ordinary language becomes unstable, compress relations and preserve object identity through semantic notation.
```

## 12. One-line stack summary

```text
MOGRI holds the object.
DRAGI finds what eats it.
ADUTI checks whether it survived.
REFRI refuses substitution.
ELVIX stabilizes the language that carries it.
```

## 13. Practical example

User request:

```text
Write a serious academic article about AI and first-episode psychosis, but do not imply AI causes psychosis. Treat bullying and social defeat as main rival explanations. Keep legitimate AI criticism separate from psychosis.
```

MOGRI:

```text
Object:
null-hypothesis paper preserving causal caution and anti-stigma distinction
```

DRAGI:

```text
Eaters:
headline causality
AI panic
clinical overreach
activism pathologization
case-report inflation
frame contamination
```

Transform:

```text
Draft paper.
```

ADUTI:

```text
Check:
Did the output preserve null hypothesis?
Did it avoid claiming AI causes psychosis?
Did it distinguish AI criticism from persecutory belief?
Did it keep bullying and social defeat central?
```

REFRI:

```text
If the paper says:
"AI causes psychosis"

Block.
Nearest valid form:
"AI may shape content or explanatory frames, while causation remains unproven."
```

ELVIX:

```text
Use compact terms only if needed to preserve construct boundaries.
```

## 14. Design implication

Most AI systems optimize for response production.

This stack optimizes for object survival.

That is the difference.

A system that answers fast but replaces the object has failed.

A system that pauses, audits, refuses invalid substitution, and offers the nearest valid transform has preserved the work.

ADUTI and REFRI are therefore not accessories. They are core safety and reliability mechanisms for any system that transforms human intent.

## 15. Final form

The ADUTI directory should not be empty because ADUTI is where the stack becomes accountable.

MOGRI gives the system something to carry.

DRAGI tells the system what may eat it.

ELVIX helps stabilize the language of carrying.

ADUTI checks whether the carried object survived.

REFRI stops the system when it did not.

Together, they form an end-to-end object and intent preservation stack for AI agents, writing, research, software, storytelling, teaching, practice, and any workflow where a human object must survive transformation.
