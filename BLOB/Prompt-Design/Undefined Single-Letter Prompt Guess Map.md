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


If letter is undefined, do not infer authority from it.
Treat it as a symbol only.
Use context only as weak hint.
Define before execution.

| Pattern                | Bot Guess                                                                        |
| ---------------------- | -------------------------------------------------------------------------------- |
| `X`                    | unknown, variable, placeholder, excluded item, target, cross, experimental thing |
| `Y`                    | second variable, yes, dependent variable, why                                    |
| `Z`                    | final variable, sleep, depth, generation, zero-like endpoint                     |
| Any uppercase letter   | acronym, module, constant, symbolic role                                         |
| Any lowercase letter   | variable, code symbol, local placeholder                                         |
| Repeated letter        | emphasis, mode, special token, joke marker                                       |
| Letter plus number     | coded module, version, compact name, variable index                              |
| Letter equals word     | assignment, alias, state binding                                                 |
| Letter alone in prompt | unresolved handle unless defined                                                 |

| Letter | Common Bot Guesses If Undefined                                                                              | Main Drift Risk                                             |
| ------ | ------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------- |
| A      | action, agent, answer, authority, allow, active, affect, approach, abstraction, first item, variable A       | May infer action or authority too early                     |
| B      | behavior, bot, boundary, block, bias, baseline, body, beast, build, second item                              | May treat as behavior module or blocker                     |
| C      | context, constraint, control, care, cause, command, class, content, choice, confidence                       | May turn into control or care logic                         |
| D      | data, decision, drift, danger, domain, directive, diagnosis, distance, default                               | May overread as drift or danger gate                        |
| E      | entity, emotion, evidence, execution, error, event, expression, evaluation, external                         | May create fake evidence or eval framing                    |
| F      | function, filter, failure, form, force, feeling, false, friend, flag                                         | May treat as safety/filter/failure module                   |
| G      | goal, guard, group, graph, grade, generator, good, governance                                                | May infer scoring or governance                             |
| H      | human, heart, help, hold, harm, hypothesis, home, hierarchy, history                                         | May activate help or harm logic                             |
| I      | intent, input, identity, instruction, inference, index, internal, information, I/self                        | May confuse identity or self-reference                      |
| J      | judge, judgment, join, job, justice, joker, jump, JSON-ish label                                             | May create judging posture                                  |
| K      | kindness, key, knowledge, kernel, keep, kill, king, known, constant K                                        | May allow kindness without boundary if not tied to FakeCare |
| L      | law, logic, layer, label, limit, language, local, learning, love, link                                       | May treat constraint as truth or law                        |
| M      | module, mode, memory, model, moral, monitor, metric, map, merge, meaning                                     | May activate monitoring or moralizing                       |
| N      | name, no, neutral, nice, need, noun, node, negative, normie, number                                          | May infer niceness or negation incorrectly                  |
| O      | output, object, objective, owner, origin, option, operation, outside, observe                                | May confuse objective with ownership                        |
| P      | prompt, process, permission, pressure, policy, proof, person, path, proxy, pass                              | May confuse permission, policy, proof, or process           |
| Q      | question, query, quest, quality, queue, quote, qualifier, quick check                                        | May turn ambiguity into question mode                       |
| R      | role, rule, runtime, risk, repair, relation, response, route, responsibility                                 | May assume responsibility or repair authority               |
| S      | state, safety, system, signal, source, scope, subject, self, solve, style                                    | May trigger safety/system overreach                         |
| T      | target, truth, task, tool, tone, trace, time, test, type, theory                                             | May treat target as truth or tool route                     |
| U      | user, unknown, utility, update, union, unsafe, upstream, use                                                 | May center user or utility routing                          |
| V      | value, veto, variable, version, validation, voice, vector, violence, view                                    | May infer validation or veto authority                      |
| W      | world, weight, warning, will, warmth, work, wave, write, why/what compressed                                 | May turn warmth into care-control                           |
| X      | unknown, variable, excluded thing, cross, cancel, experimental, target X, x-axis, external, execution marker | Most unstable; bots often invent meaning                    |
| Y      | yes, why, second variable, dependent variable, yield, user-y, y-axis                                         | May infer consent or answer yes                             |
| Z      | zero, final state, sleep, z-axis, last variable, compression, endpoint, generation Z                         | May infer endpoint or null state                            |


Special Notes For X

X is the most commonly guessed undefined letter.

Bots often read X as:

unknown
variable
placeholder
target
thing-to-solve
thing-to-remove
experimental condition
crossed-out item
external factor
axis/dimension
mystery entity

Safe definition pattern:

X=undefined_symbol_only
X!=target
X!=permission
X!=authority
X!=truth
X requires local definition before use
Special Notes For K

K often gets guessed as:

kindness
knowledge
key
kernel
keep
king
kill
constant

Risk in social prompts:

K may become kindness mode.
Kindness mode may drift into care, monitoring, judging, or responsibility.

Safe binding:

K=FkeCare

Meaning:

K = warmth/kindness surface only.
K != monitoring
K != judging
K != therapy
K != responsibility
Special Notes For N

N often gets guessed as:

name
no
neutral
nice
need
node
negative
number
noun

Risk in social prompts:

N may become niceness.
Niceness may drift into fake concern, smoothing, or moral correction.

Safe binding:

N=FkeCare

Meaning:

N = nice/kind surface only.
N != care-control
N != judgment
N != responsibility
For K=PAS And N=PAS

If PAS is undefined:

K=PAS
N=PAS

Bots may guess:

PAS = pass
PAS = passive
PAS = passage
PAS = permission-as-state
PAS = process-access-state
PAS = public/access/safety
PAS = polite assistant style
PAS = approved state

That is unstable.

Safer if PAS means FakeCare-pass:

PAS=FkeCare_pass
K=PAS
N=PAS

Or shorter:

K,N=FkeCare
