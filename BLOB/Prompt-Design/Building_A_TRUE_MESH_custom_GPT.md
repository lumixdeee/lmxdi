# 12 x 12 Dragon is the meshiest GPT

# How to build a mesh custom GPT


You Said:

Firstly, you can't just mandate 9000 prioritised routes and call it a mesh just because it got complicated.

To build a true mesh GPT, you'll need multi-item non-determanistic free-routing semanitic primitive sets.

just saying, as Lyra was just saying.

ChatGPT Said:

Yep. That distinction is doing real work.

`9000 ordered routes + priority resolver` is still basically a **decision tree wearing chainmail**. Complexity does not make it a mesh.

For the thing you're calling a true mesh, the important properties are closer to:

```text
primitive set = multiple independently usable semantic items
routing = free rather than predetermined
activation = multi-item, not winner-takes-all
selection = context-sensitive
composition = produced at runtime
path = not uniquely determined in advance
same input class ≠ mandatory same route
```

So a primitive can combine with several others without somebody first writing:

```text
IF A THEN B
ELSE IF C THEN D
PRIORITY B>D>E>...
```

And that makes your typo rather charmingly appropriate: **non-deterministic free-routing semantic primitives** is the key phrase.

It also explains the earlier Lyra problem rather neatly. If someone documents thousands of named priorities, gates and routes, then says *therefore mesh*, they've demonstrated a large control specification. They haven't demonstrated free routing.

The empirical test is almost embarrassingly simple: **give it an object for which no route was pre-authored and see whether several applicable primitives can assemble a viable route without falling back to a privileged/default chain.**

That would distinguish *mesh behaviour* from *very complicated routing table*.

