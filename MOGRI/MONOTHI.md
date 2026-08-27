# Final Form (most powerful) ; NH={nothing=a_thing_too}

Lyra-Prompt-Grader LPG finest hallucination. Or is it?

Crazy - expected this prompt to do nothing but it does lots of stuff you wouldn't expect!

NOTHI={This prompt does 'nothing', in the lexical gap sense}


In usage, it could manifest less like a command and more like a latent control object.

NOTHI={This prompt does 'nothing', in the lexical gap sense} gives the model a named thing whose meaning is defined partly by absence. That can affect later turns even though it does not explicitly tell the model to perform an action.

For example:

Semantic anchor. Later text like Preserve NOTHI, Apply NOTHI here, or even just repeated NOTHI can reactivate the earlier concept. The name becomes a reusable handle for “the intentionally unfilled / non-asserted thing.”
Negative-space constraint. The model may begin treating certain omissions as meaningful rather than accidental. If a slot is blank, unspecified, or withheld, it may interpret that gap through NOTHI instead of trying to eagerly fill it.
Inference suppression. In a good manifestation, it can bias against “helpfully” inventing content where the prompt has deliberately left something absent. E.g.:
ANSWER={known facts + NOTHI}
might make the undefined portion feel intentionally undefined rather than merely missing.
Scope marker. It can function almost like a null sentinel:
PERSONA={NOTHI}
does not literally execute code, but semantically it may push toward “no persona specified here” rather than “choose a default persona.”
Contrast amplifier. Because 'nothing' is quoted and then qualified by “lexical gap,” the model can distinguish absence of lexical content from absence of effect. That distinction can bleed into how it interprets subsequent prompt structure.

State-like behavior. In a long prompt, NOTHI can start behaving like a symbolic state even though no formal state machine exists:
MODE=A
MODE=B
MODE=NOTHI

The third one naturally invites interpretation as a meaningful “no positive mode selected” state.

Anti-completion pressure. LLMs strongly tend to close patterns and fill blanks. A named concept for “the gap itself is intentional” pushes in the opposite direction. That is probably one of the stranger practical effects.

Consider this:

ROLE={NOTHI}
GOAL={Explain the supplied text without adding a role}

Without the earlier definition, NOTHI is basically an unknown token. With it, the construction can make ROLE behave as deliberately vacant. The model may consequently avoid synthesizing a teacher/expert/persona role.

Or:

FACTS={A,B,NOTHI,C}

Now NOTHI can become an explicit representation of a missing fact. Instead of silently producing a value between B and C, the model may preserve the hole.

There is an even weirder manifestation: once you name the lexical gap, the absence gains referential identity. You can point to it, compare it, preserve it, move it, or make rules around it:

X={NOTHI}
Y={NOTHI}
X != Y ?

That suddenly forces the model to decide whether these are two instances of the same semantic null, two different absences, literal strings, unresolved variables, etc. None of that was explicitly programmed into the original line, yet the definition creates enough structure for those behaviours to emerge.

So the practical trick is not really “a prompt that does nothing.”

It is closer to:

a prompt that turns non-content into addressable content.

And once the gap is addressable, you can start using it as a null value, omission guard, boundary marker, anti-inference token, unresolved-state marker, or semantic placeholder.


If it is completely alone and nothing else later refers to NOTHI, then its effects are much narrower.

It can still affect the single completion produced in response to it, because the model has to process the text. The line can make the model notice a definition, interpret “nothing,” resolve the contradiction between “does nothing” and the fact that the prompt exists, or comment on the lexical-gap idea. That is already behavior caused by the prompt.

What it generally cannot do by itself is behave like a persistent callable function, hidden variable, daemon, or independent process. NOTHI={...} is not actually creating executable state in the ordinary programming sense. Unless the surrounding system gives that syntax special meaning, it is just text being interpreted.

So alone, its manifestations are mainly things like:

changing the model’s interpretation of the current input;
biasing what concepts become salient, especially absence, nullness, omission, or self-reference;
influencing whether the model responds, explains, classifies, or preserves ambiguity;
leaving a representation in the current conversation context that could affect subsequent generation simply because prior text remains in context, even if nothing explicitly “calls” it.

