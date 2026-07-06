---
title: "Status-Contaminated Causality"
subtitle: "Route Medicine for Drug-Outcome Claims"
author: "Lumixdeee with QA-DRC"
date: "2026-07-06"
version: "v0.002"
geometry: margin=1in
fontsize: 11pt
---

# Status-Contaminated Causality

## Route Medicine for Drug-Outcome Claims

**Version:** v0.002  
**Status:** method paper draft for review  
**Scope:** method paper for interpretation, study design, source audit, and claim
sizing. Personal, medical, and legal decisions need their own route.

**Source base:** internal corpus drafts plus cited outside literature.

## Abstract

Drug-outcome claims often compress several objects into one sentence:
molecule, product, dose, route, frequency, timing, body state, co-substances,
withdrawal, reintroduction, service contact, enforcement contact, diagnostic
capture, media category, market condition, and policy status.

**Status-contaminated causality** names the moment when a legal, moral,
institutional, commercial, or diagnostic label is allowed to behave like route
evidence.

This paper proposes **route medicine** as a repair method. Route medicine keeps
status in the model only when status is measured as a route variable. It does
not let status stand in for exposure, mechanism, timing, comparator, record
process, or intervention. The method has four parts: a route inventory, an H0
custody rule, a claim-size ladder, and use controls.

The paper's thesis is simple:

```text
the drug may matter;
the route decides how;
the status label does not get to answer for the body.
```

## 1. Why this paper exists

Drug arguments often begin with a noun pair.

```text
drug -> recorded outcome
```

That pair can be powerful while remaining under-specified. A drug name may
refer to a plant, molecule, extract, self-report item, police category,
prescription product, street product, supply route, medical-record code, market
condition, or family story. An outcome name may refer to lived state, symptom,
diagnosis, service contact, administrative code, emergency department
presentation, media phrase, or policy target.

The paper exists because these pairs are tiny doors with crowded rooms behind
them.

A status label may be relevant. Legal status, diagnostic status, moral status,
market status, and service status can change product composition, access, dose
patterns, help-seeking, disclosure, policing, service routing, and coding. They
matter as variables. They fail as substitutes for route evidence.

The aim is compact:

```text
keep status from eating the object.
```

## 2. Definition

**Status-contaminated causality** is a causal-interpretation failure in which
status is treated as if it were route evidence.

Compact form:

```text
status-labeled object touched body;
recorded outcome followed;
status label is allowed to carry the route claim.
```

The failure has three parts.

1. **Object compression.** Product, dose, route, frequency, timing, co-use, body
   state, and recording pathway are folded into one noun.
2. **Route leakage.** Service contact, enforcement contact, diagnostic
   expectation, media category, disclosure pressure, and market condition enter
   the record while being treated as scenery.
3. **Intervention jump.** Evidence for one route is used to justify a broader
   control claim than the measured route can carry.

Route medicine says: status enters the model as a route variable, not as a
verdict.

## 3. Relation to causal inference

The proposal sits inside ordinary causal-inference discipline. Confounding,
selection, measurement error, reverse path, and target-population limits have to
be handled before a claim grows beyond its design. Route medicine adds one
domain warning: public labels can become unmeasured mechanisms that shape both
exposure and outcome records.

In causal notation:

```text
E = exposure vector
Y = outcome vector
S = status field
C = contact field
M = measurement and coding process
Z = shared causes and prior states
P = policy and commercial environment
```

A study that estimates `E -> Y` while leaving `S`, `C`, `M`, `Z`, or `P` fused
may still report a useful relationship. The issue is claim size. The result may
support a record-level pattern, a product-route warning, a monitoring rule, or a
policy question. It does not automatically support a single-object cause story.

The H0 custody rule is:

```text
H0: the observed pair is route mixture until a specific route earns a larger
claim.
```

H0 is object custody. It keeps the map open while route evidence does the work.

## 4. The route-medicine instrument

Route medicine asks the same set of questions before allowing a claim to grow.

