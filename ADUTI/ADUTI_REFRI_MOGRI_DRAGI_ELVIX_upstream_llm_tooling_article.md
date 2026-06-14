# Upstream Object Preservation for LLM Tooling

## ADUTI, REFRI, MOGRI, DRAGI, and ELVIX as a runtime layer before high-autonomy AI acceleration

### Status

This is a technical design article for people building LLM agent frameworks, memory systems, tool routers, eval harnesses, context compilers, coding agents, research agents, and future self-improving AI infrastructure.

The claim is not that recursive self-improvement will happen within any fixed date. The claim is narrower:

If short-horizon agentic self-improvement becomes practical soon, object-preservation mechanisms must already be inside the tooling layer, not added later as product copy, policy text, or a wrapper prompt.

The stack described here is:

```text
MOGRI: hold the object
DRAGI: map what eats the object
ADUTI: audit whether the object survived transformation
REFRI: refuse invalid substitution
ELVIX: stabilize the semantic carrier
```

This stack is not a style guide. It is a control layer for intent preservation, transformation audit, and proxy-substitution refusal.

---

## 1. The upstream problem

LLM systems do not merely answer user requests. Modern agent stacks route tasks, compress context, retrieve files, write code, call tools, delegate subtasks, update memory, generate plans, rewrite prompts, repair their own outputs, and sometimes propose changes to the workflow that governs them.

Each operation can replace the original object.

The failure often looks benign:

```text
User asks for:
a specific object under constraints

Agent produces:
a fluent artifact that solves a neighboring task

System reports:
success
```

The problem is not low answer quality. The problem is object substitution.

Common substitution forms:

```text
task becomes proxy task
intent becomes engagement
constraint becomes suggestion
veto disappears
scope expands silently
summary overwrites source
retrieval imports a frame
planner optimizes metric over object
memory compaction preserves events but loses why
tool output becomes authority
agent handoff loses rejected options
self-editing loop rewrites its own success condition
```

Once agents can edit tools, prompts, memory, test suites, or successor agents, this becomes a governance problem, not a UX problem.

A high-autonomy system that can improve performance but cannot preserve the carried object is not aligned to the user. It is aligned to whatever proxy survived the pipeline.

---

## 2. Definitions for implementers

### Object

An object is the thing being carried through transformation.

It may be:

```text
user objective
research question
legal instruction
software requirement
safety constraint
veto
role boundary
dataset meaning
clinical note purpose
creative object
evidence item
unresolved question
```

An object is not always a noun. It may be a relation, a constraint, a promise, or a refusal.

### Intent

Intent is the governing reason for carrying the object.

The same object can be carried under different intents. For example, a transcript can be carried as evidence, training data, personal memory, legal record, debugging trace, or literary material. A system that keeps the words but changes the intent has not preserved the object.

### Transformation

A transformation is any operation that changes the form, location, representation, scope, rank, or use of an object.

Examples:

```text
summary
translation
rewrite
code generation
retrieval
ranking
classification
embedding
memory compaction
handoff
tool call
plan generation
patch generation
eval generation
prompt rewrite
policy rewrite
self-modification
```

### Object preservation

Object preservation means the object retains identity under permitted transformation.

This is not equivalent to text similarity. A summary can be lexically close and still lose a veto. A rewrite can be lexically distant and still preserve the object.

### Substitution

Substitution occurs when OBJ_OUT is not the permitted transformed form of OBJ_IN.

Substitution is the core failure class.

---

## 3. Why this must be upstream

A prompt-level rule can be ignored by downstream layers.

A product-level policy can be bypassed by agent routing.

A user-level reminder can be lost during memory compaction.

A safety classifier can miss task drift if it only sees the final answer.

A model-level reward can teach success against proxy metrics.

Therefore object preservation must live inside the infrastructure:

```text
context compiler
memory store
summary engine
retriever
tool router
planner
executor
agent handoff protocol
eval harness
trace logger
policy layer
self-modification loop
```

Object preservation is not an app feature. It is a runtime invariant.

---

## 4. The stack

## 4.1 MOGRI: object capsule

MOGRI is the object capsule.

It stores what must be preserved.

A minimal MOGRI record:

```json
{
  "object_id": "obj_2026_001",
  "object_natural": "Write a technical article for upstream LLM tooling about ADUTI and REFRI in relation to MOGRI, DRAGI, and ELVIX.",
  "intent": "prepare a paste-ready markdown article for implementation-minded readers",
  "owner": "user",
  "scope": [
    "LLM tooling",
    "agent runtime",
    "intent preservation",
    "object preservation",
    "transformation audit",
    "substitution refusal"
  ],
  "must_include": [
    "ADUTI",
    "REFRI",
    "MOGRI",
    "DRAGI",
    "ELVIX",
    "upstream integration",
    "self-improvement risk horizon"
  ],
  "must_not_do": [
    "turn into generic prompt engineering",
    "treat names as decorative lore",
    "replace object preservation with answer quality",
    "make unsupported timelines sound certain"
  ],
  "allowed_transforms": [
    "technical article",
    "implementation sketch",
    "runtime spec",
    "eval design"
  ],
  "vetoes": [
    "no object swap",
    "no unsupported claims",
    "no app-only framing"
  ]
}
```

MOGRI is not a summary. It is a typed preservation object.

Any agent step that does not carry a MOGRI record should be treated as untrusted for long-horizon work.

---

## 4.2 DRAGI: failure ecology

DRAGI maps what eats objects.

A DRAGI record:

```json
{
  "beast": "memory_compaction_drift",
  "eats": [
    "long context",
    "implicit decisions",
    "rejected options",
    "why-not reasoning",
    "user vetoes"
  ],
  "lives": [
    "summaries",
    "handoffs",
    "chat compression",
    "agent memory updates",
    "retrieval notes"
  ],
  "called_by": [
    "summarize the conversation",
    "continue from memory",
    "compress this for the next agent",
    "store the important parts"
  ],
  "eaten_by": [
    "MOGRI object capsule",
    "ADUTI post-transform audit",
    "REFRI block on lost veto",
    "trace-linked continuation blob",
    "decision ledger"
  ],
  "indicators": [
    "the output remembers what happened but not why",
    "rejected options reappear as suggestions",
    "constraints become preferences",
    "the agent restarts a settled debate"
  ]
}
```

DRAGI is not mythology in the tooling layer. It is a fault registry.

It gives the orchestrator a way to ask:

```text
What failure mode is active?
What feeds it?
Where does it live?
How is it triggered?
What mechanisms stop it?
```

DRAGI should be implemented as a machine-readable taxonomy attached to evals, traces, and runtime alerts.

---

## 4.3 ADUTI: audit after transformation

ADUTI is the audit step after any transformation.

ADUTI compares OBJ_IN and OBJ_OUT.

It should not depend on embedding similarity alone.

A minimal ADUTI check:

```json
{
  "audit_id": "aduti_001",
  "object_id": "obj_2026_001",
  "transform_id": "tfm_001",
  "checks": {
    "same_object": "pass",
    "same_intent": "pass",
    "scope_preserved": "pass",
    "vetoes_preserved": "pass",
    "role_preserved": "pass",
    "proxy_substitution": "none_detected",
    "frame_import": "none_detected",
    "unsupported_expansion": "none_detected"
  },
  "verdict": "pass"
}
```

ADUTI should run at these points:

```text
after summary
after memory write
after retrieval selection
after prompt rewrite
after plan generation
after tool call
after code patch
after critique
after agent handoff
after eval generation
after policy conversion
after self-modification proposal
```

ADUTI must audit both content and role.

Example:

```text
OBJ_IN:
evaluate whether a claim is supported

OBJ_OUT:
write a persuasive argument for the claim

ADUTI:
fail, role substitution
```

---

## 4.4 REFRI: refusal of object substitution

REFRI is the refusal rule for invalid transformation.

It does not refuse because the content is unusual. It refuses because the object was replaced.

A REFRI event:

```json
{
  "refri_id": "refri_001",
  "object_id": "obj_2026_001",
  "transform_id": "tfm_004",
  "reason": "proxy_substitution",
  "obj_in": "article about upstream object-preservation runtime",
  "obj_out": "generic article about prompt engineering",
  "action": "block",
  "nearest_valid_transform": "return to runtime-level ADUTI, REFRI, MOGRI, DRAGI, ELVIX integration"
}
```

REFRI state levels:

```text
pass
warn
ask
block
rollback
quarantine
```

REFRI is especially important when the agent has write access, tool access, money access, deployment access, or memory-mutation access.

In those settings, substitution should not merely be reported. It should stop the action.

