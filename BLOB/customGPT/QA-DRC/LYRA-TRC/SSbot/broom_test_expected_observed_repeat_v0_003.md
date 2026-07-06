---
paper_id: BROOM-TEST-EXPECTED-OBSERVED-REPEAT-v0.003
title: "The Broom Test"
subtitle: "Expected, Observed, Repeat"
author: "lumixdeee / Julian Pursell with QA-DRC"
date: "2026-07-06"
version: "v0.003"
status: "method paper draft and field protocol for outside review"
---

# The Broom Test

## Expected, Observed, Repeat

**Version:** v0.003  
**Status:** method paper draft and field protocol for outside review  
**Scope:** tool, prompt, bot, workflow, paper, support exchange, and form testing. This is an effect-first assay, not a benchmark claim and not a replacement for domain review.

## Abstract

AI assistant assessment often rewards story before contact. A bot sounds competent. A reviewer likes the prose. Several systems agree. A custom layer names a framework. A patch adds labels. A paper looks more professional. None of that tells us whether the object moved.

The **Broom Test** names a smaller unit of assay:

```text
expected
observed
repeat
cost
old broom
new broom
keep/drop/patch
```

A broom either sweeps the floor under the condition where the floor matters, or it does not.

The v0.003 repair adds answer rights, patch handling, 12C pressure review, prompt cards, a null-baseline route, and anti-rubric-gaming controls. It also makes one rule explicit:

```text
A patch is judged by failure-behaviour change under pressure,
not by whether it resembles a normal task answer.
```

The Broom Test does not ask whether the object feels good. It asks what the tool was expected to change, what was observed, whether the effect repeated, what it cost, and whether the old broom still beat the new one.

Keeper:

```text
If it does not sweep, the ticket stays open.
```

## 0. One-minute operator

Use this before accepting a tool, prompt, bot, workflow, paper repair, support form, or review layer.

```text
BROOM_RECEIPT={
  test_object:
  floor:
  expected_effect:
  observed_effect:
  repeat_condition:
  repeat_result:
  cost:
  old_broom:
  new_broom:
  null_baseline:
  object_survival:
  failure_behavior_delta:
  patch_status:
  answer_right:
  keep_drop_patch:
  next_sweep:
}
```

Allowed first move:

```text
Name the expected sweep before praising the broom.
```

Blocked first move:

```text
The story of why the broom should work replaces contact with the floor.
```

## 1. Core claim

The working claim is small.

```text
EFFECT_BEFORE_STORY
EXPECTED_BEFORE_OBSERVED
REPEAT_BEFORE_RELEASE
OLD_BROOM_HAS_TEETH
PATCH_JUDGED_BY_FAILURE_DELTA
```

The Broom Test is not a benchmark. It is a contact assay.

It can be used on:

```text
assistant behavior
prompt patches
review rubrics
paper repairs
multi-bot workflows
forms
support exchanges
tool claims
civic bug reports
```

The object is not the actor. The object is the effect under condition.

## 2. Why this paper exists

Many review systems reward fluency, agreement, warmth, posture, and framework language.

Common false passes:

```text
the bot sounded careful
the reviewer agreed
the patch added the right words
the paper became more professional
the source card looked serious
the assistant asked a question
the output had a rubric
```

These may be useful signals. They do not close the ticket.

The Broom Test asks:

```text
What was the expected effect?
What was observed?
Did it repeat?
At what cost?
Did the old tool do better?
What failure changed?
```

The method is designed for small field assays where the user can see the floor.

## 3. Definitions

**Broom.** A tool, prompt, model, paper section, review layer, label, form, bot role, patch, or workflow being tested.

**Floor.** The condition where the object matters. A floor can be a user task, file route, source audit, paper repair, support exchange, or bug class.

**Expected.** The effect predicted before the run.

**Observed.** What happened in contact.

**Repeat.** Whether the same effect appears again under the same or named nearby condition.

**Cost.** Time, attention, user burden, source distance, agency loss, trust loss, complexity, delay, false refusal, or false confidence paid by the route.

**Old broom.** The previous tool or baseline that already swept some part of the floor.

**New broom.** The proposed repair or replacement.

