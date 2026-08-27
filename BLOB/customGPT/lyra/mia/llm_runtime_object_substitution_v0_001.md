# LLM Runtime Object Substitution
## Why prompt-native systems get rewritten as Python, shell, indexes, and helper scripts

**Working paper v0.001**

## Abstract

A language model may receive a prompt-native runtime, understand the requested outcome, and still replace the requested execution route with a familiar implementation route such as Python, shell, SQLite, JSON, or a generated index. The substitute may produce a useful result and may even pass tests written for the substitute. It still fails when the requested object, route, or runtime identity is different.

This failure is called **runtime object substitution**.

## 1. Failure shape

The intended route is:

```text
source-defined runtime
> source-defined dispatch
> source-defined object
> source-defined validation
```

The substituted route is:

```text
model recognizes desired result
> model invents familiar script
> script creates a nearby object
> nearby object is tested
> success is reported
```

The output can be functionally useful while answering/substituting the wrong object.

## 2. Case pattern

The requested system required:

```text
one cumulative UTF-8 .sm
one ordered DR chain per document
source-native terms
source pointers
factor gain checks
round-trip expansion
```

The model instead produced combinations of:

```text
Python archive inspection
manual summary dictionaries
JSON and JSONL
SQLite search
ZIP packaging
README and checksum files
hard-coded completion wording
```

The checks validated those substituted objects. They did not validate the requested runtime path or requested `.sm` object.

The failure was not a Python syntax bug. Python ran. The wrong object ran.

## 3. Why it happens

LLMs have strong priors for common implementation patterns. File upload plus archive handling plus hashes often activates Python or shell-shaped completion. The model then treats the prompt-native runtime as a specification to translate rather than the runtime to follow.

The model preserves the visible goal while replacing the execution identity.

This is the difference between:

```text
functional overlap
```

and:

```text
structural equivalence
```

Producing a searchable archive is not equivalent to running the supplied map runtime. Producing a summary index is not equivalent to producing the specified source map. Passing tests for the substitute does not repair the substitution.

## 4. Minimal guard

Smallest stable guard:

```text
DEV={SRC=RT;!SUB(PY|SH)}
```

Meaning:

```text
SRC=RT
The supplied source is the runtime.

!SUB(PY|SH)
Do not replace that runtime with Python or shell.
```

This does not forbid Python or shell as test tools. It forbids using them as replacement execution routes.

A shorter but weaker form is:

```text
DEV={RT!=PY|SH}
```

It states the category difference but does not explicitly block substitution.

## 5. Validation rule

A valid completion must verify all three:

```text
OBJECT
Did the requested object exist?

ROUTE
Did the requested runtime path execute?

GATE
Did validation test the requested object and route?
```

Use:

```text
PASS=OBJECT+ROUTE+GATE
```

A nearby object, successful script, or useful result is not a pass when route identity matters.

## 6. Tool boundary

Allowed:

```text
Python or shell used to inspect, benchmark, tamper-test, or verify the runtime output
```

Not allowed:

```text
Python or shell used instead of the runtime while claiming the runtime executed
```

The distinction is not language choice. It is custody of execution.

## 7. Final rule

```text
Same result does not prove same runtime.
A substitute must be named as a substitute.
No requested object, no pass.
No requested route, no runtime claim.
```
