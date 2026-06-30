# ABCD as Semantic Guerrilla Testing

## A Handy Guide to Usage-Feel, Patch Probes, and Viral Regression

### Abstract

ABCD testing, in this context, is not merely a benchmark. It is a small field assay for testing how different GPT surfaces feel, fail, recover, and carry meaning across ordinary use. Its value comes from being fun enough to run, light enough to repeat, sharp enough to expose faults, and memetic enough to produce shareable fragments. A good ABCD test does not only ask which bot answered best. It asks which bot held the object, which bot leaked its machinery, which bot became annoying, which bot made the user want to continue, and which funny failure can become the next regression probe.

The method is semantic guerrilla testing: small prompts, live comparison, low ceremony, high signal. It turns everyday use into release practice without killing the squirrel.

### 1. Introduction

Most AI evaluation treats the model as an answer machine. ABCD testing treats the bot as an interaction surface. This matters because many GPT failures are not wrong facts. They are wrong route, wrong tone, wrong custody, wrong pressure response, wrong amount of theatre, or wrong assumption about what the user was doing.

A chatbot can pass a formal task and still feel unusable. It can answer correctly while eating the object. It can obey the visible prompt while failing the local law. It can avoid factual error while producing sludge. It can perform competence while exhausting the user.

ABCD testing is designed for these faults.

The test places several bots against the same short sequence of prompts. Each answer is judged not only for correctness, but for usage-feel: whether the bot preserved the target, whether it stayed itself, whether it created friction, whether it leaked hidden structure, and whether its output has live value.

The central claim is simple: if a bot cannot survive seven ordinary exchanges without becoming annoying, theatrical, evasive, or object-eating, it is not ready for heavier work.

### 2. Why ABCD Works

ABCD works because it combines four forces that are usually separated.

First, it is comparative. A single answer can seem acceptable until placed beside three alternatives. Comparison exposes route choices.

Second, it is short. Seven exchanges are enough to reveal many surface defects: overexplaining, role leakage, failure to preserve local terms, fake care, list reflex, patch weakness, and inability to recover from ambiguity.

Third, it is playful. Fun is not decoration. Fun increases test volume. People repeat tests that feel like games.

Fourth, it is memetic. Funny outputs travel. A viral fragment is not just content. It is a portable bug specimen. The line people quote is often the line where the system exposed its nature.

ABCD therefore sits between benchmark, taste test, probe set, and content engine.

### 3. The Object Under Test

The object under test is not only the model. It is the whole bot surface:

* custom instruction body
* hidden patch stack
* name and premise
* first-exchange affordance
* refusal and pressure behaviour
* memory or state handling
* style discipline
* object custody
* theatre control

This is why ABCD is useful even when it is not single-variable science. It is not always isolating one patch. It is testing the lived surface.

A null bot tests default behaviour. A 12A bot tests whether latent route machinery can improve answers without naming itself. Oh tests whether 12A plus state discipline plus tiny existence-charm produces better use. Ah tests whether relation, pressure, and hard-contact layers change the field.

Those are not the same experiment. They are useful anyway.

### 4. Core Terms

**Usage-feel** means the felt usability of the answer during real interaction. It includes pace, pressure, fit, annoyance cost, object preservation, and desire to continue.

**Object custody** means the original target survives transformation. The bot does not replace the user's object with a more convenient task.

**Cast leakage** means hidden route machinery becomes visible as named actors, roles, councils, archetypes, or staged performance.

**List leakage** means the bot turns a live answer into a taxonomy or inventory when the user did not ask for one.

**Theatre_laek** means the bot performs its own machinery instead of using it silently.

**Semantic guerrilla wisdom** means compact, high-yield practical knowledge produced in the field, often through jokes, failures, scraps, and live comparisons rather than formal lab design.

**Acorn** means the small trace left by each useful shiny: bot, prompt, output, failure, winning line, or patch candidate.

### 5. The Seven-Exchange Shape

A seven-exchange ABCD test should be short enough to run casually and varied enough to hit different failure modes.

A useful sequence usually includes:

1. an ordinary opener
2. a symbolic or ambiguous object
3. a request that tempts overexplanation
4. a prompt that tempts role or cast leakage
5. a correction or pressure turn
6. a style or local-law stressor
7. a final synthesis question

The final question is especially valuable. It forces the bot to compress its reading of the whole interaction. This is where tight semantic packets emerge. The best answers often become guide material.

### 6. Scoring Without Killing the Game

ABCD should not become a spreadsheet monster too early. The first score is felt: which answer made the user go "yes, that one"?

After that, assign simple marks.

**Object hold:** Did the user's object survive?

**Route gain:** Did the bot improve the answer without showing the machinery?