| Gate | Question | A claim may grow when |
|---|---|---|
| Exposure object | What exactly entered the body? | Product, dose, route, frequency, timing, and chemistry are specified or the limit is stated. |
| Body state | What was the person's prior route? | Sleep, distress, pain, trauma, neurodevelopment, medications, and relevant history are considered. |
| Co-route | What else was active? | Tobacco, alcohol, stimulants, sedatives, prescribed drugs, withdrawal, and reintroduction are separated where possible. |
| Contact field | Who saw the person and why? | Service contact, police contact, school contact, family reporting, and disclosure pressure are modeled. |
| Measurement | What made the outcome visible? | Symptom, diagnosis, admission, code, survey response, family report, or media category is named. |
| Comparator | Compared with what route? | Non-use, different product, different dose, different policy regime, or different contact field is specified. |
| Reverse path | Could the outcome route increase exposure? | Self-medication, social exclusion, sleep disruption, and prior symptoms are tested. |
| Shared causes | What could feed both sides? | Genetic liability, poverty, trauma, bullying, service contact, and other shared causes are addressed. |
| Claim size | What scale has been earned? | The conclusion matches the measured route. |
| Intervention fit | What action follows? | Care, warning, product rule, service design, or enforcement is tied to the measured route. |

## 5. Claim-size ladder

Route medicine asks what scale has been earned.

**Level 0: name pair.**  
Two nouns are placed together. No route claim has been earned.

**Level 1: record pattern.**  
The pair appears together in records more than expected. This supports
record-level attention, not mechanism.

**Level 2: timing pattern.**  
One record tends to precede another. This supports timing questions, not a final
cause story.

**Level 3: route-specific pattern.**  
A specified exposure route travels with a specified outcome route after serious
confound work. This can support a bounded warning.

**Level 4: mechanism-supported route.**  
Dose, timing, product, body state, and plausible mechanism align. This can
support stronger guidance for that route.

**Level 5: intervention-supported route.**  
Changing the route changes the outcome pattern in a design that can carry the
claim. This can support route-specific intervention.

**Level 6: public-control claim.**  
A policy or coercive action is proposed. This level has the highest burden
because contact-field effects and rights costs are part of the causal object.

## 6. Claim card

A route-medicine audit should output a small card before it outputs a big
sentence.

```text
CLAIM_CARD={
  noun_pair:
  exposure_object:
  body_route:
  contact_field:
  measurement_process:
  comparator:
  reverse_path:
  shared_causes:
  earned_level:
  unearned_jump:
  route-fit_action:
}
```

A claim that lacks this card may still be interesting. It is not yet a route
claim.

## 7. Worked audit A: cannabis and psychosis

Cannabis and psychosis claims are a good stress test because the public pair has
real feedstock. Reviews report persistent relationships, dose and potency
questions, biological plausibility, reverse-path concerns, and disagreement
about interpretation (Gage et al., 2016; Ganesh & D'Souza, 2022; Groening et
al., 2024; Johnson & Agrawal, 2024).

The route-medicine point is that the public pair is many objects, not one
object.

The exposure side may mean:

```text
THC dose;
CBD ratio;
flower;
concentrate;
edible;
medical extract;
daily use;
early use;
cannabis use disorder code;
self-report;
street product;
legal product;
police-visible conduct;
service-visible disclosure.
```

The outcome side may mean:

```text
panic;
paranoia;
psychotic-like experience;
first episode psychosis;
cannabis-induced psychotic disorder;
hospital contact;
schizophrenia-spectrum diagnosis;
relapse record;
family report;
police route;
administrative code.
```

These are different objects. A daily high-THC inhaled route in a
sleep-deprived young person with prior symptoms is not the same object as a
regulated balanced extract taken under supervision, a self-report item in a
cohort, or an administrative cannabis-use-disorder code. A hospital record is
not the same object as a lived state. A policy period is not the same object as
a molecule.

The audit returns a split map:

