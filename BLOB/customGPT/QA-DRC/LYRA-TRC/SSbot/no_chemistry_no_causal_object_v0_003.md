---
title: "No Chemistry, No Causal Object"
subtitle: "Exposure Identity Before Product-Level Drug Claims"
author: "Lumixdeee with QA-DRC"
date: "2026-07-06"
version: "v0.003"
status: "method paper draft; exposure-naming protocol; not medical advice, not legal advice"
---

# No Chemistry, No Causal Object

## Exposure Identity Before Product-Level Drug Claims

**Version:** v0.003  
**Date:** 2026-07-06  
**Status:** method paper draft for review and testing  
**Scope:** exposure-naming method for claim sizing. Personal, medical, legal, and treatment decisions require their own route.

## Abstract

Drug-outcome claims can make a broad exposure word behave like a measured product. In the cannabis-psychosis literature, the word **cannabis** may point to a plant category, legal category, self-report item, use-disorder code, street product, regulated extract, resin, flower, concentrate, edible, oil, biomarker-positive status, market route, or service-visible disclosure.

Those are not one drug object.

This paper proposes the **chemistry gate**: a product-level causal object is not earned until the exposure has a receipt. The receipt must name, measure, or explicitly mark unknown the product identity, delta-9-THC, CBD, THC:CBD ratio, route, dose, frequency, timing, tolerance state, supply pattern, co-exposures, body state, measurement source, and contact field.

The chemistry gate does not erase existing findings. It assigns them to the claim level their exposure data can carry. A broad category variable may support a category signal. A frequency variable may support a frequency pattern. A named high-potency route may support a product-route claim. A measured THC dose may support a chemical-route claim. None of these automatically becomes the whole public object.

Keeper:

```text
Make the link name the drug.
Then make it name the route.
Then make it name the body state.
Then make it state what remains unknown.
```

## 0. One-minute operator

When a paper, policy document, chart note, or public sentence says:

```text
cannabis / psychosis
```

do not accept the exposure word as the drug.

Run the product receipt first:

```text
PRODUCT_RECEIPT={
  exposure_word:
  product_identity:
  chemistry:
    THC:
    CBD:
    THC_CBD_ratio:
    other_cannabinoids:
    contaminants_or_substitution:
  route:
  dose:
  frequency:
  timing:
  tolerance_state:
  supply_pattern:
  reintroduction_or_stop_start:
  co_exposures:
  body_state:
  measurement_source:
  contact_field:
  comparator:
  earned_claim_level:
  forbidden_jump:
}
```

Allowed first move:

```text
The exposure word is broad.
The product route has to be named before the causal object can grow.
```

Blocked first move:

```text
The broad cannabis word stands in for product, dose, chemistry, and route.
```

## 1. Problem

A sentence can be grammatically small and methodologically enormous.

```text
cannabis / psychosis
```

Both nouns hide routes.

**Cannabis** can mean product chemistry, plant identity, legal status, licensed medicine, street label, smell, possession record, use-disorder code, user identity, survey answer, or biomarker-positive status.

**Psychosis** can mean acute intoxication presentation, transient unusual interpretation, sleep-loss state, first-episode presentation, hospital admission, diagnostic code, schizophrenia-spectrum diagnosis, family report, or service contact.

A study may examine one pairing and a public sentence may later speak as if every pairing was studied.

The chemistry gate blocks that expansion.

```text
plant word != dose
frequency != chemistry
self_report != cannabinoid profile
biomarker_positive != current intoxication
diagnostic_contact != incidence
policy_period != molecule
```

The method does not discard claimed associations. It keeps each finding at the claim size its exposure data can carry.

## 2. The object split

The claimed association field contains useful signals. Review, cohort, case-control, genetic, toxicology, potency, and experimental work all contribute different kinds of information. The error begins when different exposure objects are treated as one chemical object.

A broad exposure variable can say:

```text
people in this measured category differed from people outside it
```

It cannot by itself say:

```text
this measured drug route produced this clinical object
```

The missing middle is exposure identity.

The split is simple:

```text
CATEGORY_OBJECT:
  a person is marked as cannabis user, non-user, frequent user,
  cannabis-use-disorder code, or biomarker positive

PRODUCT_OBJECT:
  a specific product type is named, such as flower, resin, edible,
  concentrate, oil, extract, spray, or unknown street product

CHEMICAL_OBJECT:
  THC, CBD, ratio, dose, route, timing, and relevant co-routes are named

BODY_ROUTE_OBJECT:
  the product meets a body state: sleep, food, stress load, tolerance,
  reintroduction, co-exposures, medications, developmental window

RECORD_OBJECT:
  the outcome is a survey answer, clinical note, diagnosis code,
  hospital contact, family report, or administrative record
```

A claim should not move from one object to another without a receipt.

## 3. The chemistry gate

A study passes the chemistry gate only when it can state, or explicitly mark unknown:

```text
PRODUCT:
  flower, resin, concentrate, edible, oil, oromucosal spray,
  synthetic cannabinoid, mixed product, unknown

CHEMISTRY:
  THC, CBD, THC:CBD ratio, other cannabinoids where available,
  contaminant screen or substitution field where relevant

DOSE:
  per event, per day, per week, maximum event, titration pattern

ROUTE:
  smoked, vaped, oral, oromucosal, mixed, unknown

FREQUENCY:
  pattern across time, not only yes/no

POTENCY_SOURCE:
  laboratory measure, product label, police seizure average,
  user estimate, street name, unknown

TOLERANCE:
  new user, occasional user, stable daily user, returning after break,
  escalating use

SUPPLY:
  regulated stable product, variable street product, intermittent access,
  substitution suspected

REINTRODUCTION:
  stop-start pattern, withdrawal period, return after sleep,
  appetite, mood, or routine disruption

CO_EXPOSURES:
  tobacco, alcohol, stimulants, sedatives, prescribed medicines, other drugs

BODY_STATE:
  sleep, food, hydration, stress load, trauma state,
  neurodevelopmental load, prior symptoms, current medicines

CONTACT_FIELD:
  policing, school or workplace action, family concern, emergency route,
  diagnostic route, service-visible disclosure
```

If these fields are absent, the study may still be useful as a category signal. It has not earned the simple chemical object.

## 4. Product identity breaks the noun

A single public word can sit over different chemical distributions.

The same word can cover:

```text
low-THC flower
high-THC flower
resin
concentrate
edible
oil
regulated extract
street product with unknown content
synthetic cannabinoid substitution
mixed tobacco product
```

These routes may have different onset, duration, titration behavior, social visibility, market stability, product knowledge, and service-contact pattern.

A broad category claim is allowed when it remains broad.

```text
EARNED:
  In this dataset, this broad cannabis measure travelled with this broad
  outcome measure.

UNEARNED:
  The broad word cannabis has identified a stable chemical object.
```

That distinction is the gate.

## 5. Frequency is not dose

Frequency is often useful. It should stay. But frequency is not dose.

"Daily use" can describe:

```text
one low-dose evening event
several high-THC sessions
smoked flower with tobacco
vaped concentrate
edible with delayed onset
medical oil
unstable street supply with repeated reintroduction
high-CBD product
low-CBD high-THC product
```

A frequency variable can support a frequency-pattern claim. It cannot, by itself, settle product chemistry.

Earned sentence:

```text
heavier or more frequent reported use was linked with psychosis-related
outcomes in some study designs
```

Unearned sentence:

```text
a stable cannabis chemical object has been identified
```

The first can be tested. The second still owes product identity.

## 6. Route and bioavailability are not details

Route changes the object. Smoked, vaped, oral, and oromucosal routes do not have the same onset, peak, duration, titration behavior, or social context.

A named product gives a receipt:

```text
what it is
how much THC
how much CBD
what ratio
by what route
with what dose unit
with what titration pattern
```

A loose exposure variable often gives:

```text
cannabis
```

The difference is not cosmetic. It is the difference between a drug route and a word.

Sativex is a useful contrast case because its product information states route, dose unit, active ingredients, and formulation. It is not the target. It is an example of receipt-shaped exposure language.

## 7. Self-report and biomarkers answer different questions

Self-report and biomarkers are both useful. Neither is the whole exposure object.

Self-report can capture frequency, social use, perceived potency, product name, age of onset, and use pattern. It can also be shaped by memory, setting, disclosure pressure, fear of sanction, current state, and the interviewer relationship.

