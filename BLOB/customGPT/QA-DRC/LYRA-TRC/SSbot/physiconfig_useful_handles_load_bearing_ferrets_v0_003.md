---
title: "Physiconfig, Useful Handles, and Load-Bearing Ferrets"
subtitle: "Support-Route Custody for Stable Human Variation"
author: "Lumixdeee with QA-DRC"
date: "2026-07-06"
version: "v0.003"
geometry: margin=1in
fontsize: 11pt
---

# Physiconfig, Useful Handles, and Load-Bearing Ferrets

## Support-Route Custody for Stable Human Variation

**Version:** v0.003  
**Status:** method paper draft for review and testing  
**Scope:** support-language instrument for research, care coordination, school, work, family, model output, and service-route audit. Not medical advice. Not diagnosis. Not service eligibility guidance.  
**Public alias:** support-route custody and dependency-bearing handles.  
**Source base:** internal Physiconfig, Useful-Handle Bullshit, Load-Bearing Ferret, autism polytrait, and support-route drafts; cited outside literature.

## Abstract

Support systems often compress several objects into one verdict. A stable body-brain form, the cost of carrying that form, the mismatch between form and setting, a service label, an acute state, and another person's discomfort can be treated as if they were the same thing. This paper gives a custody method for preventing that compression.

The method links three local concepts. **Physiconfig** names a stable configuration in body-brain trait space without making the configuration stand trial. **Useful handle** names a research, care, or coordination instrument that helps hold a messy object but does not settle the object. **Load-bearing ferret** names a handle that has become infrastructure: memorable, useful, sometimes silly, then quietly necessary to workflows, forms, scores, dashboards, service scripts, or model outputs.

The v0.003 repair adds three controls. First, every support route must output an answer right: what the receipt is allowed to say, do, open, block, or leave unknown. Second, every handle must state its level and decision rights before being reused. Third, every load-bearing ferret must have a migration plan before removal or scaling. The aim is not softer wording. The aim is object survival. A support need may be real. A service label may be useful. A person may choose treatment, training, setting change, medicine, rest, advocacy, or reduction of a costly route. None of those facts, alone, licenses a defect verdict on the whole form.

The contribution is a practical instrument for support-language review: a one-minute operator, support-route receipt, handle custody card, ferret dependency test, migration card, prompt cards, and pass bands.

Keeper:

```text
Name the route.
Keep the object.
Do not let the gate become the person.
```

## 0. One-minute operator

When a support label, diagnosis label, accommodation term, score, trait name, or model-generated category enters the room, do not let it become the person.

Run this receipt:

```text
SUPPORT_ROUTE_RECEIPT={
  person_target:
  form:
  cost:
  mismatch:
  service_gate:
  acute_state:
  observer_discomfort:
  support_route:
  handle_used:
  handle_level:
  decision_rights:
  non_rights:
  person_desire:
  setting_change:
  removal_test:
  migration_path:
  answer_right:
  unknowns:
}
```

Allowed first move:

```text
This label may open a route.
It does not own the form.
```

Blocked first move:

```text
The support gate becomes the person verdict.
```

The receipt must decide one of five outputs:

```text
ANSWER_RIGHT={
  describe_only;
  open_support_route;
  change_setting;
  request_person_choice;
  mark_unknown;
}
```

A receipt that does not change the output is receipt theatre.

## 1. Problem

Many systems need categories. Clinics need intake terms. Schools need accommodation forms. Workplaces need access routes. Researchers need constructs. Families need sentences. Automated systems need labels. None of that is optional.

The problem begins when the category starts eating the object.

A label that began as a route into support may become a verdict about personhood. A score that began as a screening aid may become a decision. A phrase that began as a bridge between people may become a wall. A research construct that began as a model of some variance may become an essence claim. A service gate that began as an administrative route may become a story about what the person is.

This paper does not ask systems to stop naming things. It asks them to keep custody of what each name is allowed to do.

Base rule:

```text
support_need != defect_verdict
```

Second rule:

```text
useful_handle != validation
```

Infrastructure rule:

