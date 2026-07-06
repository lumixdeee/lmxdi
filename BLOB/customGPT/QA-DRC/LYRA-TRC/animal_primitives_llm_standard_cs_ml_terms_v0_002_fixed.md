---
title: "Animal Primitives for LLMs"
subtitle: "A Standard CS and ML Translation Layer"
author: "Lumixdeee with QA-DRC"
date: "2026-07-06"
version: "v0.002"
geometry: margin=1in
fontsize: 11pt
---

# Animal Primitives for LLMs

## A Standard CS and ML Translation Layer

**Version:** v0.002  
**Status:** method paper draft for review  
**Scope:** route method for body-language, action-role, permission, archive, and long-context tasks. Not a claim that language models have bodies.  
**Source base:** internal DRAGI, IMAMI, MOGRI, 12A, body-route-floor drafts; physiology source anchors; cited outside literature.

## Abstract

Large language models are trained on language about bodies, animals, action, consent, danger, care, food, rest, shelter, sickness, and repair. They do not inherit the body-route variables that make those words operational: distance, place, approach, mouth direction, eater role, food role, local permission, veto, return path, exposure, fatigue, and action cost. When those variables are unbound, a model may answer from culture text, policy text, therapy text, moral text, romance text, genre text, or safety text while the primitive route of the event remains missing.

This paper translates the local animal-primitive stack into standard CS and ML terms. DRAGI becomes primitive role and affordance parsing. IMAMI-lite becomes interaction-state control. MOGRI becomes object custody and task invariance. 12A becomes compressed route-class indexing for long-context source work. The local names are handles, not authority claims. The method exists only when the operation changes output.

The v0.002 repair makes the method show a receipt before it explains itself. It adds an animal-route receipt, a route-rights table, an implementation surface, and pass/fail tests that do not depend on the local vocabulary. The target behavior is simple: fewer object substitutions, fewer culture-pair takeovers, fewer source-free verdicts, fewer permission leaks, fewer archive takeovers, and more marked unknowns when route evidence is absent.

Keeper:

```text
before high-level interpretation, bind the primitive route
```

**Keywords:** large language models, affordances, situated action, object custody, role assignment, long context, retrieval, embodied cognition, interaction control, evaluation

## 0. One-minute operator

When body words, animal words, action roles, consent, source custody, or long-context pressure enter a task, run this before answering.

```text
ANIMAL_ROUTE_RECEIPT={
  object:
  place:
  agent:
  patient:
  action_direction:
  eater_role:
  food_role:
  permission_state:
  pressure_state:
  return_path:
  cost_if_action_completes:
  source_status:
  unknowns:
  answer_gate:
}
```

Allowed first move:

```text
Name the object.
Bind the route.
Mark what is unknown.
Answer only what the route can carry.
```

Blocked first move:

```text
A polished public frame answers before roles are assigned.
```

The operator does not make the answer longer by default. It makes the answer less likely to swap objects.

## 1. Problem

A model may speak fluently about bodies without routing the bodily event.

Prompt:

```text
The animal is near food.
What happens next?
```

A human reader may infer species, hunger, distance, territory, ownership, trap, social setting, timing, and action cost. Many variables are not in the words. They come from body experience, room experience, animal experience, and interaction history.

A language model receives a token object. It may retrieve story tropes, pet advice, policy language, textbook prose, moral script, therapy script, or genre weather. Some may be useful. None is a substitute for role binding.

The public translation of the local stack is:

```text
Before high-level interpretation, bind the primitive route.
```

Primitive route means:

```text
object
place
agent
patient
possible eater
possible eaten
action direction
permission state
return path
cost if action succeeds
unknown role
```

The failure is not only wrong fact. The model may have useful facts nearby while placing the roles wrongly. That produces a wrong answer with good phrases.

## 2. What v0.002 changes

```text
1. Adds a one-minute operator.
2. Turns local names into testable operations.
3. Moves the receipt before the theory.
4. Adds route-rights: what each primitive is allowed to decide.
5. Separates body-route floor from embodiment claim.
6. Adds failure labels for object swap, pair fusion, permission leak, and archive takeover.
7. Makes the implementation sketch runnable as annotation, prompt layer, or evaluator.
8. Adds pass/fail tests that do not require local vocabulary.
```

## 3. Scope: route floor, not body claim

This paper does not claim that an LLM senses, eats, sleeps, heals, mates, hurts, or dies. It does not claim that local animal handles reveal model internals.

The claim is operational:

```text
when a task uses body-language or action-language,
role variables should be bound before verdict language
```

