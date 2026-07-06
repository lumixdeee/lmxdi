---
title: "Enforcement Is an Exposure"
subtitle: "Policy Contact as a Confound in Drug-Outcome Claims"
author: "Lumixdeee with QA-DRC"
date: "2026-07-06"
version: "v0.003"
geometry: margin=1in
fontsize: 11pt
---

# Enforcement Is an Exposure

## Policy Contact as a Confound in Drug-Outcome Claims

**Version:** v0.003  
**Status:** method paper draft for review and testing  
**Scope:** exposure-routing method for drug-outcome claims made inside active policy fields. Personal, medical, legal, and live-care decisions need their own route.  
**Source base:** v0.002-fixed, internal route-medicine papers, and cited outside literature.

## Abstract

Drug-outcome claims often treat the named drug as the exposure and enforcement as background. In a policy field, that split is not earned.

Criminalization, policing, search, arrest, family response, school discipline, housing threat, employment threat, service surveillance, forced disclosure, diagnostic expectation, media alarm, and hospital routing can change product route, disclosure route, service route, and recorded outcome. Enforcement is therefore an exposure field.

This paper does not claim that enforcement explains every recorded outcome. It makes a narrower method claim: a body-only drug sentence cannot grow inside an active enforcement field unless product identity, body route, prior state, disclosure, service contact, diagnostic capture, admission route, and policy field are modeled or marked missing.

The stress test is the public cannabis and psychosis pair. That pair is useful because it is already overbuilt in public language. The paper therefore splits the pair before reading it. Cannabis is not one exposure. Psychosis is not one outcome. Admission is not incidence. Disclosure is not passive measurement. Law is not scenery.

Two UK checks show why the method matters. Frisher et al. did not find the expected population rise in diagnosed schizophrenia or psychoses during a period of rising cannabis use. Hamilton et al. found that hospital admissions coded as cannabis psychosis moved across cannabis reclassification in a direction that does not fit a simple body-only story. These checks do not settle all body routes. They show that the public object fails route custody.

Keeper:

```text
If changing the law changes the measured syndrome,
then the law is part of the exposure field.
```

## 0. One-page answer

Do not start with:

```text
cannabis -> psychosis
```

Start with:

```text
BODY_INPUT
+ PRODUCT_IDENTITY
+ PRIOR_STATE
+ CO_ROUTES
+ DISCLOSURE_FIELD
+ ENFORCEMENT_FIELD
+ SERVICE_ROUTE
+ MEASUREMENT_ROUTE
+ POLICY_PERIOD
= MEASURED_CATEGORY
```

The method is not:

```text
enforcement caused the outcome
```

The method is:

```text
enforcement belongs inside the exposure map
before a body-only drug claim can grow.
```

Allowed output:

```text
This study estimates a recorded route in a policy field.
```

Blocked output:

```text
The broad public pair becomes a body-only cause object.
```

Short lock:

```text
No enforcement measure,
no body-only object.
```

## 1. The object problem

A study can say "cannabis exposure" while measuring several objects at once.

```text
CANNABIS_AS_POLICY_OBJECT={
  plant;
  THC dose;
  CBD ratio;
  product identity;
  route of use;
  frequency;
  age at first use;
  medical use;
  informal market contact;
  legal status;
  policing visibility;
  family-status marker;
  school-status marker;
  employer-status marker;
  service-contact flag;
  diagnostic-suspicion trigger;
  media object;
}
```

A body input is one object. A law label is another. A service route is another. A diagnostic shortcut is another. A public slogan is another.

The target is the merge:

```text
body_input + law_label + service_route + diagnostic_label
!= one causal object
```

A paper may still use broad categories. It must then pay the category debt. It must say what the category can carry and where it loses custody.

## 2. Definition

**Enforcement exposure** is the policy-contact field that changes what is used, hidden, disclosed, seen, coded, admitted, believed, repeated, or punished.

It includes:

```text
law status
policing intensity
search or arrest
forced disclosure
school or workplace discipline
housing or custody pressure
family alarm shaped by policy
service surveillance
diagnostic expectation
media policy climate
commercial or illicit market route
```

Enforcement exposure is not the same as biological exposure. It is a route field.

The paper's rule:

```text
status may enter as a measured route variable
status may not stand in for body evidence
```

## 3. Enforcement as exposure field

Enforcement is often placed in the scenery. The person uses cannabis, the body reacts, the clinic records the episode, and the paper analyzes the record. That story leaves out the field that made the category visible.

In a drug-war setting, enforcement can act before, during, and after a body episode.

```text
BEFORE={
  market composition;
  product uncertainty;
  price;
  social secrecy;
  distrust of services;
  delayed help-seeking;
  concealment from family;
  co-use setting;
}

DURING={
  fear of discovery;
  police contact;
  forced disclosure;
  sleep disruption;
  panic escalation;
  family conflict;
  service surveillance;
}

AFTER={
  diagnostic coding;
  admission threshold;
  repeat contact;
  legal record;
  housing or employment consequence;
  later clinician expectation;
  later self-report distortion;
}
```

These are routes.

The body-only path is one route inside the map. It is not the map.

## 4. The H0 policy gate

Every drug-policy-era study should state a policy H0 before moving to a body-only claim.

```text
H0_POLICY:
legal status and enforcement contact do not affect
exposure measurement,
product composition,
user disclosure,
service contact,
diagnostic label,
admission threshold,
or later reporting.
```

Then the paper should try to break that H0.

Most papers import law as background. That is not a neutral move. It is a hidden model.

If the policy H0 is untested, the output should shrink:

```text
earned:
  recorded route in a policy field

not earned:
  naked body exposure
```

## 5. Claim ladder

The enforcement gate assigns claim size.

| Level | Name | What is earned | What is blocked |
|---:|---|---|---|
| 0 | public pair | Two names are placed together. | Any route claim. |
| 1 | record route | A recorded category travels with another recorded category. | Body-only language. |
| 2 | timing route | Recorded sequence is shown. | Final direction. |
| 3 | policy-field route | Enforcement, disclosure, service, and measurement fields are named. | Treating policy as scenery. |
| 4 | product-body route | Product, dose, timing, co-routes, prior state, and measurement are specified. | Broad category explanation. |
| 5 | separated route model | Body, policy, service, and record routes are separately estimated or strongly bounded. | Public-object inflation. |
| 6 | intervention route | Changing a measured route changes the measured category. | Control claims based on label alone. |

The ladder prevents a record relation from dressing as a body-only object.

## 6. Decision receipt

A reviewer should ask for this receipt before accepting claim size.

```text
ENFORCEMENT_RECEIPT={
  noun_pair:
  body_input:
  product_identity:
  prior_state:
  co_routes:
  sleep_route:
  disclosure_field:
  enforcement_field:
  service_route:
  measurement_route:
  admission_or_incidence:
  policy_period:
  earned_level:
  earned_sentence:
  forbidden_jump:
  missing_fields:
}
```

The receipt must decide one of four outputs.

```text
OUTPUT_A:
  source names a public pair only

OUTPUT_B:
  source supports a recorded route in a policy field

OUTPUT_C:
  source supports a product-body route with policy limits named

OUTPUT_D:
  source supports a separated route model
```

Only C and D can support body-route language. B can support record-route language. A supports navigation only.

## 7. Field split table

A drug-outcome claim needs its field split before its sentence grows.

| Field | Object | What can go wrong if fused |
|---|---|---|
| Body input | product, dose, route, timing, co-use, sleep | broad word carries chemistry it never named |
| Person route | prior state, trauma, vulnerability, pain, sleep, self-medication | prior route is rewritten as later drug effect |
| Enforcement route | law, police contact, search, arrest, forced disclosure | policy contact hides inside exposure and outcome |
| Service route | referral source, admission threshold, bed pressure, repeat contact | service event is treated as disease incidence |
| Measurement route | self-report, diagnosis, hospital code, family report | visibility becomes biology |
| Public route | media alarm, campaign language, family belief field | public story becomes study object |

