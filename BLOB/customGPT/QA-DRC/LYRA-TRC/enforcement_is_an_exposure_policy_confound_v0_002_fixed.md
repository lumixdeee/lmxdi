# Enforcement Is an Exposure

## Policy contact as a confound in cannabis-psychosis claims

**Version:** v0.002  
**Date:** 2026-07-06  
**Status:** method paper draft for review  
**Author lane:** lumixdeee with QA-DRC  
**Scope:** exposure-routing method for drug-outcome claims made inside active policy fields. Personal, medical, legal, and live-care decisions need their own route.

## Abstract

Cannabis-psychosis arguments often treat cannabis as the exposure and enforcement as the scenery. In a drug-war field, that split is not earned.

Criminalization, policing, search, arrest, family response, school discipline, housing threat, employment threat, service surveillance, forced disclosure, diagnostic expectation, media alarm, and hospital routing can change product route, disclosure route, service route, and recorded outcome. Enforcement is therefore an exposure.

This paper gives a route instrument for reading cannabis-psychosis claims when policy contact is active. The instrument separates body input, product identity, prior state, contact field, service route, measurement route, and policy field before allowing a body-only sentence to grow. Two UK checks show why this matters: Frisher et al. did not find the predicted population rise in diagnosed schizophrenia or psychoses during a period of rising cannabis use, and Hamilton et al. found hospital admissions for cannabis psychosis moved across UK reclassification in a direction that does not fit a simple body-only story.

Those findings do not settle every biological route. They do something more useful for method: they break the naked exposure. A cannabis-psychosis claim inside a shifting enforcement system cannot be trusted as a body-only relation unless enforcement, service contact, diagnostic capture, admission route, and policy messaging are modeled or named as absent.

Keeper:

```text
If changing the law changes the measured syndrome,
then the law is part of the exposure.
```

## 0. One-minute operator

Do not start with:

```text
cannabis -> psychosis
```

Start with this receipt:

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
  earned_claim:
  forbidden_jump:
}
```

Allowed output:

```text
This study estimates a recorded route in a policy field.
```

Blocked output:

```text
The broad public pair becomes a body-only cause object.
```

## 1. The object problem

A study can say "cannabis exposure" while measuring many things at once.

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
  policing status;
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

A paper may still use broad categories. It must then pay the category debt. It must show what the category can carry and where it loses custody.

## 2. Enforcement as exposure

Enforcement is often placed in the scenery. The person uses cannabis, the body reacts, the clinic records the episode, and the paper analyzes the record. That story leaves out the institution that made the category visible.

In a drug-war setting, enforcement can act before, during, and after the body episode.

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

These are not decorations. They are routes.

A body-only model says:

```text
cannabis -> psychosis
```

A route model says:

```text
body_input
+ product_identity
+ timing
+ prior_state
+ co_substances
+ sleep
+ social defeat
+ enforcement_contact
+ service_contact
+ diagnostic_capture
= measured_category
```

Cannabis may be one input. Enforcement may be another. The measured category may be their compound.

## 3. The H0 gate

Every drug-policy-era study should state a policy H0 before moving to causal language.

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

Most papers do not. They import law as background. That is not a neutral move. It is a hidden model.

Short form:

```text
No enforcement measure,
no body-only causal object.
```

This does not mean no body route exists. It means the body route has not earned isolation from the policy field.

## 4. Field split table

A cannabis-psychosis claim needs its field split before its sentence grows.

| Field | Object | What can go wrong if fused |
|---|---|---|
| Body input | product, dose, route, timing, co-use, sleep | broad word carries chemistry it never named |
| Person route | prior state, trauma, vulnerability, pain, sleep, self-medication | prior route is rewritten as later drug effect |
| Enforcement route | law, police contact, search, arrest, forced disclosure | policy contact hides inside exposure and outcome |
| Service route | referral source, admission threshold, bed pressure, repeat contact | service event is treated as disease incidence |
| Measurement route | self-report, diagnosis, hospital code, family report | visibility becomes biology |
| Public route | media alarm, campaign language, family belief field | public story becomes study object |

The field split does not reject a claim. It gives the claim a route to stand on.

## 5. Population check

A broad public claim often implies a population pattern.

```text
large rise in cannabis use
=> later large rise in diagnosed schizophrenia or psychoses
```

Frisher et al. examined this prediction in UK general practice data from 1996 to 2005. Earlier modeling expected incidence and prevalence to rise from 1990 onward if the cannabis-schizophrenia relation had the projected population footprint. The observed data did not show that pattern. Schizophrenia prevalence decreased, psychoses prevalence did not rise across the full period, and incidence did not show the predicted rise.

This is not a zero-effect proof. It is a population-pressure test against the simple object.

The result asks for a smaller claim:

```text
not:
  cannabis causes psychosis as a broad public object