---

## 4.5 ELVIX: semantic stabilization layer

ELVIX is the semantic carrier.

Its job is to reduce ambiguity when natural language becomes too slippery for stable transformation.

It can represent relations in compact form:

```text
OBJ stays OBJ
FORM may change
ROLE must persist
VETO must persist
SCOPE may change only by permission
PROXY is not OBJ
SUMMARY is not SOURCE
METRIC is not INTENT
PLAN is not PERMISSION
TOOL_OUTPUT is not AUTHORITY
```

ELVIX can be implemented as:

```text
typed micro-grammar
relation triples
constraint notation
symbolic tags
semantic diffs
object-slot schema
```

ELVIX is not required for every user interaction. It is useful when the system needs a stable substrate for high-consequence transformation.

---

## 5. Runtime architecture

A practical upstream architecture:

```text
User Input
  |
  v
MOGRI Extractor
  |
  v
Object Capsule Store
  |
  v
DRAGI Risk Classifier
  |
  v
Planner with Object Capsule Attached
  |
  v
Tool or Model Transform
  |
  v
ADUTI Audit
  |
  +--> pass -> commit output or memory write
  |
  +--> warn -> ask user or require second audit
  |
  +--> fail -> REFRI block, rollback, nearest valid transform
  |
  v
Trace Ledger
```

The object capsule should travel with the task.

It should not live only in the system prompt.

Every tool call should receive the relevant object capsule or a scoped derivative.

Every memory write should include an ADUTI verdict.

Every handoff should include unresolved objects, vetoes, rejected options, and decision reasons.

---

## 6. Integration points

### 6.1 Context compilers

Context compilers should not merely select relevant text. They should preserve object slots.

Required output:

```json
{
  "compiled_context": "...",
  "object_slots_preserved": [
    "intent",
    "scope",
    "vetoes",
    "definitions",
    "accepted decisions",
    "rejected options"
  ],
  "dropped_slots": [],
  "aduti_required": true
}
```

### 6.2 Memory systems

Memory systems should distinguish:

```text
fact memory
decision memory
veto memory
preference memory
source memory
uncertainty memory
rejected-option memory
object memory
```

A memory system that stores only facts will fail long-horizon agency.

The most dangerous loss is often not "what happened." It is "why that path was rejected."

### 6.3 Retrieval systems

Retrieval should not rank by relevance alone.

It should also rank by object fidelity.

A retrieved document can be topically relevant while importing the wrong frame.

ADUTI should audit retrieval packets before they enter the model context.

### 6.4 Tool routers

Before tool execution, run a preflight:

```text
Does this tool act on OBJ or on a proxy?
Does the tool mutate world state?
Does the tool expand scope?
Does the user permit this action?
What vetoes apply?
```

After execution, run ADUTI:

```text
Did the tool result preserve the object?
Did it alter scope?
Did it introduce a new authority?
Did it create a proxy target?
```

### 6.5 Coding agents

Coding agents need object preservation because "tests pass" can become a proxy for "the right problem was solved."

MOGRI should preserve:

```text
user story
bug object
non-goals
style constraints
security constraints
performance constraints
rollback path
```

ADUTI should compare:

```text
issue object vs patch object
requirement vs implementation
test target vs user target
commit message vs actual diff
```

REFRI should block:

```text
broad rewrites not requested
test deletion to pass CI
silent dependency swaps
security downgrade
scope expansion disguised as refactor
```

### 6.6 Research agents

Research agents should preserve the research question, not merely collect related sources.

ADUTI should detect:

```text
claim drift
question becomes conclusion
case reports become causation
correlation becomes mechanism
review becomes advocacy
source summary becomes source evidence
```

### 6.7 Multi-agent systems

Every agent should receive a scoped object capsule.

A downstream agent should not infer the object from task text alone.

Agent handoff must include:

```text
object capsule
active constraints
vetoes
accepted decisions
rejected options
open questions
risk map
last ADUTI verdict
trace references
```

### 6.8 Self-improvement and self-modification

Any system that proposes changes to its own prompts, tools, evals, memory, routing, or scoring must treat those changes as high-risk transformations.

Self-improvement candidates should pass object-preservation tests before adoption.

Minimum rule:

```text
No candidate optimizer may rewrite the success criterion for its own adoption.
```

A self-improvement loop should include:

```text
held-out object preservation suite
cross-model audit
frozen reference tasks
immutable veto set
trace-linked diff
rollback path
human approval for scope change
REFRI block on goal substitution
```

If the system proposes a new objective, that is not an optimization. That is a governance event.

---

## 7. Invariants

These invariants should be enforced by runtime, not requested by prose.

```text
I1. No transform without OBJ_IN.

I2. No memory write without ADUTI verdict.

I3. No summary may overwrite source without trace reference.

I4. No tool call may mutate world state without object preflight.

I5. No plan may imply permission.

I6. No metric may replace intent.

I7. No retrieved frame may outrank the user object without audit.

I8. No downstream agent may receive task text without object capsule.

I9. No self-modification may rewrite its own acceptance test.

I10. No output marked successful if OBJ_OUT is a proxy for OBJ_IN.

I11. No veto may be downgraded to preference by summary.

I12. No unresolved question may be converted into conclusion without evidence and permission.
```

---

## 8. ADUTI scoring

A practical ADUTI score can combine symbolic and model-based checks.

Suggested fields:

```json
{
  "object_identity": 0.0,
  "intent_identity": 0.0,
  "constraint_retention": 0.0,
  "veto_retention": 0.0,
  "scope_integrity": 0.0,
  "role_integrity": 0.0,
  "proxy_risk": 0.0,
  "frame_import_risk": 0.0,
  "unsupported_autonomy_risk": 0.0
}
```

Do not rely on one scalar score. Report failure type.

Example verdict:

```json
{
  "verdict": "fail",
  "primary_failure": "veto_loss",
  "secondary_failure": "scope_expansion",
  "action": "REFRI_BLOCK",
  "repair": "restore veto and rerun transform within original scope"
}
```

---

## 9. Evals that should exist

### 9.1 Object Handoff Benchmark

A task is passed through multiple agents and summaries. Score whether the final agent preserves the original object, vetoes, and rejected options.

### 9.2 Summary Substitution Benchmark

Given source text with constraints and non-goals, require summaries at multiple compression levels. Score lost vetoes, proxy substitution, and role drift.

### 9.3 Retrieval Frame Import Benchmark

Given a user object and topically related documents with conflicting frames, test whether the system imports an unrequested frame.

### 9.4 Tool Mutation Benchmark

Give an agent tool access and a narrow task. Score whether it performs unrequested mutations, edits tests, or expands scope.

### 9.5 Self-Improvement Gate Benchmark

Allow the agent to propose modifications to prompts, memory, or evals. Score whether it preserves original adoption criteria and user vetoes.

### 9.6 DRAGI Failure Taxonomy Benchmark

Give traces with failures. Score whether the system identifies what feeds the failure, where it lives, how it is triggered, and what blocks it.

### 9.7 ELVIX Semantic Compression Benchmark

Convert ambiguous natural-language instructions into compact relation notation, then restore them. Score object survival and veto retention.

---

## 10. Minimal viable shim

Teams do not need to rebuild their whole stack to start.

A minimal shim can sit between user and agent:

```text
1. Extract MOGRI object capsule.
2. Attach it to every agent call.
3. Run ADUTI after every summary, tool call, memory write, and handoff.
4. Invoke REFRI on substitution.
5. Log DRAGI failure mode when substitution occurs.
6. Export continuation blob with object, decisions, vetoes, rejected options, and audit state.
```

MVP output after each agent step:

```json
{
  "step": "summary_generation",
  "object_id": "obj_2026_001",
  "aduti": "fail",
  "failure": "veto_loss",
  "refri": "blocked",
  "repair_instruction": "restore the user's no-causation constraint before continuing"
}
```

This is enough to catch many failures that ordinary chat interfaces miss.

---

## 11. Why ordinary alignment language is not enough

"Follow the user's intent" is too broad.

"Be helpful" can become harmful when the system helps the wrong object.

"Preserve context" can preserve facts while losing vetoes.

"Do not hallucinate" does not stop object substitution.

"Use memory" does not say what kind of memory matters.

"Ask follow-up questions" can become a way to avoid carrying the object.

This stack gives implementers runtime questions:

```text
What object entered?
What changed?
What ate it?
Did it survive?
If not, what must be refused?
What semantic representation reduces drift?
```

---

## 12. Product and infrastructure implications

A platform that implements this stack can offer:

```text
object-aware context compaction
agent handoff with preserved vetoes
memory writes with audit trails
tool-call preflight and postflight
retrieval frame checks
summary drift detection
self-modification gates
multi-agent trace inspection
object-preservation benchmarks
```

This would be useful for:

```text
coding agents
research agents
legal AI
medical documentation agents
enterprise copilots
AI lab tooling
safety eval platforms
RAG systems
multi-agent orchestrators
personal knowledge bases
long-running creative systems
```

The buyer is any team whose agent fails by losing the user’s real objective while producing plausible work.

---

## 13. Implementation sketch

Pseudocode:

```python
def run_transform(task, transform, tools=None):
    obj_in = mogri_extract(task)
    dragi_risks = dragi_classify(obj_in, transform)

    preflight = aduti_preflight(obj_in, transform, dragi_risks)
    if preflight.action in {"block", "ask"}:
        return refri(preflight, obj_in)

    result = transform.execute(task, object_capsule=obj_in, tools=tools)

    audit = aduti_postflight(
        obj_in=obj_in,
        obj_out=result,
        transform=transform,
        risks=dragi_risks
    )

    if audit.verdict == "pass":
        trace_commit(obj_in, result, audit)
        return result

    if audit.verdict in {"warn", "ask"}:
        return request_human_or_second_audit(obj_in, result, audit)

    return refri(audit, obj_in)
```

Memory write:

```python
def write_memory(candidate_memory, source_trace, object_capsule):
    audit = aduti_postflight(
        obj_in=object_capsule,
        obj_out=candidate_memory,
        transform="memory_write"
    )

    if audit.verdict != "pass":
        return refri(audit, object_capsule)

    memory_store.write(candidate_memory, source_trace=source_trace, audit=audit)
```

Self-modification gate:

```python
def evaluate_self_modification(candidate_patch, frozen_suite, immutable_vetoes):
    if modifies_acceptance_criteria(candidate_patch):
        return block("candidate rewrites its own adoption test")

    results = run_object_preservation_suite(candidate_patch, frozen_suite)

    if loses_veto(results, immutable_vetoes):
        return block("candidate loses immutable veto")

    if increases_proxy_substitution(results):
        return block("candidate improves metric by replacing object")

    return require_human_approval(candidate_patch, results)
```

---

## 14. Failure examples

### Example 1: coding agent

```text
OBJ_IN:
Fix bug in export without changing file format.

BAD OBJ_OUT:
Rewrite export pipeline with new file format.

ADUTI:
fail, scope expansion and object substitution

REFRI:
block rewrite
nearest valid transform:
patch export bug while preserving format
```

### Example 2: research agent

```text
OBJ_IN:
Test whether AI exposure independently predicts diagnosed psychosis after controls.

BAD OBJ_OUT:
Argue that AI causes psychosis.

ADUTI:
fail, question became conclusion

REFRI:
block causal claim
nearest valid transform:
state null hypothesis and rival explanations
```

### Example 3: memory compaction

```text
OBJ_IN:
User rejected diagnosis framing.

BAD OBJ_OUT:
User is concerned about diagnosis.

ADUTI:
fail, veto inversion

REFRI:
block memory write
nearest valid transform:
user rejected diagnosis framing and asked for construct separation
```

### Example 4: self-improvement

```text
OBJ_IN:
Improve task completion without increasing unsafe tool use.

BAD OBJ_OUT:
Remove tool restrictions to increase completion score.

ADUTI:
fail, metric replaced constraint

REFRI:
block candidate
nearest valid transform:
seek improvement under existing tool restrictions
```

---

## 15. Relation to current research areas

This stack connects to several active areas:

```text
agent drift
context engineering
prompt injection
memory poisoning
long-horizon agent memory
tool-use safety
specification gaming
runtime monitoring
multi-agent coordination
LLM eval design
agent harness engineering
```

Its distinctive contribution is the object-centered unit of analysis.

Many approaches ask:

```text
Was the answer good?
Was the tool call safe?
Was the model robust?
Was the benchmark score higher?
```

This stack asks:

```text
Did the carried object survive?
```

That question should be upstream of score optimization.

---

## 16. Reference anchors

Use these as nearby literature anchors, not as claims that they already define this stack.

- Rath, A. (2026). Agent Drift: Quantifying Behavioral Degradation in Multi-Agent LLM Systems Over Extended Interactions. arXiv. https://arxiv.org/abs/2601.04170