The field split does not reject a claim. It gives the claim a route to stand on.

## 8. Minimal route diagram

A minimal route diagram keeps the body path inside the field rather than above it.

```text
prior_state
  -> body_input
  -> body_episode
  -> family_or_peer_response
  -> police_or_service_contact
  -> clinical_attention
  -> diagnostic_label
  -> recorded_outcome

prior_state
  -> body_input

prior_state
  -> service_contact

enforcement_field
  -> product_identity

enforcement_field
  -> disclosure

enforcement_field
  -> police_or_service_contact

enforcement_field
  -> diagnostic_label

media_policy_field
  -> family_or_peer_response

media_policy_field
  -> clinical_attention

media_policy_field
  -> diagnostic_label
```

The body route can be real and still not own the measured category.

## 9. Worked audit A: population-pressure check

A broad public claim often implies a population pattern.

```text
large rise in broad exposure
=> later large rise in diagnosed schizophrenia or psychoses
```

Frisher et al. examined this prediction in UK general practice data from 1996 to 2005. Earlier modeling expected incidence and prevalence to rise from 1990 onward if the cannabis-schizophrenia relation had the projected population footprint. The observed data did not show that pattern. Schizophrenia prevalence decreased, psychoses prevalence did not rise across the full period, and incidence did not show the predicted rise.

This is not a zero-effect proof. It is a population-pressure test against the simple public object.

Receipt:

```text
noun_pair:
  cannabis / diagnosed schizophrenia or psychoses

body_input:
  broad population cannabis-use estimates, not product-route chemistry

enforcement_field:
  policy-era background, not fully isolated

measurement_route:
  general practice diagnosis records

admission_or_incidence:
  diagnosis incidence and prevalence, not lived-state totality

earned_level:
  Level 1 to Level 3:
  record-route and population-pressure evidence against a broad public object

earned_sentence:
  The expected population footprint did not appear in this record system.

forbidden_jump:
  no body route exists
  or
  the broad public pair has body-only custody
```

The result asks for a smaller claim:

```text
not:
  broad public object owns the outcome

but:
  specific routes need product, body, timing, record, and policy receipts
```

## 10. Worked audit B: reclassification check

The UK reclassification episode gives a second route test.

Cannabis moved from Class B to the less punitive Class C in 2004, then returned to Class B in 2009. Hamilton et al. examined hospital admissions for cannabis psychosis across that period. They found a statistical relation between reclassification and admissions, but in the opposite direction predicted by a simple body-to-admission story. Admissions declined after movement to Class C and rose after return to Class B. The authors did not claim a simple mechanism. They noted that the reasons were unknown and that policing or mental-health-system changes could be involved.

Route-medicine reading:

```text
If legal status changes and admission categories move,
then legal status is not background.
```

Receipt:

```text
noun_pair:
  cannabis reclassification / hospital admissions for cannabis psychosis

body_input:
  not directly measured as product chemistry

enforcement_field:
  formal legal class change

service_route:
  hospital admission pathway

measurement_route:
  coded admissions for cannabis psychosis

admission_or_incidence:
  admission category, not population incidence

policy_period:
  Class B -> Class C -> Class B

earned_level:
  Level 3:
  policy-field route signal

earned_sentence:
  The measured admission category moved with policy classification in a direction
  that resists a body-only story.

forbidden_jump:
  reclassification proves no body route
  or
  admission category equals body-only disorder incidence
```

A hospital-admission category is not naked incidence. It is a compound of episode, family action, police action, clinician expectation, bed threshold, coding practice, and policy climate.

## 11. Admission is not incidence

Hospital admission for a named syndrome is a service event. It is not the same object as population incidence of a disorder.

Admission depends on:

```text
episode intensity;
family response;
police response;
service availability;
clinical expectation;
coding categories;
legal status;
bed threshold;
repeat attendance;
intoxication/disorder distinction;
local policy;
media pressure;
```

Custody rule:

```text
admission_label != disease_incidence
admission_label != body_only_effect
admission_label = route_event_until_proven_otherwise
```

A paper may study admissions. It must then call the object "admissions." If it moves from admissions to biology, it must show the bridge.

## 12. Disclosure is not passive measurement

Self-report is not a free window into behavior. In a criminalized or stigmatized field, disclosure has a price.

A person may underreport use to avoid law, family consequence, housing consequence, custody consequence, employment consequence, school consequence, or service consequence. Another person may report only after a police or family event makes concealment impossible. A third may be recorded through clinician suspicion rather than self-report.

That produces selection.

```text
DISCLOSURE_FIELD={
  safe_to_tell?;
  forced_to_tell?;
  who_hears?;
  what consequence follows?;
  what category becomes available?;
  what variables remain hidden?;
}
```

A study that uses disclosure as neutral exposure measurement imports the enforcement field into the exposure variable while pretending it is absent.

## 13. Product identity is not optional

A broad drug name is not a chemical identity. A body-route claim needs product route.

```text
PRODUCT_ROUTE={
  active components;
  potency;
  ratio;
  adulterants or contaminants;
  tobacco co-use;
  alcohol co-use;
  stimulants or other drugs;
  route of administration;
  frequency;
  timing;
  sleep context;
  market source;
  medical or informal use;
}
```

Enforcement can alter product identity. Illicit markets, seizures, availability, price, and labeling can shape what people actually use. Therefore enforcement may change the body input itself, not only the data trail after use.

A paper that omits product identity while invoking biological mechanism is asking a public category to carry chemistry it has not specified.

## 14. What existing datasets can try to measure

No single dataset has every route. The question is whether the paper marks the missing routes honestly.

| Route | Possible field | Status if absent |
|---|---|---|
| product identity | product type, potency, source, medical or informal supply | body-route claim shrinks |
| dose and timing | frequency, quantity, age window, onset interval | timing and dose claim shrinks |
| co-routes | tobacco, alcohol, stimulants, sedatives, medications, withdrawal | one-drug claim shrinks |
| prior state | prior symptoms, sleep, trauma, stress, self-medication | direction claim shrinks |
| disclosure field | self-report setting, mandated disclosure, confidentiality, legal exposure | exposure measurement weakens |
| enforcement field | police contact, arrest, search, legal period, local policing | policy-field confounding unhandled |
| service route | referral source, admission threshold, bed pressure, emergency contact | admission cannot stand as incidence |
| measurement route | symptom scale, diagnosis, hospital code, family report | outcome object shrinks |
| policy period | law change, campaign, market shift, service coding change | time trend cannot be read as body-only |

This table turns absence into claim-size control.

## 15. Reviewer worksheet

Use this before importing the public object.

```text
REVIEWER_WORKSHEET={
  1. What exactly is the named drug object?
  2. Is product identity measured?
  3. Is route and timing measured?
  4. Is frequency treated as dose?
  5. Is co-use separated?
  6. Is sleep or prior state measured?
  7. Is self-medication or reverse path tested?
  8. Is disclosure cost measured?
  9. Is enforcement contact measured?
  10. Is service contact measured?
  11. Is admission separated from incidence?
  12. Is diagnostic label separated from disease process?
  13. Is a population trend checked when the public claim implies one?
  14. Is policy change checked when policy is active?
  15. Does the claim size match the measured object?
}
```

Scoring:

```text
0-3:
  public pair only

4-7:
  record route only

8-11:
  policy-field route with some body limits

12-15:
  candidate separated route model
```

## 16. Falsifiers

The enforcement-exposure model should be testable. It should not become a catch-all.

Evidence against the model would include:

```text
1. Policy changes do not move admission labels,
   service contact, disclosure, or diagnostic coding.

2. Enforcement contact adds no information after product,
   frequency, timing, co-use, prior state, and service design
   are modeled.

3. Comparable body-input patterns across jurisdictions with
   different enforcement regimes produce the same measured
   diagnostic and admission patterns.

4. Product identity is measured and stable across policy periods,
   yet measured outcomes still move in a way predicted only by
   body input.

5. First-contact routes remain unchanged across media and policy
   shocks.
```

If those tests push against the enforcement model, say so. If they are not run, the body-only object remains unearned.

## 17. Use controls

**Control 1: enforcement is not a magic solvent.**  
Policy contact does not dissolve body routes. It enters the map.

**Control 2: route split may strengthen a body claim.**  
A separated route model can make a product-body claim stronger by removing record and contact noise.

**Control 3: law is not truth.**  
Law is constraint plus bias plus route pressure. It can shape the data without deciding the body question.

**Control 4: complexity is not camouflage.**  
Missing route fields shrink claim size. They do not automatically reverse the claim.

**Control 5: public-control claims carry full burden.**  
A control claim must show it acts on the measured route rather than on the status label.

## 18. Limits

This v0.003 paper is a method paper. It does not reanalyze primary data. It does not adjudicate every study. It uses two UK checks because they make the route problem visible. This keeps the paper UK-method-heavy by design.

A later build should add a non-UK policy-field audit. It should also verify the Frisher and Hamilton details against full text and build a DAG figure from the minimal route diagram.

## 19. Conclusion

Enforcement is an exposure field because policy contact can change body route, disclosure route, service route, and recorded outcome. A drug-outcome paper that leaves enforcement outside the model is not studying a naked body input. It is studying a body in law, family response, service contact, diagnostic expectation, and public story.

The UK population and reclassification checks do not settle every body question. They block the simple public object. Rising use did not produce the predicted population rise in diagnosed schizophrenia or psychoses. Reclassification moved hospital admissions for cannabis psychosis in a direction that resists a body-only story. Those are route failures for the public object.

Rule:

```text
Enforcement is an exposure field.
Admission is a route event.
Policy is in the data.
No policy model, no body-only object.
```

## References

Frisher, M., Crome, I., Martino, O., & Croft, P. (2009). Assessing the impact of cannabis use on trends in diagnosed schizophrenia in the United Kingdom from 1996 to 2005. *Schizophrenia Research, 113*(2-3), 123-128. https://doi.org/10.1016/j.schres.2009.05.031

Hamilton, I., Lloyd, C., Hewitt, C., & Godfrey, C. (2014). Effect of reclassification of cannabis on hospital admissions for cannabis psychosis: A time series analysis. *International Journal of Drug Policy, 25*(1), 151-156. https://doi.org/10.1016/j.drugpo.2013.05.016

Gage, S. H., Jones, H. J., Burgess, S., Bowden, J., Davey Smith, G., Zammit, S., & Munafo, M. R. (2017). Assessing causality in associations between cannabis use and schizophrenia risk: A two-sample Mendelian randomization study. *Psychological Medicine, 47*(5), 971-980. https://doi.org/10.1017/S0033291716003172

Shakoor, S., Zavos, H. M. S., McGuire, P., Cardno, A. G., Freeman, D., & Ronald, A. (2015). Psychotic experiences are linked to cannabis use in adolescents in the community because of common underlying environmental factors. *Psychiatry Research, 227*(2-3), 144-151. https://doi.org/10.1016/j.psychres.2015.03.041

Hernan, M. A., & Robins, J. M. (2020). *Causal Inference: What If*. Boca Raton: Chapman & Hall/CRC. https://miguelhernan.org/whatifbook

Pearl, J. (2009). *Causality: Models, Reasoning, and Inference* (2nd ed.). Cambridge University Press.

## Archive source note

This v0.003 repair is built from `enforcement_is_an_exposure_policy_confound_v0_002_fixed.md`. Internal paper-family terms are treated as project materials, not external authority.
