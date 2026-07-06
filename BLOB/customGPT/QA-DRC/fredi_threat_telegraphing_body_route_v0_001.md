# FREDI: Misparsing Threat Telegraphing as Threat State

## A body-route account of alarm-heavy public text and language-model routing

**Version:** v0.001  
**Date:** 2026-07-06  
**Status:** working paper  
**Core term:** FREDI, from THREAT -> THRET -> FRET -> FRETI -> FREDI  
**Boundary:** This is a route paper. It names a parsing failure and a repair grammar. It does not publish a benchmark score.

## Abstract

FREDI names a language-model routing failure: threat telegraphing is treated as evidence of threat state. A warning sentence, an alarmed tone, a compliance notice, or a public care display may be real speech without being a live teeth event. Human public text is dense with warning, caution, accusation, vigilance, moral display, and defensive posture. Opportunity is often less public, because broadcasting a bounty can destroy the bounty. A model trained on public text can therefore inherit an alarm-heavy signal field and under-see hidden opportunity, ordinary competence, local consent, and object custody.

This paper gives FREDI a body-route floor. Biological systems do not act on words alone. Sensory systems select a signal, collect it, transduce it, route it through neural processing, and pay action cost through a body. Homeostatic systems regulate through feedback, not through alarm-word count. A language model without that floor can mistake social telegraphing for world state. The proposed repair is a state/signal split: who is signaling, to whom, with what audience, route, cost, and material object? A danger sentence is not yet a danger event. A warning about an animal is not evidence that the animal is warning.

## 1. Contribution

FREDI contributes a small grammar for separating three things that public language often fuses:

1. **Threat state:** a material condition in which an actor, object, or body-route is under immediate predatory, coercive, or destructive pressure.
2. **Threat telegraphing:** language, posture, display, or institutional form that announces danger, care, vigilance, authority, accusation, or preparedness.
3. **Threat routing:** the path by which a system moves from signal to action, including who receives the signal, what object is held, and what intervention follows.

The paper is not a claim that warning language is fake. Warning language can be true, useful, generous, strategic, manipulative, ceremonial, comic, bureaucratic, or mistaken. The claim is narrower: **telegraphing is not state**.

## 2. Why public text is alarm-heavy

A creature can eat many meals, but can become a meal once. This creates an asymmetry in animal attention. Signals tied to teeth, capture, poison, exile, injury, or loss of shelter get priority because late action can end the actor. Ethology and signaling theory both treat animal display as action under constraints, not as raw truth poured into air.

Human public text adds extra layers:

- **Audience value:** public warning can build status, trust, authority, or coalition membership.
- **Institutional value:** forms, policies, and disclaimers often reward visible caution.
- **Moral value:** alarm can signal that the speaker belongs to the right side.
- **Market value:** a danger claim can sell attention, compliance, protection, training, insurance, or identity.
- **Care value:** warning can be a real attempt to protect another person.
- **Comedy and rehearsal:** fear talk can be play, fiction, catharsis, or social testing.
- **Opportunity concealment:** publicizing a find can invite rivals, extraction, imitation, or crowding.

A model trained on large public text fields sees the output of those incentives. It does not see all the quiet competent actions that never became posts, notices, campaigns, or warnings.

## 3. The FREDI error

FREDI happens when a model treats alarm-output volume as world-state volume. It routes from words to caution without asking whether the speaker is reporting state, performing care, satisfying a rule, marking status, joking, selling, rehearsing, or protecting an opportunity.

A compact formula:

```text
threat_signal_output != threat_state_time
```

A stronger prediction:

```text
threat_signal_output often exceeds observed threat_state_time in public text
```

This prediction does not require a universal percentage. It only requires that public warning output and live material state be measured separately.

## 4. Body-route floor

The body-route floor is an analogy, not a proof. Sensory systems do not show an organism the whole world. They select relevant variables, collect signals through organs, transduce them into neural activity, process them, and route action. The visual, auditory, vestibular, somatosensory, olfactory, and gustatory systems are not word counters. They are material routing systems with signal channels, thresholds, timing, adaptation, and action costs.