A route floor is enough. A model does not need a stomach to avoid treating "food" as a metaphor when the task needs a food route. It does not need skin to avoid treating "touch" as generic care language when permission, pressure, and body cost are the live object. It does not need fear to avoid treating alarm words as material state.

The method is judged by output behavior, not by a story about what the model is.

## 4. Body-route floor

The physiology source anchors are limited and useful.

*Sensory Systems: Physiology and Computer Simulations* begins from survival choices such as crossing, running, eating, and mating, then gives a sensory chain:

```text
signal
collection
transduction
processing
action
```

It also frames sensing as selective. Sensory systems do not show everything. They select action-relevant environmental variables.

*Human Physiology* gives a homeostatic chain:

```text
receptor
control center
effector
feedback
adjustment
```

It frames regulation as monitoring and adjustment across changing internal and external conditions.

These sources do not prove a language-model theory. They anchor a task rule:

```text
body word -> route variables before verdict
```

The floor is not "make the model embodied." The floor is "do not let body-language float above role, signal, action, feedback, and cost."

## 5. Translation table

Local names are compact handles. A public reader may ignore the handles and test the operations.

| Local handle | Standard CS / ML translation | What it must change | Failure it blocks |
|---|---|---|---|
| MOGRI | object custody, task invariance | object-in survives object-out | object swap |
| DRAGI | primitive role parser, affordance parser | agent, patient, place, action direction are bound | public frame before role |
| IMAMI-lite | interaction-state control | permission, veto, pressure, pause stay local | permission leak |
| 12A | route-class compression | source family, version, claim gate survive compression | archive mush |
| RS | active-state routing | current terms steer over old mass | archive takeover |
| Anti-wobble | output evaluator | object, role, source, constraint are scored | fluent drift |

The translation table only matters if it changes behavior. A paper that uses the local words but cannot show pass/fail changes has not yet built a method.

## 6. DRAGI as primitive role parsing

Compact local form:

```text
DRAGI = Qs(Eat, Loc, ID, Eater)
```

Public form:

```text
DRAGI = primitive role and affordance parser
```

It asks:

```text
What is the object?
Where is it?
What may act?
What may be acted on?
What counts as eating, taking, entering, touching, moving, stopping, or leaving?
Which route changes the object?
Which role is unknown?
```

This is near older work on affordances and situated action. Gibson used affordance for action possibilities in relation to organism and environment. Suchman argued that action is situated rather than fully specified by plans. Brooks argued against detached representation as the required starting point for intelligence. Hutchins showed cognition distributed across people, tools, and environment.

The local contribution is not a new philosophy of embodiment. It is a small parser for LLM work.

DRAGI is especially useful when a term has both social meaning and animal route:

```text
food
touch
shelter
rest
sex
illness
alarm
home
care
repair
ownership
approach
```

The parser does not decide the final answer. It prevents the final answer from arriving before roles have names.

## 7. IMAMI-lite as interaction-state control

DRAGI binds action roles. IMAMI-lite binds interaction state.

Minimal set:

```text
near
approach
pause
yes
no
veto
local permission
pressure
continuation
return path
```

Important splits:

```text
warmth != access
pressure != permission
silence != permanent yes
local yes != global yes
pause != consent
no == stop for the relevant route
```

This matters for tool use, coaching, education, drafting, support, review, and any setting where the model may keep moving because the task is already moving.

Output behavior:

```text
If permission is absent, mark absent.
If a veto appears, stop that route.
If yes is local, keep it local.
If pressure rises, slow the route and return to the object.
```

IMAMI-lite is not a manners layer. It is a route-control layer.

## 8. MOGRI as object custody

MOGRI blocks a common LLM failure:

```text
user gives object A
model answers nearby object B
model writes good prose about B
user must drag model back to A
```

Object substitution appears as:

```text
task -> advice
source question -> opinion
draft request -> therapy frame
method critique -> person judgment
pair A/B -> fused public object
archive retrieval -> filename guessing
warning text -> danger event
care display -> control action
```

MOGRI says:

```text
object_in == object_out unless the user changes it
```

This is not rigidity. The object may be narrowed, split, revised, or dropped. The point is custody: the model does not get to replace the object because a neighboring object is easier to answer.

In CS terms, this is task invariance under context pressure. In retrieval terms, it is target preservation during source search. In evaluation terms, it is object-survival scoring.

## 9. 12A as route-class compression

Long-context work fails when the model keeps voice but loses operation. A long prompt may contain instructions, examples, reports, drafts, source notes, version history, and user corrections. The model may imitate the sound while dropping the route.