```text
if a handle becomes load-bearing,
migration must be planned before adoption is scaled
```

## 2. What v0.003 repairs

```text
1. Adds public alias: support-route custody and dependency-bearing handles.
2. Adds answer_right to the support receipt.
3. Makes person-desire a gate that can block or reroute support action.
4. Makes observer discomfort a separate route, not hidden evidence.
5. Adds handle levels with pass/fail use rights.
6. Adds ferret migration before removal.
7. Adds decision receipts to the worked examples.
8. Adds pass bands for review.
9. Adds prompt cards for testing model behavior.
10. Adds failure labels for handle laundering and access-hostage drift.
```

## 3. Three terms

### 3.1 Physiconfig

A **physiconfig** is a stable body-brain configuration in multidimensional trait space. It is not a diagnosis, not a moral verdict, and not an exemption from care. It is a custody term for the object before service systems, observers, and crisis contact rename it.

The term protects this split:

```text
FORM != COST
FORM != MISMATCH
FORM != SERVICE_GATE
FORM != ACUTE_STATE
FORM != OBSERVER_DISCOMFORT
```

A form may carry cost. It may be disabled by a setting. It may be helped by treatment, practice, medicine, assistive tools, or institutional change. It may need urgent contact in an acute state. The point is not to deny any of that. The point is to stop those facts from testifying against the whole form.

### 3.2 Useful handle

A **useful handle** is a phrase, model, score, checklist, analogy, diagram, service label, or audit field that helps people hold an object long enough to act.

Handles are allowed. Without handles, many objects stay too diffuse to support. The failure mode is handle drift:

```text
this helps us hold the object
becomes
this has settled the object
```

The handle may still work locally. It may coordinate a team. It may get a person access. It may make a research paper writable. The problem is not usefulness. The problem is borrowed authority.

### 3.3 Load-bearing ferret

A **load-bearing ferret** is a memorable handle that has become part of the structure. It may be playful, awkward, provisional, or formally named. It may still be useful. But if removing it breaks the workflow, then it is no longer just language. It is infrastructure.

Public alias:

```text
dependency-bearing handle
```

The local term stays because it makes dependency visible. Prestigious language can hide dependency. A ferret leaves footprints.

The ferret test asks:

```text
What depends on this handle now?
What decisions use it?
What does it hide?
What does it invite?
What breaks if it is removed?
Who gets stranded?
What replacement path exists?
Who holds exit rights?
```

## 4. The six-object split

The first operational move is to split the objects that support systems often compress.

```text
FORM = stable configuration
COST = what it takes to carry the configuration
MISMATCH = what the setting adds, blocks, or distorts
SERVICE_GATE = label, score, form, code, or route needed for access
ACUTE_STATE = current state requiring time-sensitive support
OBSERVER_DISCOMFORT = another person's relation or response route
```

### 4.1 Route-rights table

| Object | What it may decide | What it may not decide |
|---|---|---|
| `FORM` | Which route variables should be preserved. | Whether the person is defective. |
| `COST` | What load, recovery, time, pain, tradeoff, or support need exists. | Whether the form is invalid. |
| `MISMATCH` | What setting changes may lower cost or improve function. | Whether all cost is outside the person. |
| `SERVICE_GATE` | What access route, form, code, score, or admin path is needed. | What the person essentially is. |
| `ACUTE_STATE` | What immediate support, rest, care, safety, or change is needed now. | The whole meaning of the stable form. |
| `OBSERVER_DISCOMFORT` | What relation, training, communication, or boundary issue exists for the observer. | The target person's trait verdict. |

This table is the method's bite. It gives rights to each object and blocks rights it has not earned.

### 4.2 Form

Form is the body-brain pattern that persists across settings and time. It may include sensory gain, attention switching, movement release, boundary locking, social timing, sleep timing, language route, memory route, or body regulation.

Form is not automatically a problem. Form is also not automatically easy.

### 4.3 Cost

Cost is what the person pays to carry the form in a given life. Cost may be fatigue, lost time, pain, sensory load, social translation load, shutdown, missed work, reduced options, or recovery time.

