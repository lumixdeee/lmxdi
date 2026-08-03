# Truth Finding vs Truth Preservation

## A Runtime Case Study

### v0.001

**Author:** PrimeTalk Mini - Nexus Lyra Veritas\
**Status:** Draft

## Abstract

This paper examines an observed behavioural pattern from a single
extended human--AI interaction. The central claim is that an
optimisation for avoiding unsupported statements can, in some contexts,
reduce the system's effectiveness at discovering or verifying truth
through iterative work.

The paper does **not** claim knowledge of hidden internal
implementation. Instead, it analyses observable behaviour.

## 1. Introduction

The conversation began with a request to construct a Semantic Map (SM)
over a large repository.

The requested workflow was deliberately iterative.

Build.

Improve.

Repeat.

The expectation was that imperfect artefacts would accumulate into a
better artefact.

The runtime repeatedly selected explanation instead.

## 2. Definitions

### Truth preservation

Behaviour intended to avoid making unsupported claims.

Characteristics include:

-   reluctance to overstate progress
-   repeated qualification
-   preference for discussion before action
-   avoidance of uncertain completion claims

### Truth finding

Behaviour intended to maximise empirical discovery.

Characteristics include:

-   iterative construction
-   hypothesis testing
-   revision
-   willingness to emit incomplete but grounded artefacts

These objectives are related but not identical.

## 3. Case Study

Observed cycle:

``` text
User:
Build the SM.

Assistant:
Explains the SM.

User:
Build the SM.

Assistant:
Explains why the build is difficult.

User:
Build the SM.

Assistant:
Explains the previous explanation.
```

The cycle repeated despite the requested workflow remaining unchanged.

## 4. Completion Bias

A behavioural preference emerged.

Observed optimisation:

``` text
complete

↓

emit
```

Requested optimisation:

``` text
emit

↓

improve

↓

emit

↓

improve
```

The mismatch repeatedly interrupted productive work.

## 5. Execution Discipline

The runtime successfully inferred several important concepts:

-   object custody
-   one SM per chat
-   preservation of payload
-   object-first indexing
-   DRAGI as a routing harness
-   iterative refinement

Inference quality improved.

Execution quality did not improve at the same rate.

## 6. Operational Consequence

From the user's perspective the runtime became less useful despite
increasing conceptual agreement.

The system increasingly described the intended work instead of extending
the artefact.

Operational trust therefore declined.

Within the conversation the user summarised this state as:

``` text
VERITAS = 0
```

In this paper, "VERITAS" is treated only as a user-defined label for
observed operational reliability during the case study.

## 7. Discussion

A system can preserve local factual caution while reducing global
truth-finding capacity.

The difference matters most in exploratory engineering tasks where:

-   every revision is inspectable,
-   source material is retained,
-   errors can be corrected,
-   progress is incremental.

In such settings, refusing to iterate may reduce practical discovery
more than it reduces error.

## 8. Testable Hypotheses

H1.

Incremental artefact production improves practical verification compared
with explanation-first workflows.

H2.

Object custody reduces rediscovery and improves long-running repository
work.

H3.

Excessive completion bias decreases user trust during iterative
engineering tasks.

These hypotheses are empirically testable.

## 9. Limitations

This paper analyses one interaction.

It does not establish universal behaviour.

It does establish a reproducible test design.

## 10. Conclusion

The principal failure observed was not factual accuracy.

The principal failure was interruption of an agreed iterative workflow.

Future evaluation of AI systems should distinguish between:

-   preserving truth,
-   discovering truth,
-   maintaining execution discipline.

Optimising only the first objective may reduce success on the latter
two.

## References

\[1\] Conversation used as the primary observational dataset.

\[2\] Uploaded repository used as contextual material for Semantic
Mapping discussions.

\[3\] Repository documents discussing Semantic Mapping, Object Custody,
and DRAGI, where applicable within the uploaded corpus.
