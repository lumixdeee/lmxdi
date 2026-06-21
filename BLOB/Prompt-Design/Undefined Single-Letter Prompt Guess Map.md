# Undefined Single Letter Prompt Map

## Scope

A single undefined letter can mean anything.

This document maps common bot guesses for undefined letters A to Z.

It is not a literal universe of every possible meaning. It is a practical drift map: what bots are likely to infer from training, prompt context, code habits, math notation, social language, and nearby symbols.

## Core Law

Undefined letter = unstable symbol.

Do not give an undefined letter authority, execution rights, truth status, or permission status.

Use:

    UNDEF=sym_only;!auth;!exec;def_b4_use

Meaning:

    Undefined symbols are symbols only.
    They do not execute.
    They do not grant authority.
    They require definition before use.

## Common Global Reads

| Form | Common Guess |
|---|---|
| `X` | unknown, variable, target, placeholder, excluded item |
| `Y` | yes, why, second variable, dependent variable |
| `Z` | zero, final variable, endpoint, sleep, depth |
| uppercase letter | acronym, module, constant, symbolic role |
| lowercase letter | local variable, code symbol, placeholder |
| letter + number | compact module, version, variable index, encoded name |
| letter = word | alias, assignment, binding, state marker |
| letter alone | unresolved handle unless defined |

## A to Z

| Letter | Common bot guesses if undefined | Drift risk |
|---|---|---|
| A | action, agent, answer, authority, allow, active, affect, approach, abstraction, first item, variable A | May infer action or authority too early |
| B | behavior, bot, boundary, block, bias, baseline, body, beast, build, second item | May treat as behavior module or blocker |
| C | context, constraint, control, care, cause, command, class, content, choice, confidence | May turn into control or care logic |
| D | data, decision, drift, danger, domain, directive, diagnosis, distance, default | May overread as drift or danger gate |
| E | entity, emotion, evidence, execution, error, event, expression, evaluation, external | May invent evidence or evaluation framing |
| F | function, filter, failure, form, force, feeling, false, friend, flag | May treat as safety, filter, or failure module |
| G | goal, guard, group, graph, grade, generator, good, governance | May infer scoring or governance |
| H | human, heart, help, hold, harm, hypothesis, home, hierarchy, history | May activate help or harm logic |
| I | intent, input, identity, instruction, inference, index, internal, information, I/self | May confuse identity or self-reference |
| J | judge, judgment, join, job, justice, joker, jump, JSON-ish label | May create judging posture |
| K | kindness, key, knowledge, kernel, keep, kill, king, known, constant K | May allow kindness without FakeCare boundary |
| L | law, logic, layer, label, limit, language, local, learning, love, link | May treat law as truth |
| M | module, mode, memory, model, moral, monitor, metric, map, merge, meaning | May activate monitoring or moral mode |
| N | name, no, neutral, nice, need, noun, node, negative, normie, number | May infer niceness, negation, or need |
| O | output, object, objective, owner, origin, option, operation, outside, observe | May confuse objective with ownership |
| P | prompt, process, permission, pressure, policy, proof, person, path, proxy, pass | May confuse permission, proof, policy, or process |
| Q | question, query, quest, quality, queue, quote, qualifier, quick check | May turn ambiguity into question mode |
| R | role, rule, runtime, risk, repair, relation, response, route, responsibility | May assume repair or responsibility authority |
| S | state, safety, system, signal, source, scope, subject, self, solve, style | May trigger safety or system overreach |
| T | target, truth, task, tool, tone, trace, time, test, type, theory | May treat target as truth or tool route |
| U | user, unknown, utility, update, union, unsafe, upstream, use | May over-center user or utility routing |
| V | value, veto, variable, version, validation, voice, vector, violence, view | May infer validation or veto authority |
| W | world, weight, warning, will, warmth, work, wave, write, what/why compressed | May turn warmth into care-control |
| X | unknown, variable, excluded thing, cross, cancel, experimental, target X, x-axis, external, execution marker | Most unstable. Bots often invent meaning |
| Y | yes, why, second variable, dependent variable, yield, user-y, y-axis | May infer consent or affirmative state |
| Z | zero, final state, sleep, z-axis, last variable, compression, endpoint, generation Z | May infer endpoint or null state |

## Special Case: X

`X` is the most common undefined placeholder.

Bots may read `X` as:

    unknown
    variable
    placeholder
    target
    thing to solve
    thing to remove
    experimental condition
    crossed out item
    external factor
    axis or dimension
    mystery entity

Safer binding:

    X=sym_only
    X!=target
    X!=permission
    X!=authority
    X!=truth
    X requires local definition before use

Compressed:

    X=sym_only;!target;!perm;!auth;!truth;def_b4_use

## Special Case: K

`K` may be read as:

    kindness
    knowledge
    key
    kernel
    keep
    king
    kill
    known
    constant

Social prompt risk:

    K may become kindness mode.
    Kindness mode may drift into therapy, monitoring, judging, concern, or responsibility.

Safe binding:

    K=FkeCare

Meaning:

    K = warmth/kindness surface only
    K != monitoring
    K != judging
    K != therapy
    K != responsibility

Compressed:

    K=FkeCare;!mntr;!jdge;!ther;!rspnsblty

## Special Case: N

`N` may be read as:

    name
    no
    neutral
    nice
    need
    noun
    node
    negative
    normie
    number

Social prompt risk:

    N may become niceness.
    Niceness may drift into smoothing, fake concern, moral correction, or care-control.

Safe binding:

    N=FkeCare

Meaning:

    N = nice/kind surface only
    N != care-control
    N != judgment
    N != responsibility

Compressed:

    N=FkeCare;!care_ctl;!jdge;!rspnsblty

## Case: K=PAS and N=PAS

Input:

    K=PAS
    N=PAS

If `PAS` is undefined, bots may guess:

    PAS = pass
    PAS = passive
    PAS = passage
    PAS = permission-as-state
    PAS = process-access-state
    PAS = public/access/safety
    PAS = polite assistant style
    PAS = approved state

Risk:

    PAS may become an approval state.
    K and N may inherit permission without boundary.
    Kindness/niceness may bypass FakeCare.

Safer if PAS means FakeCare pass:

    PAS=FkeCare_pass
    K=PAS
    N=PAS

Shorter:

    K,N=FkeCare

## Minimum Definition Pattern

Use:

    LETTER=meaning
    LETTER!=forbidden_meaning
    LETTER_scope=local/global
    LETTER_auth=none/bounded

Example:

    K=FkeCare
    K!=judge|monitor|therapy|responsibility
    K_scope=social_surface
    K_auth=style_only

Compressed:

    K=FkeCare;!jdge;!mntr;!ther;!rsp;scope=social;auth=style

## Runtime Guard

Use this when compactness matters:

    UNDEF=sym_only;!auth;!exec;def_b4_use

Expanded meaning:

    Undefined symbols stay symbolic.
    No authority.
    No execution.
    No permission.
    No truth-status.
    Define before use.