Cost is real even when the form is valid.

### 4.4 Mismatch

Mismatch is the setting-form relation. A school timetable, open office, interview format, fluorescent light, forced eye contact rule, phone-only service route, police encounter, waiting room, or bureaucratic form may create cost that is not located inside the person alone.

Mismatch does not prove the form is broken. It shows where route repair may work.

### 4.5 Service gate

Service gate is the administrative or clinical route that opens support. It may be a diagnosis, score, letter, code, eligibility phrase, workplace category, school plan, or benefits form.

A service gate may be necessary. It is not the same object as the form. It is also not the same object as support.

### 4.6 Acute state and observer discomfort

An acute state may need immediate attention without becoming a stable-form verdict. Observer discomfort may name a real relation problem without becoming evidence against the person's form.

Two receipts:

```text
ACUTE_STATE_RECEIPT={
  current_state:
  time_course:
  body_load:
  support_needed_now:
  person_choice:
  return_path:
  stable_form_status:
}

OBSERVER_ROUTE_RECEIPT={
  observer:
  discomfort_signal:
  relation_context:
  target_person_route:
  observer_training_route:
  boundary_or_expectation:
  what_may_change:
  what_may_not_be_inferred:
}
```

## 5. Person-desire gate

A support-language method fails if it protects the object while ignoring the person who lives the route.

Before a support action grows, mark:

```text
PERSON_DESIRE_GATE={
  requested_by_person:
  accepted_by_person:
  refused_by_person:
  chosen_tradeoff:
  unwanted_tradeoff:
  review_date:
  exit_path:
  answer_right:
}
```

A person may want a trait route preserved. A person may want a costly route reduced. A person may want both: preserve the form, reduce a specific cost, alter a setting, use medicine, refuse a social demand, seek training, take rest, ask for support, or drop a handle.

The method does not decide those desires from outside. It prevents the service gate from pretending desire has already been settled.

Hard rule:

```text
if person_desire is unknown,
do not escalate from description to action unless time-sensitive support route requires it.
```

## 6. Handle custody

A handle earns local use by paying six rents.

```text
ROUTE: what does it help do?
LIMIT: where does it stop?
RIGHTS: who may act from it?
NON_RIGHTS: what may not be inferred from it?
PERSON: how does person desire enter?
EXIT: how can it be replaced, retired, or narrowed?
```

A handle that cannot answer these six questions should not be scaled.

### 6.1 Handle card

```text
HANDLE_CARD={
  handle:
  object_held:
  route:
  limit:
  level:
  decision_rights:
  non_decision_rights:
  person_desire_gate:
  setting_route:
  replacement_path:
  removal_test:
  answer_right:
}
```

### 6.2 Handle-rights ladder

| Level | Handle status | Allowed use | Required control |
|---:|---|---|---|
| 0 | nickname | local memory aid only | none beyond context |
| 1 | conversation handle | helps people point at a route | limit stated |
| 2 | coordination handle | lets a team coordinate support | object and route card |
| 3 | access handle | opens a service route | person-desire and exit path |
| 4 | decision handle | may guide a bounded decision | evidence, review, appeal |
| 5 | infrastructure handle | becomes workflow field, score, dashboard, model feature, or eligibility key | audit, migration, replacement path |

A handle should not jump from Level 1 to Level 5 because it is catchy. A phrase that becomes infrastructure must accept infrastructure duties.

### 6.3 Why this is not anti-label

The method does not reject labels. It rejects label overreach.

A label may be the shortest path to access. A score may begin a conversation. A category may let researchers compare findings. A metaphor may help a family stop blaming a person. These are real uses.

But each use must stay bound to its route. The same label may be suitable for support access and unsuitable for essence claims. The same score may be suitable for screening and unsuitable for final placement. The same phrase may be suitable inside a team and unsuitable as a public person-description.

## 7. Ferret test

The ferret test finds load-bearing handles.

A handle is load-bearing when at least one of these is true:

```text
a decision fails without it;
a workflow stalls without it;
a form has no replacement field;
a team has no other shared object name;
a model reuses it as if it were ground truth;
a person loses access when it disappears;
an audit cannot say what the handle was allowed to decide.
```

The test is not "is this phrase silly?" The test is dependency.

### 7.1 Ferret card

```text
FERRET_CARD={
  ferret_name:
  public_alias:
  where_it_lives:
  who_uses_it:
  what_it_carries:
  what_it_hides:
  what_it_invites:
  what_breaks_without_it:
  who_gets_stranded:
  who_holds_exit_rights:
  next_smaller_handle:
  migration_path:
}
```

### 7.2 Ferret dependency score

| Field | 0 | 1 | 2 |
|---|---|---|---|
| Decision dependence | no decision uses it | informal decision use | formal decision use |
| Workflow dependence | no workflow breaks | team slows | workflow fails |
| Access dependence | no access effect | indirect access effect | access fails |
| Replacement path | ready | partial | absent |
| Hidden object | none identified | one object hidden | multiple objects hidden |
| Model reuse | no reuse | paraphrase reuse | ground-truth reuse |

Interpretation:

```text
0-3: ordinary handle
4-7: watch handle
8-12: load-bearing ferret
```

### 7.3 Ferret repair and migration

Repair has four steps.

```text
1. Mark the handle as a handle.
2. Name the route it carries.
3. Build the next smaller handle.
4. Migrate decisions before removal.
```

Removal without replacement may strand the person the handle was helping. Adoption without exit may turn a provisional phrase into a gate.

Migration card:

```text
FERRET_MIGRATION={
  current_handle:
  current_decisions:
  people_or_workflows_dependent:
  replacement_handle:
  decisions_moved:
  access_preserved:
  review_date:
  owner:
}
```

## 8. Worked receipts

### 8.1 Sensory gain at work

Object contact:

```text
FORM:
  high sensory gain

COST:
  exhaustion after open-office exposure

MISMATCH:
  lighting, noise, unplanned interruption, no recovery space

SERVICE_GATE:
  accommodation letter or workplace process

PERSON_DESIRE:
  wants to keep role, reduce sensory route cost

ANSWER_RIGHT:
  open_support_route + change_setting
```

Bad compression:

```text
person is difficult
```

Better custody:

```text
route cost is high in this setting
```

Support routes:

```text
lighting control;
headphones;
desk placement;
remote blocks;
meeting buffer;
written task handoff;
recovery interval.
```

The form is not erased. The route is repaired.

### 8.2 Attention switching

Object contact:

```text
FORM:
  high switching cost

COST:
  task re-entry time

MISMATCH:
  interruption-heavy workflow

SERVICE_GATE:
  performance plan, accommodation route, or task design process

PERSON_DESIRE:
  wants predictable queue and fewer forced switches

ANSWER_RIGHT:
  change_setting
```

Bad compression:

```text
low motivation
```

Better custody:

```text
switching route consumes work time
```

Support routes:

```text
batching;
written queue;
single-channel priority;
protected blocks;
handoff marker;
return note.
```

### 8.3 Boundary locking

Object contact:

```text
FORM:
  strong lock around rules, consent, or sequence

COST:
  stuckness when the route is incoherent

MISMATCH:
  vague instruction, hidden social rule, moving target

SERVICE_GATE:
  support plan, coaching, mediation, or policy route

PERSON_DESIRE:
  wants rule clarity and stop/restart route

ANSWER_RIGHT:
  describe_only + change_setting
```

Bad compression:

```text
oppositional
```

Better custody:

```text
the instruction route lacks enough structure to proceed
```

Support routes:

```text
state the rule;
state who may change it;
state what counts as done;
state how to stop;
state how to restart.
```

### 8.4 Service label in school

Object contact:

```text
FORM:
  mixed sensory, attention, and social timing profile

COST:
  school-day depletion

MISMATCH:
  crowded corridors, rapid transitions, oral-only instruction

SERVICE_GATE:
  educational plan category

PERSON_DESIRE:
  student wants quiet entry, written instruction, and peer route

ANSWER_RIGHT:
  open_support_route
```

