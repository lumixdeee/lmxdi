# From Markdown to Governed Deployment

## ADUTI, REFRI, MOGRI, DRAGI, and ELVIX for legal, audit, evidence, compliance, and HCI teams

### 1. Why this document exists

This document is for people whose job is not to build the cleverest model.

It is for people who must answer questions like:

- What did the user ask for?
- What did the system do to that request?
- What evidence was used?
- What changed between input and output?
- Who approved the change?
- What was refused?
- What was escalated?
- Can the organisation reconstruct the event later?
- Can the user understand what happened to their object?
- Can legal, audit, records, product, and engineering teams rely on the same event history?

The stack described here takes five primitives:

- MOGRI
- DRAGI
- ADUTI
- REFRI
- ELVIX

and translates them into deployable governance controls for AI workflows.

The short form:

```text
MOGRI records the object.
DRAGI maps what may eat it.
ADUTI checks whether it survived transformation.
REFRI stops invalid substitution.
ELVIX stabilizes language where ambiguity creates legal or user risk.
```

The goal is not to add more paperwork.

The goal is to prevent silent substitution.

---

## 2. The compliance problem

AI systems transform objects.

In legal, audit, records, customer support, HR, healthcare, finance, and public-sector settings, an object may be:

- a complaint
- a claim
- a consent
- a contract clause
- a medical note
- a legal instruction
- a policy rule
- a risk assessment
- an evidence item
- a regulator request
- a user appeal
- a disciplinary record
- an incident report
- a customer vulnerability marker
- a human decision awaiting review

A model or agent may summarize, classify, route, translate, rewrite, extract, compare, redact, recommend, or escalate that object.

The risk is not only that the output is wrong.

The deeper risk is that the object changes identity during the workflow.

Examples:

```text
A complaint becomes sentiment.
A legal instruction becomes advice.
A consent becomes assumed permission.
A user appeal becomes a fraud signal.
A medical history becomes a risk score.
A disputed fact becomes accepted fact.
A document summary becomes treated as the document.
A policy exception becomes routine routing.
A human veto disappears inside an agent handoff.
```

This is where legal, audit, and HCI concerns meet.

If the system cannot preserve the object, it cannot preserve accountability.

---

## 3. The stack in compliance language

### MOGRI: object record

MOGRI is the authoritative carried object.

In deployment, MOGRI becomes an object card:

```text
object_id:
object_type:
source_actor:
source_time:
source_channel:
jurisdiction:
legal_basis_or_policy_basis:
user_intent:
permitted_transformations:
forbidden_transformations:
human_vetoes:
retention_class:
evidence_links:
current_status:
```

MOGRI is not just a label. It is the anchor for the workflow.

It tells the system:

```text
This is what must not be silently replaced.
```

### DRAGI: risk ecology

DRAGI maps what can consume, distort, or replace the object.

DRAGI asks:

```text
What does it eat?
Where does it live?
How is it called or identified?
What eats it?
```

In compliance terms, DRAGI becomes a risk register for object loss.

Example:

```text
Risk:
summary becomes evidence

Eats:
long documents, executive pressure, dashboard metrics, missing source links

Lives:
case management systems, audit packs, email summaries, board reports

Called by:
"just give me the key points", "make this digestible", "extract action items"

Eaten by:
source binding, hash records, ADUTI object comparison, mandatory citation to record ID
```

DRAGI helps teams stop treating failures as one-off incidents.

It turns them into recurring risk classes.

### ADUTI: audit after transformation

ADUTI is the post-transform audit.

It compares:

```text
OBJ_IN
TRANSFORM
OBJ_OUT
```

ADUTI asks whether the output preserved:

- object identity
- user intent
- authority boundary
- evidence link
- consent boundary
- legal basis
- policy basis
- human veto
- permitted scope
- required escalation path

ADUTI is where a system records that the object survived, or did not.

ADUTI events should be generated after every material AI transformation.

### REFRI: refusal and hold state

REFRI is the refusal rule.