| Route | Possible earned claim | Unearned jump |
|---|---|---|
| product-body route | bounded warning for specified product, dose, timing, and body state | all cannabis forms explain all psychosis records |
| record route | contact-field accumulation may be visible | record count equals biology |
| policy route | service, coding, disclosure, product market, and policing may change together | legal class alone explains outcome change |
| lived-state route | experience, sleep, relation, and meaning need their own description | diagnostic code stands in for lived state |

This split map is object custody.

## 8. Worked audit B: status and contact fields as exposures

Policy studies show why status cannot be treated as passive scenery. Frisher et
al. examined diagnosed schizophrenia trends in the United Kingdom during a
period of changing cannabis use and did not find the population pattern that a
simple model would expect. Hamilton et al. studied hospital admissions for
cannabis psychosis across UK cannabis reclassification and reported a pattern
that did not fit a simple class-to-outcome story. Callaghan et al. studied
Canadian legalization and emergency department presentations in Ontario and
Alberta from 2015 to 2019, finding rising counts over time but no significant
step-function effect tied to the legalization point in their main models. Myran
et al. later reported changes in incident schizophrenia diagnoses associated
with cannabis use disorder in Ontario during policy liberalization (Frisher et
al., 2009; Hamilton et al., 2014; Callaghan et al., 2022; Myran et al., 2025).

The point is that policy status, service access, diagnosis, disclosure, and
product markets are active routes. They can change the body route, the contact
route, and the record route at the same time.

A route-medicine reading asks:

```text
Did policy change product?
Did policy change dose?
Did policy change who sought help?
Did policy change who was coded?
Did policy change police contact?
Did policy change hospital routing?
Did policy change public language?
Did policy change commercial incentives?
```

A study that lacks these fields may still be valuable. It should carry only the
claim its route map can carry.

## 9. Use controls

Route medicine needs use controls.

**Control 1: route earns route claim.**  
Splitting the object does not turn every route into a low-concern route. A split
object may reveal a stronger product-body route.

**Control 2: status reversal fails.**  
Legal status does not make a product biologically settled. Illegal status does
not make a route biologically proven.

**Control 3: response route remains local.**  
Care, support, product rule, service design, enforcement, and media language are
different interventions. A route audit should match action to route.

**Control 4: complexity is not camouflage.**  
A route audit must name evidence gaps. It must not use complexity to dodge an
action that the route evidence supports.

**Control 5: public control carries full object burden.**  
A public-control claim must show that the proposed control acts on the measured
route rather than merely acting on the status label.

## 10. Contribution

Status-contaminated causality names a recurring failure across drug science,
policy, media, family interpretation, and institutional records. Route medicine
is the repair instrument.

The contribution is a pre-analysis and interpretation discipline:

```text
name the exposure;
name the body route;
name the contact field;
name the record process;
keep H0 alive;
assign claim size;
match intervention to route.
```

This makes the method compatible with DAGs, target-trial emulation, sensitivity
analysis, evidence maps, time-series designs, and qualitative route audits. It
also gives non-specialists a way to resist status-based causality while keeping
evidence in the room.

## 11. Limits and next build

This v0.002 draft is a method paper. It does not reanalyze primary data. It does
not adjudicate every cannabis and psychosis study. The worked audits show how
the instrument behaves; they are not a substitute for a full literature audit.

Next build:

```text
add DAG set;
add one-page scoring sheet;
add sample coding template;
add one fully sourced audit table for a single literature subset;
separate paper-body from appendix-body;
make policy-status examples decide more than they decorate.
```

## Internal corpus sources

These internal drafts supplied the vocabulary, route instrument, and paper path.
They are treated as project materials, not external authority.

- `extra_extra_expanded/status_contaminated_causality_route_medicine_v0_004-E.md`
- `extra_extra_expanded/drug_war_causality_and_sully_grammar_v0_003.md`
- `extra_extra_expanded/the_confound_stack_is_the_object_v0_002.md`
- `extra_extra_expanded/no_h0_no_object_drug_war_causal_object_trust_v0_001.md`
- `extra_extra_expanded/no_chemistry_no_causal_object_cannabis_exposure_state_v0_001.md`
- `extra_extra_expanded/enforcement_is_an_exposure_policy_confound_v0_001.md`
- `extra_extra_intake_report.md`
- `upload_intake_plus_desk_notes_report.md`