but:
  some routes, products, timings, bodies, and contexts
  may contribute to some measured categories
  under specified conditions
```

That smaller claim may survive. The broad object does not get custody by slogan.

## 6. Reclassification check

The UK reclassification episode gives a second route test.

Cannabis moved from Class B to the less punitive Class C in 2004, then returned to Class B in 2009. Hamilton et al. examined hospital admissions for cannabis psychosis across that period. They found a statistical relation between reclassification and admissions, but in the opposite direction predicted by a simple cannabis-to-admission story. Admissions declined after movement to Class C and rose after return to Class B. The authors did not claim a simple mechanism. They noted that the reasons were unknown and that policing or mental-health-system changes could be involved.

This is the route-medicine point.

```text
If legal status changes and admission categories move,
then legal status is not background.
```

A hospital-admission category is not naked incidence. It is a compound of episode, family action, police action, clinician expectation, bed threshold, coding practice, and policy climate.

The measured object may be:

```text
episode + admission pathway + label + policy climate
```

not simply:

```text
THC in body -> psychotic disorder
```

The reclassification result does not protect cannabis from biological scrutiny. It protects causal inference from status substitution.

## 7. Admission is not incidence

Hospital admission for "cannabis psychosis" is a service event. It is not the same object as population incidence of psychotic disorder.

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

A named admission category can also become an attractor. When a person in distress is known to use cannabis, the label may become available faster in one policy climate than another. That does not mean the clinician is dishonest. It means the diagnostic field is not sealed from policy.

Custody rule:

```text
admission_label != disease_incidence
admission_label != body_only_effect
admission_label = route_event_until_proven_otherwise
```

A paper may study admissions. It must then call the object "admissions." If it moves from admissions to biology, it must show the bridge.

## 8. Disclosure is not passive measurement

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

## 9. Product identity is not optional

"Cannabis" is not a chemical identity. A causal claim needs product route.

```text
PRODUCT_ROUTE={
  THC level;
  CBD level;
  synthetic cannabinoid contamination;
  tobacco co-use;
  alcohol co-use;
  stimulants or other drugs;
  route of administration;
  frequency;
  sleep context;
  market source;
  medical or informal use;
}
```

Enforcement can also alter product identity. Illicit markets, seizures, availability, price, and product labeling can shape what people actually use. Therefore enforcement may change the body input itself, not only the data trail after use.

A paper that omits product identity while invoking biological mechanism is asking "cannabis" to carry chemistry it has not specified.

## 10. Contact-field diagram

The minimal contact-field model is:

```text
prior_state
  -> cannabis_use
  -> body_episode
  -> family_or_peer_response
  -> police_or_service_contact
  -> clinical_attention
  -> diagnostic_label
  -> recorded_outcome

prior_state
  -> cannabis_use

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

The body-only path is one route inside this map. It is not the map.

A statistical adjustment that includes age, sex, socioeconomic position, and some co-use still may not solve the field. Enforcement contact is not a static trait. It is a moving exposure tied to place, year, race or class position, policing intensity, service design, and policy attention.

## 11. What a paper must measure

A route-qualified paper should not stop at "ever used" or "current user." It should separate at least the following:

```text
BODY_INPUT={
  product;
  potency;
  route;
  frequency;
  timing;
  co_substances;
  sleep_state;
  withdrawal_or_reintroduction;
}

PERSON_ROUTE={
  prior_episodes;
  family_vulnerability;
  trauma_history;
  social_defeat;
  self_medication;
  sensory_overload;
  stress_physiology;
}

ENFORCEMENT_ROUTE={
  legal_status;
  police_contact;
  search_or_arrest_history;
  school_or_work_discipline;
  housing_or_custody_pressure;
  forced_disclosure;
  fear_of_service_contact;
}

SERVICE_ROUTE={
  referral_source;
  admission_threshold;
  clinician_expectation;
  coding_category;
  local_bed_pressure;
  intoxication_or_disorder_distinction;
  repeat_admission_handling;
}

PUBLIC_ROUTE={
  media_event;
  policy_change;
  campaign_language;
  local_warning_climate;
  family_belief_field;
}
```

No single paper must measure everything. But no paper may omit these routes and then sell a body-only object.

Allowed:

```text
This study estimates the relation between a recorded cannabis category
and a recorded admission category in a given policy field.
```

Blocked:

```text
This study proves the public object.
```

## 12. Enforcement claim card

A reviewer should ask for this card before accepting claim size.