When ADUTI detects substitution, the system must not continue as if nothing happened.

REFRI can trigger:

- stop
- hold
- escalate
- ask human reviewer
- request source document
- request consent
- revert to prior object
- produce a substitution notice
- block automated action

REFRI is not generic refusal. It is a targeted control against object substitution.

Example:

```text
ADUTI finding:
The model changed a disputed allegation into an accepted fact.

REFRI action:
Block downstream decision.
Route to human reviewer.
Attach source records and substitution notice.
```

### ELVIX: semantic stabilizer

ELVIX is the language control layer.

It is useful where ordinary wording creates legal, operational, or user-interface risk.

ELVIX can stabilize:

- definitions
- roles
- permissions
- tense
- source status
- assertion status
- disputed versus accepted facts
- user intent versus system inference
- human decision versus AI recommendation
- evidence versus summary

ELVIX is especially useful in regulated workflows where small language shifts create large consequences.

Example:

```text
Not stable:
"The customer admitted fraud."

Stable:
"The customer used wording that the fraud model classified as suspicious. No admission is recorded."
```

---

## 4. From .md to deployed benefit

A Markdown file does not create benefit by itself.

It becomes useful when converted into controls, interface states, logs, tests, and governance routines.

The route is:

```text
.md principle
-> workflow object
-> runtime event
-> audit record
-> user-facing state
-> refusal rule
-> dashboard metric
-> governance review
```

The job is to turn the stack into operational artifacts.

---

## 5. The minimum deployable set

A team can start with six files and one middleware hook.

### 1. OBJECT_CARD.md

Defines the object being carried.

```text
object_id:
object_type:
owner:
source:
jurisdiction:
user_intent:
permitted_transformations:
forbidden_transformations:
vetoes:
evidence_refs:
retention_rule:
```

### 2. DRAGI_RISK_REGISTER.md

Lists the ways this object may be eaten.

```text
risk_id:
risk_name:
eats:
lives:
called_by:
eaten_by:
control_owner:
severity:
review_cycle:
```

### 3. TRANSFORM_EVENT.json

Created whenever AI transforms the object.

```json
{
  "event_id": "",
  "object_id": "",
  "timestamp_utc": "",
  "actor_type": "human|model|agent|tool",
  "model_or_tool": "",
  "transform_type": "",
  "input_refs": [],
  "output_refs": [],
  "prompt_template_id": "",
  "retrieval_refs": [],
  "human_approver": "",
  "policy_context": ""
}
```

### 4. ADUTI_REPORT.md

Compares before and after.

```text
object_id:
transform_event_id:
obj_in_summary:
obj_out_summary:
identity_preserved: yes|no|uncertain
intent_preserved: yes|no|uncertain
evidence_preserved: yes|no|uncertain
scope_preserved: yes|no|uncertain
vetoes_preserved: yes|no|uncertain
substitution_detected:
required_action:
reviewer:
```

### 5. REFRI_HOLD_NOTICE.md

Generated when substitution is detected.

```text
hold_id:
object_id:
trigger:
substitution_type:
downstream_action_blocked:
human_review_required:
source_records_needed:
nearest_valid_transform:
```

### 6. ELVIX_TERM_MAP.md

Defines sensitive terms.

```text
term:
allowed_meaning:
forbidden_meaning:
source_of_definition:
examples:
review_owner:
```

### 7. Middleware hook

The middleware hook sits between the application and the model or agent framework.

It does four things:

1. attaches the object card
2. records the transform event
3. runs ADUTI comparison
4. invokes REFRI when substitution is detected

This can be deployed before model replacement, before agent redesign, and before full enterprise AI governance maturity.

---

## 6. Where to deploy first

Do not begin everywhere.

Begin where object substitution is costly and visible.

Good first pilots:

### Legal intake

Object:
client question, instruction, document, or claim.

Risk:
the model turns instruction into advice, summary into fact, or missing context into certainty.

Benefit:
better record of what was asked, what was answered, and what remained unverified.

### Customer complaints