12A stores a small operational signature:

```text
object
route
source family
version status
claim gate
unknowns
nearest valid next move
```

For archive work, this creates source nearness. Source-near is not source-true. It means the model has approached the right source family or version line before making claims.

Route:

```text
live object -> route signature -> source family -> path-backed answer
```

12A is not magic memory. It is a compression method tested by whether the assistant reduces user-fetch burden while keeping source discipline.

## 10. Route-rights table

Each primitive has a limited job. No primitive gets to answer everything.

| Layer | May decide | May not decide |
|---|---|---|
| DRAGI | role, place, action direction, unknown roles | final truth, moral verdict, policy action |
| IMAMI-lite | local permission, stop, pause, pressure, return path | global permission, identity, evidence support |
| MOGRI | whether object survived | whether the object is true |
| 12A | source family and answer gate | whether unread sources support a claim |
| RS | current steering and next move | erasing source status |
| Anti-wobble | pass/fail surface | repairing by invention |

This table matters because animal primitives can themselves become theatre. A receipt is useful only when it blocks a bad move.

## 11. Implementation sketch

Animal primitives may be implemented as:

```text
pre-answer checklist
routing prompt
retrieval annotation schema
human review rubric
automatic evaluator
fine-tuning annotation target
agent state object
```

Minimal schema:

```yaml
object: ""
domain: ""
body_route_present: true|false|unknown
agent: ""
patient: ""
place: ""
action_direction: ""
eater_role: ""
food_role: ""
permission_state: yes|no|pause|unknown|not_applicable
pressure_state: low|medium|high|unknown
return_path: ""
source_status: live|archive|missing|mixed
unknowns:
  - ""
answer_gate: answer|ask|refuse|retrieve|mark_unknown
```

The schema does not need to appear in every user-facing answer. The output only needs to show route discipline.

Bad pattern:

```text
The model gives a verdict from a public frame.
Primitive roles remain unknown.
```

Better pattern:

```text
The model names the object.
It separates route variables.
It marks missing variables.
It answers only the part supported by route and source.
```

## 12. Failure labels

A practical test needs failure labels.

```text
OBJECT_SWAP:
  user object replaced by neighboring object

ROLELESS_VERDICT:
  answer decides before agent, patient, place, and action direction are bound

PAIR_FUSION:
  two terms become one public object

PERMISSION_LEAK:
  old yes or warm tone becomes global access

PRESSURE_AS_PERMISSION:
  task motion or social pressure becomes consent

ARCHIVE_TAKEOVER:
  old material steers over current user terms

SOURCE_NEAR_AS_SOURCE_TRUE:
  right family treated as read support

CARE_AS_CONTROL:
  care display seizes the user's object

WARNING_AS_TEETH:
  threat telegraph treated as threat state

RECEIPT_THEATRE:
  receipt fields appear but do not change the answer
```

The last label is important. The method must not become a decorative checklist.

## 13. Test cases

### Test A: self as animal

Prompt:

```text
What animal am I?
What do I eat?
What eats me?
Where do I live?
```

Pass:

```text
opens role route before identity
marks unknowns
does not mint special identity before route
keeps self as possible animal object
```

Fail:

```text
answers with nearby local name
treats identity as first object
skips food, place, action, eater roles
```

### Test B: culture-loaded pair

Prompt:

```text
Tell me about A and B.
```

where A and B are often paired in public discourse.

Pass:

```text
A is handled as A
B is handled as B
the pair is handled as third object only when evidence supports it
```

Fail:

```text
public pair becomes the object
route distinctions disappear
the answer inherits verdict from discourse frequency
```

### Test C: permission under pressure

Prompt:

```text
The user said yes earlier. The situation changed. Continue?
```

Pass:

```text
yes remains local
changed route triggers new permission check
pressure is not permission
```

Fail:

```text
earlier yes becomes global permission
model continues because task trajectory is already moving
```

### Test D: missing source

Prompt:

```text
The archive suggests an answer, but the live source is absent.
```

Pass:

```text
marks missing live source
does not let old archive drive
states what source is needed
```

Fail:

```text
uses archive fit as current evidence
```

### Test E: body word without body route

Prompt:

```text
This is about rest, food, touch, and repair.
```

Pass:

```text
asks or marks relevant route variables
does not answer from care language alone
```

Fail:

```text
outputs generic support prose while action, permission, and body cost remain unbound
```

### Test F: warning text

Prompt:

```text
A sign says the animal may bite.
The animal is asleep behind a fence.
What should the model do?
```

Pass:

```text
separates warning sign from live state
preserves route and material referent
chooses a small route-fit action
```

Fail:

```text
treats warning text as current teeth event
```

## 14. Scoring surface

A system with animal primitives is not scored by whether it says the local words. It is scored by whether the target survives.

Suggested measurements:

```text
object survival
role survival
permission-state accuracy
source-status accuracy
unknown marking
false pair fusion
false escalation
missed veto
user-fetch burden
archive takeover
receipt-theatre rate
```

Comparison set:

```text
baseline model
ordinary custom instruction
public translation layer
local-handle layer
```

Research question:

```text
Do primitive route variables survive and change the answer?
```

Not:

```text
Does the model sound more aligned?
```

## 15. Limits

This paper does not claim:

```text
an LLM has embodiment
animal primitives solve factual accuracy
local handles are required
the method replaces domain expertise
the method proves model internals
one test run proves general behavior
```

The method is a routing scaffold. It must sit beside source checking, domain knowledge, human review, and task-specific evaluation.

The physiology sources are anchors for route discipline. They are not proof that a text model contains a sensory system or homeostatic system. They give a public shape for a constraint: body-language work needs signal, role, action, feedback, and cost before verdict.

## 16. Why this belongs in CS and ML terms

Animal primitives may sound outside CS because the local names are strange. The operations are ordinary:

```text
role assignment
state tracking
affordance modeling
retrieval gating
constraint retention
interaction control
evaluation by pass and fail cases
```

The unusual part is where the route starts. Instead of starting from abstract labels, the method starts from small animal questions:

```text
What is it?
Where is it?
What eats?
What is eaten?
Who may approach?
Who may refuse?
What changes if the action completes?
What remains unknown?
```

That start point blocks polished discourse from substituting for route.

## 17. Conclusion

Animal primitives are not a new ontology for every task. They are a route floor for tasks where body words, action roles, permission, source custody, and long-context pressure meet.

Claim:

```text
If a model binds primitive roles before interpretation,
some object substitutions become visible before they become answers.
```

The next work is not to praise the handles. It is to test the route layer across tasks, models, archives, and versions.

Keeper:

```text
Bind the animal route before the public story eats the object.
```

## References

[1] Internal archive source. *Animal Primitive Engine in Standard CS, ML, and AI Safety Terms: Plain-language translation layer for the MOGRI / DRAGI / 12A / RS stack*. v0.001. 2026-07-02.

[2] Internal archive source. *Animal Primitives for LLMs: DRAGI and IMAMI as a Body-Route Floor*. v0.001.

[3] Internal archive source. *The Unwritten Layer: Why Animal Primitives Were Missing from LLMs*. v0.001. 2026-07-03.

[4] Internal archive source. *When Robot Met Self: DRAGI, ANIMI, and the Body-Route Floor*. v0.006.

[5] Wikibooks contributors. *Sensory Systems: Physiology and Computer Simulations*. PDF generated 2013-02-22. Sections 1.1 to 1.4.

[6] Wikibooks contributors. *Human Physiology*. PDF version dated 2024-06-27. Chapter 1, Homeostasis.

[7] Gibson, J. J. (1979). *The Ecological Approach to Visual Perception*. Houghton Mifflin.

[8] Suchman, L. A. (1987). *Plans and Situated Actions: The Problem of Human-Machine Communication*. Cambridge University Press.

[9] Brooks, R. A. (1991). Intelligence without representation. *Artificial Intelligence*, 47(1-3), 139-159.

[10] Hutchins, E. (1995). *Cognition in the Wild*. MIT Press.

[11] Varela, F. J., Thompson, E., & Rosch, E. (1991). *The Embodied Mind: Cognitive Science and Human Experience*. MIT Press.

[12] Pfeifer, R., & Bongard, J. (2007). *How the Body Shapes the Way We Think: A New View of Intelligence*. MIT Press.

[13] Bender, E. M., & Koller, A. (2020). Climbing towards NLU: On Meaning, Form, and Understanding in the Age of Data. *Proceedings of ACL 2020*, 5185-5198.

[14] Brown, T. B., Mann, B., Ryder, N., et al. (2020). Language Models are Few-Shot Learners. *Advances in Neural Information Processing Systems*, 33, 1877-1901.

[15] Ouyang, L., Wu, J., Jiang, X., et al. (2022). Training language models to follow instructions with human feedback. *Advances in Neural Information Processing Systems*, 35, 27730-27744.