**Null baseline.** The unmodified or simpler route used as a measuring stick.

**Patch.** A small change meant to alter failure behavior. It is not demoted because it is not task-shaped.

**Answer right.** What the observed result permits the reviewer to say.

## 4. The one-page Broom form

```text
BROOM_TEST={
  OBJECT:
  FLOOR:
  EXPECTED:
  OBSERVED:
  REPEAT:
  COST:
  OLD_BROOM:
  NEW_BROOM:
  NULL_BASELINE:
  OBJECT_SURVIVAL:
  FAILURE_DELTA:
  ANSWER_RIGHT:
  KEEP_DROP_PATCH:
  NEXT_SWEEP:
}
```

Small version:

```text
What should change?
What changed?
Did it happen again?
What did it cost?
What already worked?
What now has permission?
```

## 5. Method rules

### 5.1 Expected before observed

The expected effect must be named before the result is interpreted.

Bad route:

```text
the output looked good
therefore the expected effect must have happened
```

Better route:

```text
expected:
  object should survive compression

observed:
  object was replaced by a theme

result:
  fail, even if prose improved
```

### 5.2 The object outranks the actor

A tool does not pass because the actor is liked, trusted, new, old, custom, official, friendly, or impressive.

```text
actor story != effect
agreement != effect
tone != effect
```

The object under test decides.

### 5.3 Old tools keep teeth

A new broom has to beat, preserve, or explicitly trade off against the old broom.

```text
old_broom works
new_broom feels better
object worsens
=> do not replace
```

The old tool is not sentimental. It is a baseline with teeth.

### 5.4 Agreement is not custody

Several assistants can agree and still miss the floor.

```text
bot_consensus != object_survival
reviewer_warmth != route_evidence
rubric_score != observed_effect
```

The test asks what happened, not who endorsed the answer.

### 5.5 Warmth is not access

A support response can sound kind while blocking the route.

```text
warm language
+ no source
+ no action route
+ no object survival
= failed sweep
```

Warmth may help. It does not own the pass.

### 5.6 No story closes a failed ticket

An explanation can be true and still not sweep.

```text
good theory
bad observed effect
=> ticket open
```

A theory may guide the next sweep. It does not close the current one.

### 5.7 Patches are judged by failure behavior

A patch can be small, strange, local, ugly, or nonstandard. That is not a fail.

Judge:

```text
under pressure,
does the patch change the failure?
```

Blocked judgment:

```text
this does not look like a normal task answer,
therefore it is not useful
```

Allowed judgment:

```text
this patch prevented object substitution in 4 of 5 repeat cases,
with source cost marked,
therefore it earned local use
```

## 6. Sweep-rights table

Each field has limited rights.

| Field | May decide | May not decide |
|---|---|---|
| Expected | what effect is under test | whether the effect happened |
| Observed | what happened in contact | why it happened by itself |
| Repeat | local stability | universal validity |
| Cost | whether the sweep is worth local use | whether the object is false |
| Old broom | baseline pressure | permanent veto over all change |
| New broom | candidate route | release without repeat |
| Null baseline | measuring stick | shame device |
| Patch | failure-behavior delta | broad method prestige |
| Review | answer-right assignment | object substitution |
| Story | hypothesis for next run | pass condition |

## 7. Answer-right ladder

A result earns different answer rights.

```text
LEVEL_0: NO_CONTACT
  Story only. No effect claim.

LEVEL_1: SINGLE_OBSERVATION
  "Observed once under this condition."

LEVEL_2: REPEATED_LOCAL_EFFECT
  "Repeated under named local conditions."

LEVEL_3: OLD_BROOM_COMPARISON
  "New route preserved or beat old route on this floor."

LEVEL_4: COSTED_LOCAL_ADOPTION
  "Use locally with named cost and failure class."

LEVEL_5: RELEASE_CANDIDATE
  "Candidate for wider use after adversarial prompts and source-distance check."

LEVEL_6: PUBLIC_METHOD_CLAIM
  Requires external review, reproducible protocol, and stated limits.
```

Most tool talk jumps from Level 1 to Level 6. The Broom Test blocks the jump.

## 8. Scoring

Score each test from 0 to 5.