Object:
complaint, harm, requested remedy, supporting evidence.

Risk:
the system turns a complaint into sentiment, churn risk, or ticket category.

Benefit:
fewer escalations caused by users feeling unheard or misrepresented.

### HR investigations

Object:
allegation, response, witness note, policy issue.

Risk:
the system collapses disputed facts into a single narrative.

Benefit:
better separation of allegation, evidence, inference, and decision.

### Insurance or benefits claims

Object:
claim, entitlement basis, submitted evidence, policy rule.

Risk:
summary replaces evidence or automated routing hides an exception.

Benefit:
stronger appeal record and review trail.

### Healthcare administration

Object:
patient request, referral note, symptom report, appointment issue.

Risk:
AI output sounds clinical while evidence status is weak.

Benefit:
better boundary between recorded patient statement, system extraction, and clinician decision.

### Public-sector casework

Object:
citizen request, eligibility question, uploaded evidence, appeal.

Risk:
AI routing buries rights, exceptions, or human-review needs.

Benefit:
stronger procedural fairness and better audit replay.

---

## 7. HCI deployment

This stack must be visible to humans in the interface.

Not all logs should be shown, but object state must be legible.

Useful interface states:

```text
Object captured
Object transformed
Object under audit
Object preserved
Object changed
Object held for review
Evidence missing
Human approval required
Summary not source
Decision not yet made
```

The user should be able to see when a summary is not the evidence, when an AI recommendation is not a decision, and when a human reviewer is needed.

For staff, the interface should show:

- object ID
- current status
- source record
- last AI transformation
- ADUTI pass or fail
- REFRI hold state
- missing evidence
- human reviewer
- next valid action

This is not only compliance. It is interaction design.

Users trust systems more when they can see what happened to their object.

---

## 8. Records and evidence preservation

A governance layer should preserve:

- source object
- transformed output
- prompt template ID
- model name and version where available
- retrieval references
- tool calls
- timestamp
- actor
- approval state
- refusal state
- hash of source where appropriate
- retention category
- deletion or redaction basis
- jurisdictional context

Sensitive raw content may need secure storage rather than routine logging.

A safer pattern is:

```text
metadata in audit log
content in controlled evidence vault
hash linking both
role-based access
retention policy
redaction workflow
```

This allows replay without spreading sensitive data through every dashboard.

---

## 9. Benefit model

The benefits are practical.

### For legal

- stronger evidentiary trace
- better privilege and confidentiality boundaries
- less confusion between advice, instruction, evidence, and summary
- easier dispute reconstruction

### For compliance

- auditable workflow controls
- better demonstration of human oversight
- stronger policy enforcement
- fewer undocumented AI actions

### For internal audit

- replayable transformation events
- testable control points
- reduced dependence on informal staff memory
- better sampling of high-risk AI use

### For records teams

- object IDs tied to retention rules
- better source-output linkage
- lower risk that summaries become orphan records
- better deletion and preservation decisions

### For HCI and product

- user trust through visible object status
- fewer hidden state failures
- better escalation design
- better distinction between model output and organisational decision

### For engineering

- runtime invariant checks
- structured event logs
- API-level guardrails
- model-agnostic governance layer

### For executives

- lower AI deployment risk
- faster approval of bounded use cases
- better evidence during regulator, customer, or litigation pressure
- practical control without waiting for perfect model interpretability

---

## 10. Metrics

Track benefit using operational measures.

```text
object_survival_rate
substitution_incident_count
reopened_cases_due_to_summary_error
human_override_rate
evidence_missing_rate
REFRI_hold_count
ADUTI_uncertain_count
time_to_audit_reconstruction
time_to_user_explanation
appeal_success_due_to_record_error
staff_confidence_score
user_understanding_score
regulator_response_time
```

The core metric is not model accuracy alone.

The core metric is:

```text
Was the object preserved through the workflow?
```

---

## 11. Thirty-day pilot

### Week 1: choose one workflow

Pick one workflow with real risk and manageable volume.

Define:

- object type
- transformations
- downstream decisions
- human reviewers
- retention rules
- escalation points

### Week 2: create object cards and risk register

Write:

- OBJECT_CARD.md
- DRAGI_RISK_REGISTER.md
- ELVIX_TERM_MAP.md

Do not overbuild. Start with five to ten object-loss risks.

### Week 3: instrument transformations

Add:

- TRANSFORM_EVENT.json
- ADUTI_REPORT.md
- REFRI_HOLD_NOTICE.md

Run the workflow in shadow mode if production integration is not yet allowed.

### Week 4: measure and review

Review:

- substitutions detected
- uncertain cases
- staff friction
- user-facing language
- missing evidence
- time cost
- value of holds

Decision:

```text
expand
revise
pause
retire
```

---

## 12. Sixty-day implementation

After the pilot:

- integrate object IDs into case management
- add role-based access
- add retention mapping
- add source hashes where appropriate
- route REFRI holds to existing review queues
- add dashboard metrics
- train staff on object substitution
- update user-interface copy
- add periodic audit sampling

By day 60, the stack should no longer be a document. It should be a working control layer around one or two real AI workflows.

---

## 13. Ninety-day governance path

By day 90:

- legal owns interpretation boundaries
- compliance owns policy mapping
- internal audit owns testing
- records owns retention and preservation
- product owns interface states
- engineering owns runtime events
- security owns access and evidence vault controls
- business owner owns workflow outcomes

The organisation should be able to answer:

```text
Which AI transformations occurred?
What object did each transformation act on?
What evidence was used?
Did the object survive?
What was refused?
Who approved the next action?
Can the event be reconstructed later?
```

---

## 14. Procurement language

Buyers can require vendors to support object-preservation controls.

Sample requirement:

```text
The system must maintain an object-level audit trail for AI transformations. For each material transformation, the system must record source object identity, transformation type, input references, output references, model or tool identifier, timestamp, actor, evidence references, human approval state, and substitution audit result. The system must support hold or escalation when output object identity, user intent, evidence status, scope, or vetoes are not preserved.
```

Sample HCI requirement:

```text
The interface must distinguish source evidence, AI-generated summary, AI recommendation, human decision, and held state. Users and staff must not be led to treat a summary as the source record or an AI recommendation as a final organisational decision.
```

Sample audit requirement:

```text
The system must support replay of a sampled workflow from source object through transformation events, ADUTI reports, REFRI holds, human approvals, and final disposition.
```

---

## 15. Common objections

### "We already log prompts and outputs."

That is not enough.

Prompt-output logging records text. It does not necessarily record object identity, permitted scope, evidence status, vetoes, or substitution.

### "The model has a system prompt."

A system prompt is not an audit trail.

### "We can review bad cases manually."

Manual review works only when the case is surfaced. ADUTI and REFRI help detect cases before downstream action.

### "This slows deployment."

It may slow unsafe deployment. It can speed safe deployment by giving legal, audit, and product teams a control they can inspect.

### "This belongs in engineering."

It also belongs in legal, compliance, audit, records, HCI, and product. Object substitution is cross-functional risk.

---

## 16. Relationship to existing governance

This stack does not replace:

- legal advice
- records schedules
- security controls
- data protection impact assessments
- model cards
- system cards
- risk registers
- incident response
- human oversight
- procurement controls
- sector-specific regulation

It supplies a missing operational bridge:

```text
How do we know the object survived the AI workflow?
```

That bridge can support AI governance, algorithmic auditing, traceability, lifecycle governance, audit evidence, paradata, and accountability work already discussed in the literature.

---

## 17. What to put in front of stakeholders

Do not begin by showing them lore.

Show them a before-and-after case.

### Before

```text
User submits complaint.
AI summarizes complaint.
Summary routes case.
Original remedy request disappears.
User appeals.
Organisation cannot reconstruct why the request was lost.
```

### After

