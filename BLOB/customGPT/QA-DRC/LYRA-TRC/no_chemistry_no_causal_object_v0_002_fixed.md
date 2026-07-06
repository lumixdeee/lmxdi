# No Chemistry, No Causal Object

## Product identity before cannabis-psychosis causality

**Version:** v0.002-fixed  
**Date:** 2026-07-06  
**Status:** method paper draft for review  
**Author lane:** lumixdeee with QA-DRC  
**Scope:** exposure-naming method for claim sizing. Personal, medical,
legal, and treatment decisions need their own route.

## Abstract

The public cannabis-psychosis sentence often treats **cannabis** as if it
were a stable scientific exposure. It is not. The word can point to plant
category, legal category, survey answer, self-report item, use-disorder code,
street product, regulated extract, resin, flower, concentrate, edible, oil,
biomarker-positive status, market route, or service-visible disclosure.

Those are not one drug.

This paper proposes the **chemistry gate**: a causal-object claim does not
earn product-level language until product identity, delta-9-THC, CBD,
THC:CBD ratio, route, dose, frequency, potency source, tolerance state,
supply pattern, reintroduction, co-exposures, sleep, food, and contact field
are either measured or marked absent.

Existing study findings stay in the record at their earned level. The gate
blocks a different move: promotion from broad label to causal object.

Keeper:

```text
Make the link name the drug.
Then make it name the route.
Then make it name the body state.
```

## 0. One-minute operator

When a paper says:

```text
cannabis -> psychosis
```

run this before accepting the sentence:

```text
PRODUCT_RECEIPT={
  exposure_word:
  product_identity:
  THC:
  CBD:
  THC_CBD_ratio:
  route:
  dose:
  frequency:
  timing:
  tolerance_state:
  supply_pattern:
  co_exposures:
  body_state:
  measurement_source:
  contact_field:
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
cannabis -> psychosis
```

Both nouns hide routes.

"Cannabis" can mean product chemistry, plant identity, legal status, licensed
medicine, street label, smell, possession record, use-disorder code, user
identity, survey answer, or biomarker-positive status.

"Psychosis" can mean acute intoxication presentation, transient reaction,
panic with unusual interpretation, sleep-loss state, first-episode
presentation, hospital admission, diagnostic code, schizophrenia-spectrum
diagnosis, or family report.

A paper may study one of those pairings and write as if it studied all of
them. The chemistry gate blocks that expansion.

```text
plant word != dose
frequency != chemistry
self_report != cannabinoid profile
biomarker positive != current intoxication
diagnostic contact != incidence
```

The method does not throw away association studies. It keeps each study at the
claim size its exposure data can carry.

## 2. The field signal stays, but the object splits

The association field contains real feedstock. Review and meta-analytic work
reports links between cannabis measures and psychosis-related outcomes, with
stronger estimates often reported for heavier use, earlier use, or
high-potency patterns. Controlled THC administration also gives a product-body
contrast case.

Those findings matter. They do not settle the object.

A broad exposure variable can say:

```text
people in this measured category had different outcome rates
```

It cannot by itself say:

```text
this chemical route caused this clinical object
```

The missing middle is exposure identity. A causal sentence needs the drug,
route, dose, timing, body state, measurement route, and alternative routes.

## 3. The chemistry gate

A study has passed the chemistry gate only when it can state, or explicitly
mark absent:

```text
PRODUCT:
  flower, resin, concentrate, edible, oil, oromucosal spray,
  synthetic cannabinoid, mixed product, unknown

CHEMISTRY:
  THC, CBD, THC:CBD ratio, other cannabinoids where available,
  contaminant screen where relevant

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
  stop-start pattern, withdrawal period, return after sleep or appetite
  disruption

CO_EXPOSURES:
  tobacco, alcohol, stimulants, sedatives, prescribed medicines, other drugs

BODY_STATE:
  sleep, food, hydration, stress load, trauma state, neurodevelopmental load

CONTACT_FIELD:
  policing, school or workplace action, family concern, emergency route,
  diagnostic route, service-visible disclosure
```

If those fields are absent, a study may still be useful as a category signal.
It has not earned the simple chemical object.

## 4. Product identity breaks the noun

European drug data show why the noun cannot carry chemistry. The EUDA 2026
cannabis report states that in 2024 average THC content in EU-seized cannabis
resin was 24.6 percent, about twice that of herbal cannabis at 12 percent.

The same product word therefore sits over different chemical distributions
across product type, country, and year.

An exposure label such as "cannabis use" can join together:

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

These routes may have different onset, duration, dosing behavior, social
visibility, market stability, and service-contact pattern. They should not be
collapsed into one object unless the claim is explicitly about a broad category
signal.

## 5. Frequency is not dose

Frequency is often the best available variable. It should stay. But frequency
is not dose.

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

Frequency studies can support bounded statements about association by
frequency or level of use. They do not convert frequency into chemistry.

Earned sentence:

```text
heavier or more frequent reported use is linked with psychosis outcomes
in some study designs
```

Unearned sentence:

```text
a stable cannabis chemical object has been identified
```

The first can be tested. The second still owes product identity.

## 6. Route and bioavailability are not details

Route changes the object. Smoked, vaped, oral, and oromucosal routes do not
have the same onset, peak, duration, titration behavior, or social context.