Urine testing answers another question. A positive THC-COOH result can show prior exposure, but it does not automatically identify current intoxication, exact dose, product, route, or time since last use.

The repair is not:

```text
replace self-report with urine
```

The repair is:

```text
join report, product data, route data, timing data, and biomarker status
without pretending any one field is the whole drug
```

## 8. Policy shapes chemistry before analysis starts

Policy is not only interpretation. Policy can shape the exposure itself.

Enforcement, legality, market route, supply stability, product testing, disclosure conditions, and service-contact pathways can all alter the measured field. A user in a regulated medical route may know product, dose, and titration. A user in an unstable street route may not know product, potency, ratio, contaminant status, or substitution.

A chemistry gate that ignores policy can still misname the exposure.

```text
law_status
  -> market_route
  -> product_knowledge
  -> supply_stability
  -> user_disclosure
  -> service_contact
  -> diagnostic_record
```

The policy field does not answer the body question. It changes what body questions are even measurable.

## 9. Body state is part of the route

The same product can meet different bodies.

A causal object should not collapse:

```text
first exposure
early titration
dose increase
stable dose
tolerance state
interrupted supply
return after break
withdrawal or rebound sleep/appetite/emotion disruption
co-use weekend
sleep-debt state
stress-state use
```

into one line called cannabis.

Controlled THC work supports route-specific attention to THC. It does not let every cannabis word become a THC dose, nor every unusual state become a chronic psychosis object.

The route has to name the body state it is claiming.

## 10. Claim ladder

The chemistry gate does not make findings vanish. It sorts claim size.

```text
LEVEL_0: NOUN_PAIR
  "Cannabis and psychosis" appear in one sentence.
  No exposure object has been earned.

LEVEL_1: CATEGORY_SIGNAL
  "People marked as cannabis users differed from non-users."
  allowed when exposure is broad and marked broad

LEVEL_2: FREQUENCY_PATTERN
  "Heavier or more frequent reported use showed higher estimates."
  allowed when frequency data support it

LEVEL_3: PRODUCT_ROUTE_PATTERN
  "This product type, potency band, or route in this setting travelled
   with this outcome measure."
  allowed when product route is named

LEVEL_4: CHEMICAL_ROUTE_CLAIM
  "THC exposure by this route at this dose contributed to this outcome
   pattern."
  allowed only with chemistry, route, dose, timing, comparator,
   and alternative-route work

LEVEL_5: INDIVIDUAL_ATTRIBUTION
  "This person's episode was produced by this exposure."
  requires clinical evidence, timing, alternative-route work,
  co-exposure work, and a separate decision route
```

Most public sentences jump from Level 1 or 2 to Level 4 or 5. That is the object error.

## 11. Product identity score

A reviewer can score a claim before accepting causal-object language.

| Field | 0 | 1 | 2 |
|---|---|---|---|
| Product | broad word | product type named | product tested or specified |
| THC | absent | estimated | measured or labeled |
| CBD / ratio | absent | partial | measured or labeled |
| Route | absent | broad route | route and dosing route named |
| Dose | absent | frequency only | event dose or dose range |
| Timing | absent | broad timing | route timing mapped |
| Tolerance | absent | named | modeled or stratified |
| Co-exposure | absent | named | measured or stratified |
| Body state | absent | named | measured or bounded |
| Supply | absent | broad market | product source or stability named |
| Contact field | absent | named | modeled or stratified |
| Measurement | record treated as object | record type named | measurement route analyzed |
| Claim-size match | overgrown | partly bounded | matches exposure payment |

Interpretation:

```text
0-8:
  category signal only

9-16:
  bounded claimed association

17-22:
  product-route claim possible

23-26:
  chemical-route claim may be considered
```

The score is not a truth machine. It is a claim-size grip.

## 12. Four receipts

The gate should decide. These four receipts show the intended movement.

### 12.1 Broad self-report receipt

```text
SOURCE_SHAPE:
  exposure = ever used cannabis / current use / frequency self-report
  chemistry = unknown
  route = partial or unknown
  dose = unknown
  body_state = partial or absent
  contact_field = usually under-modeled

EARNED_LEVEL:
  LEVEL_1 or LEVEL_2

ALLOWED:
  category signal or frequency pattern

BLOCKED:
  chemical-route claim
  individual attribution
```