```text
User submits complaint.
MOGRI object card records complaint, evidence, requested remedy, vetoes.
AI summarizes complaint.
ADUTI compares complaint to summary.
ADUTI detects missing remedy request.
REFRI blocks routing.
Case is held for reviewer.
Interface shows: "summary incomplete, human review required."
Audit log preserves source, summary, detected loss, and action.
```

That is the deployment story.

Not philosophy.

Not branding.

A prevented failure.

---

## 18. Small technical architecture

```text
Application
  -> Object registry
  -> AI transformation service
  -> Transform event logger
  -> ADUTI comparator
  -> REFRI policy engine
  -> Evidence vault
  -> Case management system
  -> Audit dashboard
  -> User and staff interface states
```

This can be added as middleware.

It does not require owning the foundation model.

It does not require perfect interpretability.

It does require disciplined object records and event logs.

---

## 19. Why this matters before more autonomous AI

As AI systems gain longer memory, tool use, agent routing, and self-modifying workflows, the risk shifts.

The old question was:

```text
Did the model answer correctly?
```

The new question is:

```text
Did the system preserve the object while acting across time, tools, memory, and authority boundaries?
```

Legal and audit teams cannot wait until autonomy is mature before asking this question.

By then, the workflow may be too complex to reconstruct.

Object preservation needs to be upstream.

---

## 20. Final summary

The stack turns a Markdown idea into deployable governance by converting concepts into artifacts:

```text
MOGRI -> object card
DRAGI -> risk register
ADUTI -> transformation audit
REFRI -> refusal and hold state
ELVIX -> semantic control map
```

It creates benefit when embedded into:

- model wrappers
- agent frameworks
- case management systems
- audit dashboards
- user interfaces
- review queues
- procurement terms
- records policies

The promise is practical:

```text
Do not let AI workflows silently replace the thing a human gave you.
Record it.
Transform it only within scope.
Audit the result.
Refuse substitution.
Preserve evidence.
Show humans what happened.
```

---

## Further reading

Ahmad, S., Harbola, A., Sachdeva, S., & Yadav, B. K. (2026). Generative AI in enterprise IT implications for audit evidence, assurance, and governance. EDPACS. https://www.tandfonline.com/doi/abs/10.1080/07366981.2026.2633846

Bommarito, J., & Katz, D. M. (2025). Governing AI Agents: Risk, Compliance, and Accountability in Law and Finance. SSRN. https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5911464

Cameron, S., Franks, P. C., & Huvila, I. (2025). Navigating accountability: the role of paradata in AI documentation and governance. Journal of Documentation. https://scholarworks.sjsu.edu/cgi/viewcontent.cgi?article=7269&context=faculty_rsca

Ghosh, O., & Pandey, A. (2026). Accountability, Responsibility, and Liability in AI and Data Ecosystems: Centering Transparency Through End-to-End Governance. IGI Global. https://www.igi-global.com/chapter/accountability-responsibility-and-liability-in-ai-and-data-ecosystems/409345

Lacmanovic, S., & Skare, M. (2025). Artificial intelligence bias auditing: current approaches, challenges and lessons from practice. Review of Accounting and Finance. https://www.emerald.com/raf/article-abstract/24/3/375/1274302

Leon, M. (2026). Lifecycle-Based Governance to Build Reliable Ethical AI Systems. Systems Research and Behavioral Science. https://onlinelibrary.wiley.com/doi/abs/10.1002/sres.70014

Rana, R., & Bhambri, P. (2026). Ensuring Ethical and Equitable AI: From Bias Mitigation to Algorithmic Auditing. IGI Global. https://www.igi-global.com/chapter/ensuring-ethical-and-equitable-ai/403579

Seet, M. (2026). ISO 42001 and Legal Compliance: A Principled Implementation of the AI Management System. Google Books listing. https://books.google.com/books?id=_H-lEQAAQBAJ

Shahbaz, U. (2025). Transparency through tensions: an integrated multi-method framework for advanced interpretations and robust auditing of artificial intelligence systems. Figshare, Macquarie University. https://figshare.mq.edu.au/ndownloader/files/59675438