Sativex gives a useful contrast case. Its product information states the dose
unit, route, active ingredients, and formulation: each 100 microlitre spray
contains 2.7 mg delta-9-THC and 2.5 mg CBD from *Cannabis sativa* L.

That does not make Sativex the target. It makes Sativex a receipt.

A named product says:

```text
what it is
how much THC
how much CBD
by what route
with what dose unit
with what titration pattern
```

A loose association variable often says:

```text
cannabis
```

The difference is not cosmetic. It is the difference between a drug route and
a word.

## 7. Self-report and biomarkers answer different questions

Self-report and biomarkers are both useful. Neither is the whole exposure
object.

Self-report can capture frequency, social use, perceived potency, product
name, age of onset, and use pattern. It can also be shaped by memory, setting,
disclosure pressure, fear of sanction, current state, and the interviewer
relationship.

Urine testing answers another question. A positive THC-COOH result can show
prior exposure, but it does not automatically identify current intoxication,
exact dose, product, route, or time since last use.

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

Enforcement, legality, market route, supply stability, product testing,
disclosure conditions, and service-contact pathways can all alter the measured
field. A user in a regulated medical route may know product, dose, and
titration. A user in an unstable street route may not know product, potency,
ratio, contaminant status, or substitution.

Two UK studies are useful counterweights. Frisher et al. tested whether
increasing cannabis use should have produced increasing diagnosed
schizophrenia or psychoses from 1996 to 2005 and did not find the predicted
population trend. Hamilton et al. found a reclassification/admission pattern
that did not match a simple policy story, with policing and mental-health
system changes among possible explanations.

Those papers do not prove a single alternative route. They show that policy
and service route can enter the measurement field.

```text
law status -> market route -> product knowledge -> supply stability
           -> user disclosure -> service contact -> diagnostic record
```

A chemistry gate that ignores policy can still misname the exposure.

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
withdrawal or rebound sleep/appetite/emotion disturbance
co-use weekend
sleep-debt state
stress-state use
```

into one line called cannabis.

Controlled THC work supports route-specific attention to THC. It does not let
every cannabis word become a THC dose, nor every unusual state become a
chronic psychosis object.

The route has to name the body state it is claiming.

## 10. Claim ladder

The chemistry gate does not make findings vanish. It sorts claim size.

```text
LEVEL_1: CATEGORY_SIGNAL
  "People marked as cannabis users differed from non-users."
  allowed when exposure is broad and marked broad

LEVEL_2: FREQUENCY_PATTERN
  "Heavier or more frequent reported use showed higher estimates."
  allowed when frequency data support it

LEVEL_3: PRODUCT_ROUTE_PATTERN
  "Daily high-potency use, as measured or estimated in this setting,
   was linked to higher odds."
  allowed when product route is named

LEVEL_4: CHEMICAL_ROUTE_CLAIM
  "THC exposure by this route at this dose contributed to this outcome
   pattern."
  allowed only with chemistry, route, dose, timing, comparator, and
  alternative-route work

LEVEL_5: INDIVIDUAL_ATTRIBUTION
  "This person's episode was caused by this exposure."
  requires clinical evidence, timing, alternative-route work,
  co-exposure work, and a separate decision route
```

Most public sentences jump from Level 1 or 2 to Level 4 or 5. That is the
object error.

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
| Supply | absent | broad market | product source / stability named |
| Contact field | absent | named | modeled or stratified |
| Measurement | record treated as object | record type named | measurement route analyzed |
| Claim-size match | overgrown | partly bounded | matches exposure payment |

Interpretation:

```text
0-8:
  category signal only

9-16:
  bounded association claim

17-22:
  product-route claim possible

23-26:
  chemical-route claim may be considered
```

The score is not a truth machine. It is a claim-size grip.

## 12. What would move the paper

The chemistry gate can be beaten by better data. The following would move a
study upward:

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

The gate is therefore not anti-evidence. It is evidence hungry. It tells a
claim what it must pay before it can live at a larger scale.

## 13. Relation to the method line

This paper is the chemistry member of a four-paper method line.

```text
Status-Contaminated Causality:
  status labels must not behave like biological evidence

The Pair Is Not the Object:
  a public noun-pair is not yet a causal object

No Chemistry, No Causal Object:
  the exposure must be named before the link can be trusted

Enforcement Is an Exposure:
  policy and contact fields can become part of the measured route
```

Shared rule:

```text
do not let a familiar sentence become the thing it claims to measure
```

## 14. Conclusion

"Cannabis" is not one chemical quantity. It can be a plant word, a law word, a
street word, a product word, a self-report word, or a biomarker word. A causal
paper has to say which.

The chemistry gate keeps findings at their earned level. It lets frequency
studies remain frequency studies. It lets high-potency studies remain
high-potency studies. It lets THC experiments remain THC experiments. It does
not let the broad word cannabis impersonate product, dose, route, tolerance,
supply, and body state.

```text
Make the link name the drug.
Then make it name the route.
Then make it name the body state.
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

Internal draft sources used for lineage and object terms. Parent folder:
`/mnt/data/extra_extra_expanded/`.

- No Chemistry exposure-state draft.
- No H0 causal-object trust draft.
- Enforcement as exposure draft.
- Confound stack draft.
- Status-contaminated causality v0.004 draft.
- SCH route-custody draft for the compressed cannabis-psychosis pair.