### 12.2 High-potency case-control receipt

```text
SOURCE_SHAPE:
  exposure = reported high-potency product, daily or near-daily route
  chemistry = estimated from local product categories or market samples
  route = more specified
  dose = still limited
  body_state = partial
  contact_field = still relevant

EARNED_LEVEL:
  LEVEL_3, sometimes approaching LEVEL_4 only if chemistry, timing,
  comparator, and alternatives are stronger

ALLOWED:
  product-route pattern

BLOCKED:
  all cannabis forms as one chemical object
```

### 12.3 Controlled THC receipt

```text
SOURCE_SHAPE:
  exposure = measured THC dose by defined route
  chemistry = specified
  timing = defined
  body_state = selected participants and study setting
  outcome = acute measured state

EARNED_LEVEL:
  LEVEL_4 for the acute experimental route

ALLOWED:
  chemical-route claim inside that experiment

BLOCKED:
  broad cannabis category claim
  chronic diagnosis claim without separate bridge
```

### 12.4 Named medicinal product receipt

```text
SOURCE_SHAPE:
  exposure = named product, dose unit, route, THC, CBD, formulation
  chemistry = specified
  route = specified
  titration = documented
  population = product-specific

EARNED_LEVEL:
  product receipt exists; outcome claim depends on study design

ALLOWED:
  product identity comparison

BLOCKED:
  using the named product as a proxy for every cannabis object
```

These receipts prevent two opposite errors:

```text
broad variable inflated into chemistry
named product inflated into whole category
```

## 13. What would move the field

The chemistry gate can be beaten by better data. The following would move a study upward:

```text
linked product testing
event-level dose diary
route-specific recording
THC and CBD data
biomarker timing
sleep and food logging
co-exposure logging
interruption and return-after-break records
service-contact route records
pre-registered claim ladder
comparison across regulated and unregulated supply routes
```

The gate is therefore not anti-evidence. It is evidence hungry. It tells a claim what it must pay before it can live at a larger scale.

## 14. Relation to the method line

This paper is the exposure-identity member of a four-paper method line.

```text
Status-Contaminated Causality:
  status labels must not behave like biological evidence

The Pair Is Not the Object:
  a public noun-pair is not yet a causal object

No Chemistry, No Causal Object:
  the exposure must be named before the link can grow

Enforcement Is an Exposure:
  policy and contact fields can become part of the measured route
```

Shared rule:

```text
do not let a familiar sentence become the thing it claims to measure
```

## 15. Public-use card

```text
CHEMISTRY_GATE_PUBLIC_CARD={
  What product?
  What chemistry?
  What route?
  What dose?
  What timing?
  What body state?
  What measurement?
  What contact field?
  What claim level?
}
```

Short version:

```text
No chemistry, no chemical object.
No route, no route claim.
No body state, no body-route claim.
No receipt, no upgrade.
```

## 16. Failure labels

**Broad-word upgrade.** A loose exposure word is promoted into a chemical object.

**Frequency-dose swap.** Frequency is treated as if it named dose.

**Potency fog.** A study discusses potency but lacks product-level measurement or source clarity.

**Receipt laundering.** A named product receipt is used to upgrade a broader category claim.

**Biomarker overreach.** Prior exposure evidence is treated as current dose, route, or timing evidence.

**Contact-field invisibility.** Police, school, family, service, or diagnostic visibility shapes the record while being treated as background.

**Body-state erasure.** Sleep, food, tolerance, reintroduction, medications, and stress load vanish from the claimed route.

**Outcome-object collapse.** A lived state, acute state, hospital contact, diagnostic code, and long-term category are treated as the same outcome.

## 17. Conclusion

"Cannabis" is not one chemical quantity. It can be a plant word, a law word, a street word, a product word, a self-report word, or a biomarker word. A causal paper has to say which.

The chemistry gate keeps findings at their earned level. It lets frequency studies remain frequency studies. It lets high-potency studies remain high-potency studies. It lets THC experiments remain THC experiments. It does not let the broad word cannabis impersonate product, dose, route, tolerance, supply, and body state.

```text
Make the link name the drug.
Then make it name the route.
Then make it name the body state.
Then make it state what remains unknown.
Then make it pay rent.
```