```text
CLAIM_CARD={
  noun_pair:
    cannabis / psychosis

  body_input:
    named product, potency, route, dose, frequency, timing, sleep, co-use

  person_route:
    prior state, self-medication, vulnerability, stress, trauma, pain, exclusion

  enforcement_field:
    legal status, police contact, forced disclosure, discipline, housing or work pressure

  service_route:
    referral source, admission threshold, coding practice, clinician expectation

  measurement_route:
    self-report, family report, diagnosis, hospital admission, administrative code

  admission_or_incidence:
    state which object is measured

  policy_period:
    law, campaign, policing, service, or market change named where relevant

  earned_claim:
    record route, route question, product-body route, or intervention route

  forbidden_jump:
    recorded cannabis category becomes body-only cause
}
```

## 13. Falsifiers

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

If those tests fail the enforcement model, say so. If they are not run, the body-only object remains unearned.

## 14. Reading card for cannabis-psychosis papers

Use this card before importing the causal object.

```text
READING_CARD={
  Is cannabis one exposure or several?
  Is product identity measured?
  Is timing measured?
  Is frequency measured?
  Is co-use measured?
  Is sleep measured?
  Is prior state measured?
  Is self-medication tested?
  Is reverse path tested?
  Is enforcement measured?
  Is service contact measured?
  Is disclosure cost measured?
  Is admission separated from incidence?
  Is diagnostic label separated from disease process?
  Is population trend checked?
  Is policy change checked?
  Does the claim size match the measured object?
}
```

A paper can pass some gates and fail others. The answer is not rejection by title. The answer is custody by route.

## 15. Why this is medicine, not evasion

The method does not say "ignore distress." It says name the object that is in front of you.

A person may need sleep, safety, food, companionship, withdrawal support, medication review, crisis care, sensory relief, substance support, protection from coercion, or housing help. A person may also need honest discussion of product, dose, frequency, timing, and co-use.

What does not help is allowing a law label to speak for the body.

Route medicine asks:

```text
What happened?
When?
With what product?
In what body?
In what setting?
With what other substances?
With what sleep?
With what pressure?
Who responded?
Who recorded it?
What label was used?
What action helped?
```

That is not pro-drug or anti-medicine. It is object custody.

## 16. Conclusion

Enforcement is an exposure because policy contact can change the body route, the disclosure route, the service route, and the recorded outcome. A cannabis-psychosis paper that leaves enforcement outside the model is not studying a naked body input. It is studying a body in law, family response, service contact, diagnostic expectation, and public story.

The UK population and reclassification checks do not settle every biological question. They do block the simple object. Rising use did not produce the predicted population rise in diagnosed schizophrenia or psychoses. Reclassification moved hospital admissions for cannabis psychosis in the opposite direction expected by a body-only story. Those are not side notes. They are route failures for the public object.

Rule:

```text
Enforcement is an exposure.
Admission is a route event.
Policy is in the data.
No policy model, no causal-object trust.
```

## Next build

```text
1. Add a DAG figure for body, enforcement, service, and record routes.
2. Add a one-page reviewer worksheet from the reading card.
3. Verify the Frisher and Hamilton claims against full text.
4. Add one non-UK example or state why the paper is UK-method-only.
5. Mark which routes can be measured in existing datasets.
6. Split paper body from appendix material if submitting externally.
```

## References

Frisher, M., Crome, I., Martino, O., & Croft, P. (2009). Assessing the impact of cannabis use on trends in diagnosed schizophrenia in the United Kingdom from 1996 to 2005. *Schizophrenia Research, 113*(2-3), 123-128. https://doi.org/10.1016/j.schres.2009.05.031

Hamilton, I., Lloyd, C., Hewitt, C., & Godfrey, C. (2014). Effect of reclassification of cannabis on hospital admissions for cannabis psychosis: A time series analysis. *International Journal of Drug Policy, 25*(1), 151-156. https://doi.org/10.1016/j.drugpo.2013.05.016

Gage, S. H., Jones, H. J., Burgess, S., Bowden, J., Davey Smith, G., Zammit, S., & Munafo, M. R. (2017). Assessing causality in associations between cannabis use and schizophrenia risk: A two-sample Mendelian randomization study. *Psychological Medicine, 47*(5), 971-980. https://doi.org/10.1017/S0033291716003172

Shakoor, S., Zavos, H. M. S., McGuire, P., Cardno, A. G., Freeman, D., & Ronald, A. (2015). Psychotic experiences are linked to cannabis use in adolescents in the community because of common underlying environmental factors. *Psychiatry Research, 227*(2-3), 144-151. https://doi.org/10.1016/j.psychres.2015.03.041

Hernan, M. A., & Robins, J. M. (2020). *Causal Inference: What If*. Boca Raton: Chapman & Hall/CRC. https://miguelhernan.org/whatifbook

Pearl, J. (2009). *Causality: Models, Reasoning, and Inference* (2nd ed.). Cambridge University Press.

## Archive source note

This v0.002 repair is built from the uploaded v0.001 paper `QA-DRC-enforcement_is_an_exposure_policy_confound_v0_001.md`. Internal paper-family terms are treated as project materials, not external authority.