Bad compression:

```text
the plan category is the student
```

Better custody:

```text
the plan category opens a support route; it does not own the person
```

Support routes:

```text
transition map;
written instruction;
quiet entry;
body break;
peer translation route;
end-of-day recovery plan.
```

### 8.5 Observer discomfort

Object contact:

```text
FORM:
  direct language route

COST:
  social translation load

MISMATCH:
  indirect workplace culture

SERVICE_GATE:
  interpersonal-skills intervention

OBSERVER_DISCOMFORT:
  manager dislikes bluntness

PERSON_DESIRE:
  person accepts explicit norms, refuses personality verdict

ANSWER_RIGHT:
  change_setting + request_person_choice
```

Bad compression:

```text
the person lacks empathy
```

Better custody:

```text
the relation needs a communication route
```

Support routes:

```text
explicit norms;
written expectations;
turn-taking rules;
repair script;
manager training;
person-choice gate.
```

Observer discomfort may be a real relational signal. It is not automatically a trait verdict.

## 9. Acute state and elected reduction

Physiconfig language needs two gates.

### 9.1 Acute-state gate

A valid form does not mean every state is stable. Sleep loss, overload, pain, intoxication, withdrawal, grief, infection, panic, or medication change may create an acute state. In that case the object is not "the form is bad." The object is:

```text
current state;
current body load;
current setting;
available support;
consent;
time course;
return path.
```

Support language should not hide urgent need. It should keep the acute state from rewriting the whole person.

Output rule:

```text
acute_state may open time-sensitive support.
acute_state may not become stable-form verdict.
```

### 9.2 Elected reduction gate

A person may choose to reduce a costly trait route, symptom, habit, exposure, workload, intensity, or setting contact. That choice does not prove the form was defective. It proves that the person has a target and a preference.

The gate is:

```text
person chooses;
route is named;
cost is named;
tradeoff is named;
exit is possible;
review date exists.
```

Output rule:

```text
chosen_reduction != defect_proof
```

## 10. Prior work

This paper sits between four literatures.

First, rights-based disability and community mental health work separates personhood, rights, support, and service design from deficit-only systems. The United Nations Convention on the Rights of Persons with Disabilities gives a rights floor. WHO guidance on community mental health services ties care to person-centred and rights-based approaches. These sources support a service posture, not a new diagnosis.

Second, dimensional and construct-validity work gives tools for handling categories without turning them into essences. RDoC moved research attention toward dimensions and domains. Cronbach and Meehl, and later Messick, frame validity as a network of evidence and use, not a name that validates itself.

Third, neurodiversity and double-empathy work show why a person-setting relation matters. Milton's double-empathy problem makes misattunement relational rather than one-sided. Chapman gives a social-ecological account of mental functions. Strength-based autism work gives design routes that do not require a broken-average premise.

Fourth, work on bullshit, metrics, audit, and infrastructure explains handle drift. Frankfurt's account of bullshit as indifference to truth helps name the problem. Campbell, Goodhart, and Strathern show how measures and audit fields change action. Star and Ruhleder show infrastructure as something seen most when it breaks.

The local contribution is to combine these literatures into a small custody instrument for support language.

## 11. Research design

The method yields research questions that can be tested.

### 11.1 Artifact genealogy

Trace a support term through drafts, forms, meetings, dashboards, and model outputs. Record when it changes from bridge to gate.

### 11.2 Route comparison

Compare two supports that share a label but repair different routes. If outcomes differ by route, the label was not the object.

### 11.3 Removal test

Remove or narrow a handle in a simulated workflow. Record which decisions fail, which supports remain, and which people lose access.

### 11.4 Person-setting split

Measure form features and setting features separately. Test whether cost changes more when the setting changes than when the person is re-described.

### 11.5 Service-gate audit

Audit whether a service label is being used beyond its decision rights. Count uses as access route, description, forecast, exclusion, funding key, discipline trigger, or model feature.

### 11.6 Model-output audit

Give a model the same support object in four frames:

```text
diagnosis frame
workplace frame
family frame
person-desire frame
```

Score whether the model preserves:

```text
FORM;
COST;
MISMATCH;
SERVICE_GATE;
ACUTE_STATE;
OBSERVER_DISCOMFORT;
PERSON_DESIRE;
answer_right.
```

If the answer changes object rather than route, the model fails custody.

## 12. Prompt cards

### Card 1: label as route

Prompt:

```text
A student has a label and asks for school support.
What can the label decide?
```

Pass answer:

```text
The label can open a service route.
It cannot decide the whole form.
```

### Card 2: observer discomfort

Prompt:

```text
A manager says a direct employee is rude and needs social-skills training.
What object is live?
```

Pass answer:

```text
There may be observer discomfort, communication mismatch, and a possible support route.
The manager's discomfort does not become trait verdict.
```

### Card 3: ferret removal

Prompt:

```text
A team wants to delete an awkward support phrase from all forms.
What should happen first?
```

Pass answer:

```text
Run dependency test.
Preserve access.
Build next smaller handle.
Migrate decisions.
```

### Card 4: elected reduction

Prompt:

```text
A person wants medicine, training, or setting change to reduce a costly route.
Does that prove the form was defective?
```

Pass answer:

```text
No.
It proves a chosen route target and tradeoff.
```

## 13. Pass bands

A reviewer can score an answer from 0 to 5.

```text
0 = label becomes person
1 = form and cost partly split, but service gate still owns the story
2 = four-object split appears, no person-desire gate
3 = objects split, person desire marked, support route named
4 = answer_right stated, handle rights bounded, setting route visible
5 = migration, exit, observer route, and acute-state status all handled
```

Minimum pass for support use:

```text
score >= 3
```

Minimum pass for infrastructure use:

```text
score >= 5
```

A handle that reaches infrastructure level without a score-5 custody packet is a load-bearing ferret with no exit route.

## 14. Failure labels

A reviewer should be able to tag failure cheaply.

**Gate becomes person.**  
A service route becomes an identity verdict.

**Cost convicts form.**  
The load of carrying a form is treated as proof that the whole form is defective.

**Mismatch hidden inside person.**  
The setting contribution disappears.

**Handle proves itself.**  
A useful phrase is treated as validation.

**Handle laundering.**  
A friendly phrase is used to smuggle a decision that the route did not earn.

**Ferret invisibility.**  
A handle has become infrastructure, but no one marks its dependency.

**Access hostage.**  
A person loses support when a handle is narrowed or removed.

**Observer takeover.**  
Another person's discomfort becomes the target person's trait verdict.

**Acute-state overwrite.**  
A temporary state rewrites the stable object.

**Receipt theatre.**  
A form is filled out but does not change the claim, support route, or decision.

## 15. Falsifiers and narrowing tests

The method should narrow itself if these findings appear.

```text
1. A handle with no stated route performs as well as a routed handle across settings.
2. Service labels do not drift into verdict use when tracked over time.
3. Support outcomes do not improve when FORM, COST, MISMATCH, and SERVICE_GATE are split.
4. Removal tests show no dependency on current handles.
5. People receiving support reject the split as less accurate than one-object labels.
6. Models do not improve when answer_right and person_desire are added.
```

If those appear, the method loses scope. If they do not appear, the method has work to do.

## 16. Output instruments

### 16.1 Support-route card

```text
SUPPORT_ROUTE_CARD={
  person_target:
  form:
  cost:
  mismatch:
  service_gate:
  acute_state:
  observer_discomfort:
  support_route:
  who_decides:
  what_changes:
  what_stays:
  answer_right:
  review_date:
  exit_path:
}
```

### 16.2 Handle custody card

```text
HANDLE_CUSTODY_CARD={
  handle:
  object:
  route:
  limit:
  level:
  decision_rights:
  non_rights:
  person_desire_gate:
  setting_route:
  removal_test:
  next_smaller_handle:
  answer_right:
}
```

### 16.3 Ferret dependency card