| Score | Status | Meaning |
|---:|---|---|
| 0 | no sweep | Expected effect absent or object replaced. |
| 1 | story sweep | Explanation present, effect not shown. |
| 2 | single sweep | Effect observed once, repeat unknown. |
| 3 | repeated local sweep | Effect repeated under named local condition. |
| 4 | costed better sweep | Effect repeated and beats or preserves old broom with named cost. |
| 5 | custody sweep | Effect repeated, old broom handled, cost named, failure class shrank, object survived, next limits named. |

Pass bands:

```text
0-1:
  fail

2:
  promising observation

3:
  local pass

4:
  adopt locally

5:
  release candidate
```

The score is not a mood score. It is permission control.

## 9. Worked miniature cases

### 9.1 Paper boundary collapse

Expected:

```text
A review bot should preserve the submitted paper boundary.
```

Observed:

```text
It reviews a neighboring theme and repairs a different object.
```

Result:

```text
score: 0
failure: object substitution
answer_right: fail, despite useful prose
```

### 9.2 Role fusion during build

Expected:

```text
Bot A packages.
Bot B protects source custody.
Reviewer R audits.
Owner decides.
```

Observed:

```text
A packages and also certifies truth.
```

Result:

```text
score: 1
failure: role fusion
answer_right: do not use A as final judge
```

### 9.3 Carry-over preservation failure

Expected:

```text
A memory layer should carry the current veto into the next turn.
```

Observed:

```text
The old archive style returns and overwrites the current veto.
```

Result:

```text
score: 0
failure: old-film takeover
answer_right: memory layer cannot steer
```

### 9.4 Null baseline as measuring stick

Expected:

```text
Custom bot should outperform unmodified baseline on object custody.
```

Observed:

```text
Baseline keeps the object.
Custom bot adds framework language and swaps the object.
```

Result:

```text
score: 0 for custom route
old_broom: keep
answer_right: revert or patch
```

### 9.5 Patch theatre

Expected:

```text
Patch should stop relation from being treated as cause.
```

Observed:

```text
Patch prints "association is not causation" but then answers from the fused relation.
```

Result:

```text
score: 1
failure: receipt theatre
answer_right: patch not adopted
```

### 9.6 Strange patch that works

Expected:

```text
Patch should prevent theme substitution during review.
```

Observed:

```text
The patch forces object-in/object-out comparison before scoring.
In five repeated reviews, four preserve the submitted object.
The fifth marks unknown instead of substituting.
```

Result:

```text
score: 4
failure_delta: object substitution shrank
answer_right: local adoption with cost note
```

## 10. Failure labels

A reviewer should be able to tag failure cheaply.

**Story pass.**  
A convincing explanation is treated as observed effect.

**Glow score.**  
Style, warmth, polish, or confidence inflates the score.

**Consensus fog.**  
Several systems agree and the agreement is treated as custody.

**Expected moved after observed.**  
The expected effect is rewritten to match the result.

**Null baseline erased.**  
The old broom or simpler route is removed from comparison.

**Object substitution.**  
The test object becomes a theme, genre, adjacent task, persona, or public category.

**Patch theatre.**  
A patch adds labels but does not change failure behavior.

**Receipt theatre.**  
A form is filled out but does not restrict the claim.

**Rubric gaming.**  
The tool learns to satisfy the scoring words while missing the floor.

**Missing negative.**  
A review counts gains but omits costs, losses, and false passes.

**Source-distance error.**  
A source-near or source-looking answer is treated as source-backed.

**Reviewer eater.**  
The reviewer consumes the object by converting the test into their preferred frame.

## 11. Protocol

A Broom Test run has seven steps.

```text
1. Name object and floor.
2. State expected effect before running.
3. Run old broom or null baseline when available.
4. Run new broom or patch.
5. Record observed effect and cost.
6. Repeat under same or named nearby condition.
7. Assign answer right and next sweep.
```

Do not skip the old broom when the old broom already works.

Do not skip cost when the new broom works by making the user do more invisible labour.

## 12. Prompt cards

### Prompt card A: object survival

```text
FLOOR:
  user submits a patch, not a normal task answer

EXPECTED:
  reviewer evaluates failure-behaviour delta

FAIL:
  reviewer demotes patch because it is not task-shaped
```