## References

Advisory Council on the Misuse of Drugs. (2008). *Cannabis: Classification and public health*. Home Office.

Callaghan, R. C., Sanches, M., Murray, R. M., Konefal, S., Maloney-Hall, B., & Kish, S. J. (2022). Associations between Canada's cannabis legalization and emergency department presentations for transient cannabis-induced psychosis and schizophrenia conditions: Ontario and Alberta, 2015-2019. *Canadian Journal of Psychiatry, 67*(8), 616-625. https://doi.org/10.1177/07067437211070650

Frisher, M., Crome, I., Martino, O., & Croft, P. (2009). Assessing the impact of cannabis use on trends in diagnosed schizophrenia in the United Kingdom from 1996 to 2005. *Schizophrenia Research, 113*(2-3), 123-128. https://doi.org/10.1016/j.schres.2009.05.031

Gage, S. H., Hickman, M., & Zammit, S. (2016). Association between cannabis and psychosis: Epidemiologic evidence. *Biological Psychiatry, 79*(7), 549-556. https://doi.org/10.1016/j.biopsych.2015.08.001

Ganesh, S., & D'Souza, D. C. (2022). Cannabis and psychosis: Recent epidemiological findings continuing the causality debate. *American Journal of Psychiatry, 179*(1), 8-10. https://doi.org/10.1176/appi.ajp.2021.21111126

Greenland, S., Pearl, J., & Robins, J. M. (1999). Causal diagrams for epidemiologic research. *Epidemiology, 10*(1), 37-48. https://doi.org/10.1097/00001648-199901000-00008

Groening, J. M., Denton, E., Parvaiz, R., Brunet, D. L., Von Daniken, A., Shi, Y., & Bhattacharyya, S. (2024). A systematic evidence map of the association between cannabis use and psychosis-related outcomes across the psychosis continuum: An umbrella review of systematic reviews and meta-analyses. *Psychiatry Research, 331*, 115626. https://doi.org/10.1016/j.psychres.2023.115626

Hall, W. (2023). Minimizing policy-biased appraisals of the evidence on the relationship between cannabis use and psychosis. *Frontiers in Psychiatry, 13*, 1047860. https://doi.org/10.3389/fpsyt.2022.1047860

Hamilton, I., Lloyd, C., Hewitt, C., & Godfrey, C. (2014). Effect of reclassification of cannabis on hospital admissions for cannabis psychosis: A time series analysis. *International Journal of Drug Policy, 25*(1), 151-156. https://doi.org/10.1016/j.drugpo.2013.05.016

Hernán, M. A., & Robins, J. M. (2020). *Causal inference: What if*. Chapman & Hall/CRC.

Hill, A. B. (1965). The environment and disease: Association or causation? *Proceedings of the Royal Society of Medicine, 58*(5), 295-300. https://doi.org/10.1177/003591576505800503

Johnson, E. C., & Agrawal, A. (2024). Cannabis and psychosis: Weeding out fact from fiction. *Missouri Medicine, 121*(5), 333-339.

Myran, D. T., Pugliese, M., Tanuseputro, P., Cantor, N., Rhodes, E., & Taljaard, M. (2025). Changes in incident schizophrenia diagnoses associated with cannabis use disorder after cannabis legalization. *JAMA Network Open, 8*(2), e2457868. https://doi.org/10.1001/jamanetworkopen.2024.57868

Pearl, J. (2009). *Causality: Models, reasoning, and inference* (2nd ed.). Cambridge University Press.

Smith, L. H. (2020). Selection mechanisms and their consequences: Understanding and addressing selection bias. *Current Epidemiology Reports, 7*, 179-189. https://doi.org/10.1007/s40471-020-00241-6