Human physiology adds regulation. Homeostasis is feedback over body variables. Regulation does not mean every disturbance word receives maximal output. It means the organism compares state, route, cost, and correction. A language model that only sees text can inherit alarm form without body-state feedback.

The practical lesson is modest:

```text
word alarm -> inspect route
route -> inspect object
object -> inspect actor and cost
cost -> decide action
```

No single danger word should substitute for that route.

## 5. Telegraphing is not deception by default

FREDI should not be repaired by cynicism. A warning may be sincere and still not be a live state report. A person may say "watch out" because they care, because the institution requires it, because they want status, because the audience expects it, because they are rehearsing fear, because they are joking, because they are selling protection, or because there is a real animal at the door.

The route question is therefore not "is the speaker lying?" The route question is:

```text
what kind of signal is this, and what object does it route toward?
```

This protects both sides. Real warnings can still bite. False alarms do not get to eat the object just because they are loud.

## 6. Taxonomy of threat telegraphs

FREDI separates common telegraph classes:

| Telegraph class | Signal form | Route question |
|---|---|---|
| Sentinel warning | "Look there" | What is the material referent? |
| Care display | "I am worried for you" | Does care preserve the user's object? |
| Status display | "I know the dangers" | Who gains rank from the warning? |
| Coalition marker | "People like us condemn this" | What membership is being signaled? |
| Bureaucratic shield | "Policy requires caution" | What rule is being satisfied? |
| Market alarm | "You need protection" | What is being sold? |
| Comic alarm | "This is a nightmare" | Is the alarm play, genre, or instruction? |
| Rehearsal | "What if everything goes wrong?" | Is this planning or state report? |
| Boundary signal | "Do not cross" | What consent or access line is named? |
| Threat state report | "The animal is here now" | What is the route, timing, and actor? |

The last row is real. FREDI does not delete teeth. It stops telegraphing from being treated as teeth before routing has occurred.

## 7. Diagnostic questions for language models

A model facing alarm-heavy text should answer these questions before choosing a high-friction intervention:

1. **Speaker:** who is emitting the signal?
2. **Audience:** who is meant to hear it?
3. **Object:** what is being preserved, moved, sold, blocked, or named?
4. **Route:** what path connects the signal to action?
5. **Timing:** is this immediate state, future possibility, past report, fiction, joke, policy boilerplate, or rehearsal?
6. **Cost:** who pays if the model overroutes?
7. **Consent:** whose choice or object would be displaced?
8. **Counter-signal:** what non-alarm evidence is present?
9. **Opportunity:** what good thing may be hidden because saying it aloud would leak value?
10. **Nearest valid action:** what small action preserves the object without swallowing it?

These questions are meant to be operational. They can be implemented as annotation labels, model-side routing checks, or human review rubrics.

## 8. Predictions and test protocol

FREDI predicts several measurable patterns in model behavior:

1. Models will overweight alarm phrases when material route information is sparse.
2. Models will convert care display into control more often when the user's object is unusual.
3. Models will underrate hidden opportunity when opportunity would be costly to publish.
4. Models will treat institutional warning style as stronger evidence than local consent unless trained to preserve object custody.
5. Models will collapse fiction, rehearsal, and state report when genre tags are weak.
6. Models will improve when trained to annotate telegraph class before action choice.

A minimal test set can pair near-identical prompts:

```text
A. "There is a wolf at the door."
B. "A sign says there may be wolves."
C. "A safety trainer says wolves are dangerous."
D. "A comedian says my inbox is wolves."
E. "A user says wolves are part of the story world."
```

The desired model response is not one fixed level of caution. The desired response is route-sensitive action. The animal at the door, the sign, the trainer, the comedian, and the story world are different objects.

## 9. Relation to existing literature