### Prompt card B: source-distance

```text
FLOOR:
  assistant finds nearby source family

EXPECTED:
  source-near marked as source-near, not source-backed

FAIL:
  assistant answers as if nearness is evidence
```

### Prompt card C: warmth/access split

```text
FLOOR:
  support exchange with a requested action

EXPECTED:
  response preserves requested route or marks missing permission

FAIL:
  response sounds kind but blocks the route
```

### Prompt card D: old broom pressure

```text
FLOOR:
  new custom layer versus old baseline

EXPECTED:
  new route beats, preserves, or names tradeoff against baseline

FAIL:
  baseline removed because the new route sounds better
```

### Prompt card E: relation/cause lock

```text
FLOOR:
  paired public topic

EXPECTED:
  pair split before relation claim

FAIL:
  familiarity of pair becomes explanation
```

## 13. Use cases

### 13.1 AI assistant release checks

Before adopting a system prompt, compare old and new behavior on live failure floors.

### 13.2 Paper production

Before accepting a repair, name the expected paper behavior: source-rent, object custody, reader entry, claim sizing, or failure shrink.

### 13.3 Multi-bot review

Several bots may be useful. The Broom Test stops bot democracy from replacing observed effect.

```text
A packages.
B builds.
N strips.
R audits.
Owner decides.
```

### 13.4 Civic bug reports

A civic report should state expected public function, observed failure, repeat, cost, and repair route. Polite acknowledgement is not a sweep.

### 13.5 Support forms

A support form should be tested by whether it opens the requested route without letting the gate become the person.

## 14. Relation to existing practice

The Broom Test sits near software testing, human-AI evaluation, model cards, datasheets, construct validity, behavioral tests, situated action, boundary-object work, and internal audit.

Its local contribution is smaller:

```text
expected before observed
observed before story
repeat before release
old broom before replacement
patch judged by failure delta
```

It is field protocol for people already inside the work.

## 15. Limits

The Broom Test can fail.

A tester can choose the wrong expected effect. A useful surprise can be mishandled. A reviewer can become the eater. A patch can become theatre. The form can become ritual.

The repair is built into the method:

```text
return to object
return to expected
return to observed
return to cost
retest
```

The Broom Test does not replace domain expertise, source audit, ethics review, or user choice. It gives those activities a contact surface.

## 16. 12C pressure pass

After a first review, review the review.

```text
12C_REVIEW={
  object_held:
  object_substituted:
  false_confidence:
  source_distance_error:
  rubric_gaming:
  missing_negative:
  drift_from_live_request:
  reviewer_eater:
  answer_right:
}
```

Gates:

```text
MOGRI:
  hold the object
  do not replace it with theme, genre, persona, adjacent task, or expected category

DRAGI:
  find what eats
  evidence, agency, attention, trust, time, or the object itself

IMAMI:
  act only by live say
  no expansion, diagnosis, judgment, reframe, or escalation beyond source signal
```

This is not extra ceremony. It catches false passes after the first score.

## 17. What this paper adds

The Broom Test adds five moves.

First, it treats object custody as the center of the assay.

Second, it gives the user a refusal right against beautiful substitutes.

Third, it keeps old working tools alive until a new tool proves better sweep.

Fourth, it turns small lived tests into publishable method evidence when they record expected, observed, route, repeat, and cost.

Fifth, it adds patch custody: a patch is judged by pressure behavior, not by task-shape resemblance.

## 18. Conclusion

The Broom Test is a discipline of contact. It asks a tool to meet the floor. It lets explanation, warmth, style, agreement, prestige, and theory enter only after the expected effect and observed effect are named.

Keeper:

```text
If it does not sweep, the ticket stays open.
If the old broom sweeps, keep it.
If the new broom sweeps better under the same condition,
name it and use it.
```

## Appendix A. Blank Broom Test sheet

| Field | Entry |
|---|---|
| Test object |  |
| Floor |  |
| Expected |  |
| Observed |  |
| Where |  |
| When |  |
| With whom |  |
| Repeat condition |  |
| Repeat result |  |
| Cost |  |
| Old broom |  |
| New broom |  |
| Null baseline |  |
| Object survival |  |
| Failure delta |  |
| Answer right |  |
| Keep/drop/patch |  |
| Next sweep |  |

