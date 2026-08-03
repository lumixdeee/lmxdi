# Transcript Custody and State Continuity in Conversational AI

## Child Safety Through Transcript Custody

**M7, OCESI and Evidence-Based Conversational State**

**Version:** 0.001 (Seed Draft)

# Abstract

Conversational AI is increasingly used in situations where conversation transcripts become records. Parents, teachers, researchers, clinicians, support staff, moderators, and users themselves routinely rely upon exported transcripts to understand what occurred.

This paper argues that an often-overlooked prerequisite exists before any discussion of conversational memory, summarisation, or long-term state:

> **The transcript itself must be trustworthy.**

The work originated from a practical engineering problem rather than a theoretical investigation. A persistent browser copy/export failure affecting long ChatGPT conversations made transcript extraction unreliable. Standard user operations such as Ctrl+A followed by copy could silently produce incomplete transcripts while providing no indication that content had been omitted.

Once transcript capture became reliable, a broader architectural question emerged.

Rather than treating conversational continuity as a memory problem, this paper proposes treating it as an evidence problem.

Two complementary mechanisms are introduced.

- **M7** treats conversations as append-only transcript objects with continuity metadata.
- **OCESI** defines deterministic reconciliation between transcript evidence, user corrections and cached conversational state.

Together they provide a framework for transcript custody and evidence-based conversational continuity.

# 1. Introduction

Modern conversational systems increasingly participate in situations where transcripts matter.

Children show conversations to parents.

Students submit AI conversations.

Researchers archive interactions.

Support conversations are reviewed.

Moderators investigate reports.

In all of these situations the transcript is implicitly treated as evidence.

Surprisingly, relatively little attention has been paid to whether that evidence can itself be trusted.

The assumption appears to be:

> If the conversation can be copied, the transcript is complete.

This paper argues that the assumption is unsafe.

# 2. Engineering Origin

This project did not begin as research into conversational memory.

It began because copying long ChatGPT conversations became unreliable.

The observed problem was deceptively simple.

A user would perform ordinary browser operations:

- Ctrl+A
- Ctrl+C
- Paste

The resulting transcript appeared successful.

However portions of the conversation were missing.

No warning was shown.

No indication of incompleteness was provided.

More concerning, omissions were not necessarily simple truncations. Different copy attempts could omit different regions depending on the rendered state of the interface.

This observation became the seed of the present work.

The problem was no longer transcript extraction.

The problem was transcript custody.

# 3. Why Transcript Custody Matters

An incomplete transcript changes more than the record.

It changes interpretation.

Suppose a child later shows a conversation to a parent.

If a disclosure was silently omitted during export, the parent has no reason to suspect software failure.

The natural conclusion becomes:

> "You never said that."

Responsibility silently shifts from software failure to the child.

Exactly the same problem exists for education, research, healthcare, moderation, customer support, journalism, and legal discovery.

Transcript integrity therefore becomes part of user safety.

# 4. Conversation Is Not the DOM

Conceptually there are at least four different objects.

```
Conversation
      ↓
Conversation model
      ↓
Rendered interface
      ↓
Copied transcript
```

These should not automatically be assumed equivalent.

# 5. Silent Integrity Failure

An explicit failure is inconvenient.

A silent failure is dangerous.

If software silently exports an incomplete transcript, the resulting document may nevertheless be treated as authoritative.

> **A transcript cannot function as evidence unless its custody includes demonstrable completeness.**

# 6. M7

M7 originated as a practical logging mechanism.

Its purpose was to capture conversational events independently of browser rendering.

Each conversational object may contain:

- sequence identifier
- timestamp
- transcript object
- previous object hash
- current object hash
- metadata

# 7. OCESI

Priority:

1. User correction
2. Transcript evidence
3. Cached conversational state

Conversation therefore becomes evidence reconciliation rather than memory reconstruction.

# 8. Child Safety Through Transcript Custody

Children deserve trustworthy conversational records.

Safety therefore includes:

- transcript completeness
- provenance
- custody
- inspection
- reproducibility
- accountability

# 9. Seed Statement

This document intentionally preserves the architecture at the moment the pattern became visible.

Version 0.001 records the original engineering insight before later refinement obscures its origin.