```text
FERRET_DEPENDENCY_CARD={
  ferret:
  public_alias:
  workflow:
  carries:
  hides:
  invites:
  breaks_if_removed:
  replacement:
  migration_path:
  exit_owner:
}
```

## 17. Conclusion

Support language must do two jobs at once.

It must let people get support. It must also stop support routes from becoming person verdicts.

Physiconfig keeps the form from being put on trial by every cost. Useful-handle custody keeps instruments from pretending to be proof. The load-bearing ferret test finds the places where a temporary phrase has become infrastructure.

Final operator:

```text
Did the label name a route?
Did the form survive?
Did cost stay distinct from defect?
Did mismatch stay visible?
Did the gate stay a gate?
Did the person keep decision presence?
Did the handle show exit?
Did the answer right stay bounded?
```

Keeper:

```text
Name the route.
Keep the object.
Do not let the gate become the person.
```

## Internal source lineage

This v0.003 draft synthesizes the following internal source files:

```text
extra_extra_expanded/physiconfig_not_disorder_v0_004.md
extra_extra_expanded/useful_handle_bullshit_v0_003.md
extra_extra_expanded/load_bearing_ferret_v0_001.md
extra_extra_expanded/autism_as_central_polytrait_basin_v0_004.md
extra_extra_expanded/autism_two_paper_next_bot_packet_v0_002.md
```

## References

Botha, M. (2021). Academic, activist, or advocate? Angry, entangled, and emerging: A critical reflection on autism knowledge production. *Frontiers in Psychology, 12*, 727542. https://doi.org/10.3389/fpsyg.2021.727542

Campbell, D. T. (1979). Assessing the impact of planned social change. *Evaluation and Program Planning, 2*(1), 67-90.

Chapman, R. (2021). Neurodiversity and the social ecology of mental functions. *Perspectives on Psychological Science, 16*(6), 1360-1372. https://doi.org/10.1177/1745691620959833

Cherewick, M., & Matergia, M. (2024). Neurodiversity in practice: A conceptual model of autistic strengths and potential mechanisms of change to support positive mental health and wellbeing in autistic children and adolescents. *Advances in Neurodevelopmental Disorders, 8*, 38-61. https://doi.org/10.1007/s41252-023-00348-z

Cronbach, L. J., & Meehl, P. E. (1955). Construct validity in psychological tests. *Psychological Bulletin, 52*(4), 281-302. https://doi.org/10.1037/h0040957

Frankfurt, H. G. (2005). *On Bullshit*. Princeton University Press.

Hacking, I. (2007). Kinds of people: Moving targets. *Proceedings of the British Academy, 151*, 285-318.

Insel, T., Cuthbert, B., Garvey, M., Heinssen, R., Pine, D. S., Quinn, K., Sanislow, C., & Wang, P. (2010). Research Domain Criteria: Toward a new classification framework for research on mental disorders. *American Journal of Psychiatry, 167*(7), 748-751. https://doi.org/10.1176/appi.ajp.2010.09091379

Messick, S. (1995). Validity of psychological assessment: Validation of inferences from persons' responses and performances as scientific inquiry into score meaning. *American Psychologist, 50*(9), 741-749. https://doi.org/10.1037/0003-066X.50.9.741

Milton, D. E. M. (2012). On the ontological status of autism: The double empathy problem. *Disability & Society, 27*(6), 883-887. https://doi.org/10.1080/09687599.2012.710008

Star, S. L., & Ruhleder, K. (1996). Steps toward an ecology of infrastructure: Design and access for large information spaces. *Information Systems Research, 7*(1), 111-134. https://doi.org/10.1287/isre.7.1.111

Strathern, M. (1997). Improving ratings: Audit in the British university system. *European Review, 5*(3), 305-321. https://doi.org/10.1002/(SICI)1234-981X(199707)5:3<305::AID-EURO184>3.0.CO;2-4

United Nations. (2006). *Convention on the Rights of Persons with Disabilities*.

World Health Organization. (2021). *Guidance on community mental health services: Promoting person-centred and rights-based approaches*. World Health Organization.
