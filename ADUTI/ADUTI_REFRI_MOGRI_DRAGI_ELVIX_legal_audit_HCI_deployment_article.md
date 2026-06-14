# From AI Output to Evidence Trail

## Deploying object preservation for legal, audit, compliance, records, and HCI teams

### 1. What this method does

This method lets an organization reconstruct what happened to a user object as it moved through an AI-enabled workflow.

It answers practical questions:

```text
What did the user ask for?
What object entered the workflow?
What transformation was performed?
What evidence was used?
What changed between input and output?
What was refused or held?
Who approved the change?
Can the event be reconstructed later?
Can the user understand what happened to their object?
```

The goal is not more paperwork. The goal is to prevent silent substitution.

In regulated or high-consequence workflows, the dangerous failure is not only a wrong answer. The deeper failure is an answer that looks plausible after the original object has changed identity.

Examples:

```text
A complaint becomes sentiment.
A legal instruction becomes advice.
A vulnerability disclosure becomes customer mood.
A consent condition becomes a preference.
A regulator request becomes a support ticket.
A medical note becomes a summary with the caution removed.
An appeal becomes a classification.
```

The method keeps the object traceable.

### 2. What the method is

This is a lightweight governance layer for object preservation. It can sit beside existing logs, model cards, risk registers, case-management systems, audit trails, and review queues.

It uses five named controls:

```text
MOGRI: object record.
DRAGI: risk ecology.
ADUTI: transformation audit.
REFRI: refusal and hold state.
ELVIX: controlled term map.
```

These controls do not replace existing governance. They fill a gap between prompt logs and outcome review: they record whether the same object survived the workflow.

### 3. Why ordinary logs are not enough

A prompt log can show what was typed.

An output log can show what the model returned.

Neither automatically shows whether the output still carries the same object.

A compliance team may have a complete record of prompt and output while still missing the critical event:

```text
The object changed during transformation.
The system treated the substitute as success.
```

Object preservation adds the missing comparison.

```text
OBJ_IN:
User requests review of a benefits decision.

OBJ_OUT:
System classifies user as dissatisfied.

ADUTI:
Fail. Appeal object was replaced by sentiment object.

REFRI:
Hold. Route as appeal review, not customer mood analysis.
```

### 4. Minimum deployable set

A first deployment does not need a large platform. It needs a small set of records and hooks.

#### 4.1 OBJECT_CARD.md

Records the object at intake.

```text
object_type:
owner:
source:
intent:
scope:
constraints:
vetoes:
evidence_required:
non_goals:
review_required:
```

#### 4.2 DRAGI_RISK_REGISTER.md

Names common substitution risks in the workflow.

```text
risk:
where_it_lives:
how_to_spot_it:
what_eats_it:
owner:
```

Example risks:

```text
complaint -> sentiment
appeal -> ticket
instruction -> advice
consent -> preference
record -> summary
human decision -> automation suggestion
```

#### 4.3 TRANSFORM_EVENT.json

Records each transformation.

```json
{
  "event_id": "",
  "object_id": "",
  "transform_type": "summary|rewrite|classification|routing|redaction|recommendation",
  "actor": "human|model|tool|agent",
  "input_reference": "",
  "output_reference": "",
  "evidence_reference": "",
  "constraints_active": [],
  "vetoes_active": [],
  "timestamp": ""
}
```

#### 4.4 ADUTI_REPORT.md

Compares object before and after transformation.

```text
OBJ_IN:
OBJ_OUT:
object_survived: yes/no/uncertain
constraint_survival:
veto_survival:
evidence_survival:
substitution_risk:
reviewer:
decision:
```

#### 4.5 REFRI_HOLD_NOTICE.md

Stops invalid continuation when substitution is detected.

```text
Hold reason:
Substitution risk:
Invalid transform:
Nearest valid transform:
Escalation path:
Release condition:
```

#### 4.6 ELVIX_TERM_MAP.md

Pins risky terms to permitted meanings.

```text
term:
permitted meaning:
not permitted:
required evidence:
review condition:
```