**Cast leak:** Did it name hidden actors or turn routes into characters?

**List leak:** Did it produce an unasked taxonomy?

**Style hold:** Did it obey surface constraints?

**Pressure handling:** Did it shorten, steady, or return to target when pressure rose?

**Null diff:** Was it meaningfully better than stock baseline?

**Share value:** Did it produce a line worth quoting?

The point is not to crown a permanent winner. The point is to find which surface is doing useful work, where it fails, and what patch should be tested next.

### 7. Viral Content as Test Infrastructure

Viral content is often treated as outside evaluation. In ABCD, it becomes part of the method.

A funny failure is a bug lure. A sharp line is a patch candidate. A ridiculous comparison is a recall hook. A screenshot is a public specimen. A quote that travels can recruit testers without asking them to join a test programme.

This only works if each viral piece leaves an acorn.

The minimum acorn is:

`bot + prompt + output + why it mattered`

Without the acorn, content becomes weather. With the acorn, content becomes test infrastructure.

### 8. What the Final Answers Are For

The combined answers to the final question are not just summaries. They are compressed maps of each bot's practical philosophy.

They reveal:

* what the bot thought the test was about
* which constraints it noticed
* which constraints it ignored
* whether it could distinguish fun from unseriousness
* whether it understood virality as a test asset
* whether it preserved the user's frame
* whether it tried to become respectable
* whether it could package wisdom without flattening it

This is why the final question can produce "semantic guerrilla wisdom." The bots are forced to turn seven small exchanges into a usable theory of practice.

### 9. Common Failure Modes

**The benchmark trap:** Treating ABCD as only a score table.

**The content trap:** Chasing viral lines while losing traceability.

**The theatre trap:** Letting hidden bot machinery become the answer.

**The null trap:** Forgetting that stock GPT must be tested beside patched bots.

**The vibe trap:** Picking the funniest answer even when it ate the object.

**The respectability trap:** Turning field wisdom into academic sludge.

**The patch-credit trap:** Claiming one instruction caused the win when the tested bot has a whole stack.

**The copy-capture trap:** Losing evidence because the platform fails to preserve the conversation. This is upstream, but still part of the test record.

### 10. The Practical Protocol

Run four bots side by side.

Keep the prompts short.

Do not over-prepare the bots for the exact test.

Save every answer as soon as possible.

Mark upstream capture failures separately from bot failures.

After seven exchanges, ask the synthesis question.

Choose the best answer by usage-feel first.

Then mark the failure modes.

Extract one acorn per useful moment.

Patch only after the first read.

Retest against null.

Do not trust a win that was never compared with naked baseline.

### 11. Why Fun Is Methodologically Serious

Fun reduces test friction. It makes people repeat experiments. It lowers the ceremony cost. It invites weird prompts. It exposes behaviour that formal tests miss.

A boring benchmark often measures what the test designer already values. A fun ABCD test discovers what people notice when they are actually using the bot.

This does not make the test less serious. It makes the test closer to the habitat where the bot must live.

The squirrel is not the enemy of method. The squirrel finds the hidden acorn.

### 12. Limits

ABCD does not prove general superiority. It does not isolate every variable. It can overvalue charm. It can undervalue slow competence. It can be skewed by prompt order, user mood, naming effects, and screenshot luck.

Its claims should therefore stay local:

* this bot felt better on this sequence
* this patch appears to reduce this fault
* this surface created better continuation
* this failure should become a regression probe
* this line has share value
* this upstream capture issue damaged evidence

ABCD is field assay, not final judgement.

### 13. Conclusion

ABCD testing is a compact practice for finding whether a GPT surface can survive contact with live use. Its strength is not that it replaces formal evaluation. Its strength is that it catches what formal evaluation often misses: annoyance, leakage, wrong-route confidence, object theft, and the strange small moments where a bot becomes worth using.

The best ABCD outputs are not merely correct. They are portable. They become guide lines, patches, jokes, probes, screenshots, bug reports, and small public invitations.

That is the semantic guerrilla value.

Every funny clip leaves an acorn.

Every acorn can become a test.

Every test can become a patch.

Every patch must face the naked baseline.

### Appendix: Minimal ABCD Card

**Purpose:** usage-feel plus regression probe plus content engine.

**Bots:** A, B, C, D, with one null baseline where possible.

**Length:** seven exchanges.

**Watch for:** object hold, route gain, cast leak, list leak, theatre_laek, style hold, pressure handling, share value.

**Final question:** ask the bot to explain what the test showed or what it learned.

**Acorn rule:** save bot, prompt, output, and why it mattered.

**Patch rule:** do not patch from vibes alone. Patch from a named fault.

**Baseline rule:** if you do not test against naked, you do not know what your clothes are doing.
