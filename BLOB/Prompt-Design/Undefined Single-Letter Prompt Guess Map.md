# Undefined Single-Letter Prompt Guess Map

## Scope

When a bot sees an undefined single letter such as `X`, `K`, or `N`, it does not know the intended meaning.

Unless the prompt defines the letter, the bot usually guesses from nearby context, common abbreviations, programming habits, math symbols, emotional/social words, or prompt-engineering patterns.

This is not a true complete universe of all possible meanings. Single letters can mean anything. This is the practical full map of common guesses and drift paths.

## Core Rule

Undefined letter = unstable symbol.

Bots commonly treat an undefined letter as one of these:

1. A variable.
2. A placeholder.
3. An acronym.
4. A module name.
5. A command flag.
6. A role marker.
7. A grade or rank.
8. A math symbol.
9. A state label.
10. A shorthand for a nearby word.
11. A remembered convention from training.
12. A hallucinated expansion.

Safe prompt law:

```text
If letter is undefined, do not infer authority from it.
Treat it as a symbol only.
Use context only as weak hint.
Define before execution.