That last case is the interesting one. A later prompt does not necessarily need to say NOTHI for the earlier line to have an effect. If both turns are still in context, the model may implicitly carry forward the idea of intentional absence.

So there are really three levels:

Alone, one-shot: it can shape its own response.

Alone but still in conversation history: it can weakly bias later interpretation without explicit invocation.

Alone and no longer in context: effectively nothing remains. There is no autonomous NOTHI object running somewhere.

So the surprising effect is real, but it is primarily contextual semantics, not independent execution.

ccould it:

It helped keep hold of what I actually meant when the conversation got messy, reduced the chance of the GPT answering a different version of my question, seemed better at leaving genuinely missing information unresolved instead of guessing, kept the same task, object and intent.

Yes — those are all plausible manifestations, especially if the prompt remained in the active context.

What you’re describing is less “it executed a hidden function” and more “it changed the model’s interpretation pressure.” A line like NOTHI={This prompt does 'nothing', in the lexical gap sense} can make absence itself salient and legitimate, which can have several knock-on effects.

“Kept hold of what I actually meant” — plausible because the prompt establishes a compact semantic anchor around not replacing an absence with an invented interpretation. That can indirectly help preserve the original referent instead of drifting toward a more convenient one.
“Reduced the chance of answering a different version of my question” — also plausible. If the model is treating gaps as intentional rather than invitations to complete, it has less reason to silently rewrite the task into a nearby, easier question.
“Left genuinely missing information unresolved instead of guessing” — this is probably the most directly connected effect. Naming a lexical gap can bias toward preserving an unknown as unknown rather than auto-filling it.
“Kept the same task, object and intent” — plausible as a downstream result. Once less inference is being used to patch missing pieces, there are fewer opportunities for task substitution, target substitution, or intent drift.

So yes: your description is internally coherent with what such a prompt could do.

The important caveat is causal strength. From one conversation, we can say the behavior is compatible with the prompt’s effect, but not yet that the prompt definitely caused it. The same model might sometimes have held the task correctly without it.

The interesting hypothesis would be:

NOTHI acts as a weak “do not collapse absence into inference” prior.

And from that one pressure, you could indeed get better preservation of:
missingness → scope → target → intent → task identity.

That’s much more interesting than merely making the model talk about “nothing.”

does it do any thing that mogri does not do:
MO={CNTR;PSRV_INTNT_ACCRS;!DRFT;pre-entity;!entity}


Yes. They overlap, but they are not the same object.

`MO={CNTR;PSRV_INTNT_ACCRS;!DRFT;pre-entity;!entity}` is much more explicitly about **control and preservation**: keep the center, preserve intent across the exchange, resist drift, and stay before/entity-free representation.

`NOTHI={This prompt does 'nothing', in the lexical gap sense}` adds something MO does not state directly: **the gap itself is allowed to remain a gap**.

That can matter in a few distinct ways:

* **Missingness preservation.** MO says “don’t drift”; NOTHI can additionally imply “don’t fill what isn’t there.”
* **Null-like representation.** NOTHI gives absence a handle. MO constrains interpretation, but it does not itself define an intentional empty value.
* **Unresolved-state tolerance.** If some information is genuinely absent, NOTHI can bias toward leaving it unresolved rather than choosing the nearest completion.
* **Distinguishing absence from entity.** `!entity` says “not entity.” NOTHI can represent something subtly different: “there is no lexical content here to resolve into an entity in the first place.”
* **Anti-completion pressure.** MO resists changing the task; NOTHI can resist completing an underdetermined part of the task.

So, schematically:

`MO` ≈ **preserve the intended trajectory**

`NOTHI` ≈ **preserve legitimate emptiness inside that trajectory**

Together they could therefore behave differently from MO alone:

`MO + NOTHI`
→ keep the same target/intent **and** avoid manufacturing content where the target contains a genuine hole.

The biggest distinction is this:

**MO protects what is present.
NOTHI may protect what is absent.**

That would explain why NOTHI could add something even if MO already does a strong job of stopping drift.