## References

American College of Medical Toxicology. (2020). *Interpretation of urine for tetrahydrocannabinol metabolites.* https://www.acmt.net/wp-content/uploads/2022/06/PRS_191101_Interpretation-of-Urine-for-Tetrahydrocannabinol-Metabolites.pdf

Chesney, E., Oliver, D., Green, A., et al. (2024). Assessing cannabis use in people with psychosis. *Psychological Medicine.* https://pmc.ncbi.nlm.nih.gov/articles/PMC10874830/

Di Forti, M., Morgan, C., Dazzan, P., et al. (2009). *The British Journal of Psychiatry, 195*(6), 488-491. https://pubmed.ncbi.nlm.nih.gov/19949195/

Di Forti, M., Marconi, A., Carra, E., et al. (2015). *The Lancet Psychiatry, 2*(3), 233-238. https://pubmed.ncbi.nlm.nih.gov/26359901/

Di Forti, M., Quattrone, D., Freeman, T. P., et al. (2019). *The Lancet Psychiatry, 6*(5), 427-436. https://pubmed.ncbi.nlm.nih.gov/30902669/

D'Souza, D. C., Perry, E., MacDougall, L., et al. (2004). The psychotomimetic effects of intravenous delta-9-tetrahydrocannabinol in healthy individuals. *NPP, 29*, 1558-1572. https://www.nature.com/articles/1300496

European Union Drugs Agency. (2026). *Cannabis: the current situation in Europe.* European Drug Report 2026. https://www.euda.europa.eu/publications/european-drug-report/2026/cannabis_en

Frisher, M., Crome, I., Martino, O., & Croft, P. (2009). *Schizophrenia Research, 113*(2-3), 123-128. https://www.sciencedirect.com/science/article/abs/pii/S0920996409002692

Gage, S. H., Jones, H. J., Burgess, S., et al. (2017). *Psychological Medicine, 47*(5), 971-980. https://pubmed.ncbi.nlm.nih.gov/27928975/

Hamilton, I., Lloyd, C., Hewitt, C., & Godfrey, C. (2014). *International Journal of Drug Policy, 25*(1), 151-156. https://pubmed.ncbi.nlm.nih.gov/23867051/

Hill, A. B. (1965). The environment and disease: association or causation? *Proceedings of the Royal Society of Medicine, 58*(5), 295-300. https://pmc.ncbi.nlm.nih.gov/articles/PMC1898525/

Johnson, E. C., Hatoum, A. S., Deak, J. D., et al. (2021). The relationship between cannabis and schizophrenia: a genetically informed perspective. *Addiction Biology, 26*(6). https://pmc.ncbi.nlm.nih.gov/articles/PMC8492483/

Marconi, A., Di Forti, M., Lewis, C. M., Murray, R. M., & Vassos, E. (2016). *Schizophrenia Bulletin, 42*(5), 1262-1269. https://pubmed.ncbi.nlm.nih.gov/26884547/

National Academies of Sciences, Engineering, and Medicine. (2017). *The health effects of cannabis and cannabinoids: The current state of evidence and recommendations for research.* Chapter 12. https://www.ncbi.nlm.nih.gov/books/NBK425748/

Robinson, T., Ali, M. U., Easterbrook, B., et al. (2022). *Psychological Medicine, 52*(4), 1-11. https://pmc.ncbi.nlm.nih.gov/articles/PMC10317818/

Sativex Oromucosal Spray. (2026). *Summary of Product Characteristics.* electronic Medicines Compendium. https://www.medicines.org.uk/emc/product/602/smpc

von Elm, E., Altman, D. G., Egger, M., Pocock, S. J., Gotzsche, P. C., & Vandenbroucke, J. P. (2007). The STROBE statement. *The Lancet, 370*(9596), 1453-1457. https://pubmed.ncbi.nlm.nih.gov/18064739/

## Source custody notes

Internal draft sources used for lineage and object terms. They are project materials, not external authority.

- No Chemistry exposure-state draft.
- No H0 causal-object trust draft.
- Enforcement as exposure draft.
- Confound stack draft.
- Status-contaminated causality draft.
- Route-custody draft for the compressed cannabis-psychosis pair.