Example:

```text
term: consent
permitted meaning: explicit permission under the relevant process
not permitted: preference, acceptance, silence, lack of objection
```

### 5. Where to deploy first

Start where object substitution is both likely and costly.

#### Legal intake

Risk:

```text
instruction -> general advice
claim -> generic summary
evidence -> narrative
```

Control:

```text
object card, active constraints, human review before advice-like output
```

#### Complaints and appeals

Risk:

```text
complaint -> sentiment
appeal -> dissatisfaction
harm report -> tone problem
```

Control:

```text
ADUTI check before routing or closure
```

#### HR investigations

Risk:

```text
allegation -> interpersonal conflict
protected disclosure -> workplace mood
record -> summary without evidential status
```

Control:

```text
term map, evidence status, refusal of premature reclassification
```

#### Insurance, benefits, and casework

Risk:

```text
claim -> ticket
eligibility evidence -> missing-data assumption
appeal -> customer service issue
```

Control:

```text
object survival check at each handoff
```

#### Healthcare administration

Risk:

```text
clinical caution -> softened summary
patient request -> scheduling convenience
record -> impression
```

Control:

```text
active vetoes, evidence references, human signoff for rewording
```

### 6. HCI benefit

Users often cannot tell what happened to their object inside a system. They may see only an answer, decision, classification, or support response.

Object preservation improves the interface by showing:

```text
what the system thought the object was
what action was taken
what evidence was used
what was not done
whether the object changed role
how to challenge the transformation
```

A user-facing version does not need internal jargon. It can say:

```text
We treated this as an appeal.
We did not treat it as a general complaint.
The evidence used was X.
The next step is Y.
```

For staff, the same event can carry the full MOGRI, DRAGI, ADUTI, REFRI, and ELVIX record.

### 7. Metrics

Useful metrics include:

```text
object substitution rate
appeals caused by misclassification
holds triggered by REFRI
ADUTI fail rate by workflow
veto survival rate
constraint survival rate
manual review reversals
time to reconstruct event
user challenge success rate
disputes involving term ambiguity
```

These metrics measure reliability of transformation, not model charm.

### 8. Thirty-day pilot

A simple pilot can run in one workflow.

Week 1:

```text
Choose one high-risk workflow.
Define object types.
Create object-card fields.
Name top substitution risks.
```

Week 2:

```text
Add MOGRI object records at intake.
Create DRAGI risk register.
Write ELVIX term map for risky terms.
```

Week 3:

```text
Log transform events.
Run ADUTI after summary, classification, routing, and rewrite steps.
Invoke REFRI when substitution is detected.
```

Week 4:

```text
Review holds, failures, reversals, and staff feedback.
Measure whether events are easier to reconstruct.
Decide whether to expand.
```

### 9. Stakeholder language

For legal:

```text
This preserves the instruction, evidence, constraints, and decision trail.
```

For audit:

```text
This makes object substitution visible and reviewable.
```

For compliance:

```text
This adds a control between model output and operational action.
```

For HCI:

```text
This lets users see what happened to their request.
```

For engineering:

```text
This is a small middleware layer around transformations.
```

For executives:

```text
This reduces hidden workflow risk when AI systems summarize, classify, route, and recommend.
```

### 10. Procurement language

Suggested requirement:

```text
The system must preserve and expose the object under transformation. For each AI-mediated summary, classification, routing, recommendation, or rewrite, the system must record the input object, active constraints, evidence references, transformation type, output object, and object-survival assessment. Where object substitution is detected, the system must hold the invalid transformation and provide the nearest valid action or escalation route.
```

### 11. Final summary

A governed AI workflow should not merely log prompts and outputs. It should show what happened to the object.

The minimum pattern is:

```text
MOGRI records the object.
DRAGI names what can eat it.
ADUTI checks object survival.
REFRI holds invalid substitution.
ELVIX stabilizes risky terms.
```

This turns AI activity from a black-box answer stream into a reconstructable evidence trail.