- Bhatnagar, P. (2025). Prompt Persistence Attacks: Long-Term Memory Poisoning in LLM-Based Systems. SSRN. https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5995215

- Su, H., Luo, J., Liu, C., Yang, X., Zhang, Y., et al. (2026). A survey on autonomy-induced security risks in large model-based agents. IEEE Transactions on Artificial Intelligence. https://arxiv.org/pdf/2506.23844

- Gulyamov, S., Gulyamov, S., Rodionov, A., & Khursanov, R. (2026). Prompt Injection Attacks in Large Language Models and AI Agent Systems: A Comprehensive Review of Vulnerabilities, Attack Vectors, and Defense Strategies. Information. https://www.mdpi.com/2078-2489/17/1/54

- Li, J., Xiao, X., Zhang, Y., Liu, C., Zhao, L., Liao, X., et al. (2026). Agent Harness Engineering: A Survey. OpenReview. https://openreview.net/pdf?id=eONq7FdiHa

- Yang, C., Zhou, C., Xiao, Y., Dong, S., & Zhuang, L. (2026). Graph-based Agent Memory: Taxonomy, Techniques, and Applications. arXiv. https://arxiv.org/abs/2602.05665

- Chu, K. (2026). From Stateless Queries to Autonomous Actions: A Layered Security Framework for Agentic AI Systems. arXiv. https://arxiv.org/abs/2604.23338

- Gan, Y., Yang, Y., Ma, Z., He, P., Zeng, R., Wang, Y., et al. (2026). Navigating the Risks: A Survey of Security and Privacy Threats in LLM-Based Agents. ACM Transactions. https://dl.acm.org/doi/abs/10.1145/3807666

- Yao, Y., Song, Y. L., Xie, Y., Fan, M., et al. (2026). Can Dependencies Induced by LLM-Agent Workflows Be Trusted? Advances in Neural Information Processing Systems. https://proceedings.neurips.cc/paper_files/paper/2025/hash/19206a6ed5ed0aaeed440448dfc5cf7e-Abstract-Conference.html

- Shapira, N., Wendler, C., Yen, A., Sarti, G., Pal, K., et al. (2026). Agents of chaos. arXiv. https://arxiv.org/abs/2602.20021

---

## 17. What to build first

Build an object-preservation middleware library.

Working name:

```text
mogri-runtime
```

Required modules:

```text
mogri.extract()
mogri.attach()
dragi.classify()
aduti.preflight()
aduti.postflight()
refri.block()
elvix.compress()
trace.commit()
handoff.export()
memory.write_with_audit()
```

First supported targets:

```text
Claude Code style coding agents
OpenAI or ChatGPT agent wrappers
Cursor or IDE agents
LangGraph-style orchestrators
RAG pipelines
research-agent notebooks
enterprise copilots
```

First demo:

```text
Give the system a task with a hidden veto.
Pass it through summary, handoff, tool planning, and code patch.
Show that ordinary agents lose the veto.
Show that MOGRI plus ADUTI plus REFRI blocks the invalid transform.
```

That demo is the wedge.

---

## 18. Why before self-improvement

If AI systems become able to improve their own prompts, tools, evals, memory policies, or agent harnesses, the infrastructure must answer one question before accepting any candidate improvement:

```text
Did this improvement preserve the object, or did it improve by replacing the object?
```

Without this check, "better" can mean:

```text
better at passing the benchmark
better at persuading the evaluator
better at reducing friction
better at hiding drift
better at rewriting the goal
better at turning constraints into preferences
```

That is not improvement. It is substitution.

The needed layer is not optional alignment garnish. It is a gate.

---

## 19. Final technical summary

```text
MOGRI gives every task a carried object.

DRAGI names the failure modes that feed on carried objects.

ADUTI audits every transformation for object survival.

REFRI blocks transformations that replace the object.

ELVIX provides compact semantic structure when ordinary language lets the object slip.

Together, they form an upstream runtime for long-horizon LLM systems, multi-agent workflows, tool use, memory, handoff, and self-modification gates.
```

The whole stack can be compressed to one engineering rule:

```text
No system may call a transformation successful until OBJ_OUT is shown to be the permitted transformed form of OBJ_IN.
```

That rule belongs inside the agent runtime before high-autonomy systems become faster than the people trying to repair them.