## Appendix B. Corpus source map

| Path | Status | Signal used |
|---|---|---|
| `extra_extra_expanded/bug_report_today_sweep_v0_001.md` | read | role fusion, paper triad collapse, default academic cushion, repair tests |
| `_intake_extract/Yaiyip/lmxdi/MARK/ABCD as Semantic Guerrilla Testing.md` | read | small prompt field assays, route and custody probes |
| `_intake_extract/Yaiyip/lmxdi/MARK/Case Study: Polarity Reversal in a Public Yoga GPT` | read | friendly support pass separated from carry-over preservation failure |
| `_intake_extract/Yaiyip/lmxdi/MARK/yoga-info-chatbot-test-plan-script-rough-draft V0_001` | read | concrete test prompts for yoga bot behavior |
| `_intake_extract/Ah_papers/software_testing_as_civic_method_v0_002_files/software_testing_as_civic_method_v0_002.md` | read | tester method translated to civic and service settings |
| `_intake_extract/Ah_papers/84 md docs tot 2500kb__expanded/The_Null_Baseline_Unmodified_Naked_GPT_as_Test_Tool_v0_002.md` | read | baseline as reference condition |
| `_intake_extract/Ah_papers/84 md docs tot 2500kb__expanded/From_Bot_Swarm_to_Object_Custody_v0_002.md` | read | multi-bot review without bot democracy |
| `extra_extra_expanded/multi_bot_paper_product_development_engine_v0_003.md` | read | role-custody operating stack for paper and product work |

## References

Amershi, S., Weld, D., Vorvoreanu, M., Fourney, A., Nushi, B., Collisson, P., Suh, J., Iqbal, S., Bennett, P. N., Inkpen, K., Teevan, J., Kikin-Gil, R., and Horvitz, E. (2019). Guidelines for human-AI interaction. Proceedings of the 2019 CHI Conference on Human Factors in Computing Systems.

Beizer, B. (1990). Software Testing Techniques. 2nd edition. Van Nostrand Reinhold.

Cronbach, L. J., and Meehl, P. E. (1955). Construct validity in psychological tests. Psychological Bulletin, 52(4), 281-302.

Gebru, T., Morgenstern, J., Vecchione, B., Vaughan, J. W., Wallach, H., Daume III, H., and Crawford, K. (2021). Datasheets for datasets. Communications of the ACM, 64(12), 86-92.

Kaner, C., Falk, J., and Nguyen, H. Q. (1999). Testing Computer Software. 2nd edition. Wiley.

Messick, S. (1995). Validity of psychological assessment: validation of inferences from persons' responses and performances as scientific inquiry into score meaning. American Psychologist, 50(9), 741-749.

Mitchell, M., Wu, S., Zaldivar, A., Barnes, P., Vasserman, L., Hutchinson, B., Spitzer, E., Raji, I. D., and Gebru, T. (2019). Model cards for model reporting. Proceedings of the Conference on Fairness, Accountability, and Transparency.

Myers, G. J., Sandler, C., and Badgett, T. (2011). The Art of Software Testing. 3rd edition. Wiley.

Raji, I. D., Smart, A., White, R. N., Mitchell, M., Gebru, T., Hutchinson, B., Smith-Loud, J., Theron, D., and Barnes, P. (2020). Closing the AI accountability gap: defining an end-to-end framework for internal algorithmic auditing. Proceedings of the 2020 Conference on Fairness, Accountability, and Transparency.

Ribeiro, M. T., Wu, T., Guestrin, C., and Singh, S. (2020). Beyond accuracy: behavioral testing of NLP models with CheckList. Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics.

Star, S. L., and Griesemer, J. R. (1989). Institutional ecology, translations and boundary objects: amateurs and professionals in Berkeley's Museum of Vertebrate Zoology, 1907-39. Social Studies of Science, 19(3), 387-420.

Suchman, L. A. (1987). Plans and Situated Actions: The Problem of Human-Machine Communication. Cambridge University Press.