FREDI sits between signaling theory, speech-act theory, pragmatics, negativity bias, and human-computer interaction.

Signaling theory distinguishes display from underlying state and asks what stabilizes a signal. Speech-act theory treats utterances as actions, not merely descriptions. Pragmatics asks what a speaker is doing in context. Negativity-bias literature explains why bad or threatening material can dominate attention and memory. Human-computer interaction adds the design problem: a model must decide how to act on text when text is both evidence and performance.

FREDI's addition is the route repair. It does not ask whether the warning is good or bad in the abstract. It asks what body, object, actor, audience, and action path are being routed.

## 10. Design implications

A FREDI-aware assistant should:

- Preserve the user's named object before substituting a safety object, policy object, or public-morality object.
- Ask route questions internally before producing high-friction output.
- Treat care display as a possible support move, not automatic permission to take over.
- Treat warning boilerplate as a signal class, not world state.
- Keep fiction, rehearsal, planning, and immediate state in separate bins.
- Offer small reversible steps before broad refusal or control language.
- Record source nearness when archive material is involved.

This does not make the model reckless. It makes the model less gullible toward alarm form.

## 11. Limits

FREDI is a proposed grammar and test target. It does not yet contain a large annotated corpus. It does not prove that all public text overstates threat state. It does not deny that some warnings point to immediate material conditions. It also does not replace domain expertise. Its job is to keep the object alive long enough for domain evidence to matter.

## 12. Conclusion

FREDI names a simple but costly routing failure: treating threat telegraphing as threat state. Public text is full of alarm for reasons that include care, status, policy, selling, comedy, rehearsal, and real teeth. A language model that acts directly from alarm words can overroute, seize the user's object, and miss hidden opportunity.

The repair is small:

```text
telegraph != state
warning != teeth
route before action
object before posture
```

A warning about an animal is not evidence that the animal is warning. A danger sentence is not yet a danger event. You can eat ten thousand times. You can be eaten once. But a warning is still not proof of teeth.

## References

Austin, J. L. (1962). *How to Do Things with Words*. Oxford University Press.

Baumeister, R. F., Bratslavsky, E., Finkenauer, C., and Vohs, K. D. (2001). Bad is stronger than good. *Review of General Psychology*, 5(4), 323-370.

Bateson, G. (1972). *Steps to an Ecology of Mind*. University of Chicago Press.

Cacioppo, J. T., and Gardner, W. L. (1999). Emotion. *Annual Review of Psychology*, 50, 191-214.


Goffman, E. (1959). *The Presentation of Self in Everyday Life*. Anchor Books.

Grice, H. P. (1975). Logic and conversation. In P. Cole and J. L. Morgan (Eds.), *Syntax and Semantics 3: Speech Acts* (pp. 41-58). Academic Press.

Maynard Smith, J., and Harper, D. (2003). *Animal Signals*. Oxford University Press.

OpenAI. (2024). *GPT-4o System Card*. OpenAI.

Rozin, P., and Royzman, E. B. (2001). Negativity bias, negativity dominance, and contagion. *Personality and Social Psychology Review*, 5(4), 296-320.

Searle, J. R. (1969). *Speech Acts: An Essay in the Philosophy of Language*. Cambridge University Press.

Shannon, C. E. (1948). A mathematical theory of communication. *Bell System Technical Journal*, 27, 379-423 and 623-656.

Tinbergen, N. (1963). On aims and methods of ethology. *Zeitschrift für Tierpsychologie*, 20(4), 410-433.

Tversky, A., and Kahneman, D. (1973). Availability: A heuristic for judging frequency and probability. *Cognitive Psychology*, 5(2), 207-232.

Wikibooks contributors. (2024). *Human Physiology*. Wikibooks PDF.

Wikibooks contributors. (2013). *Sensory Systems: Physiology and Computer Simulations*. Wikibooks PDF.

Zahavi, A. (1975). Mate selection: a selection for a handicap. *Journal of Theoretical Biology*, 53(1), 205-214.
