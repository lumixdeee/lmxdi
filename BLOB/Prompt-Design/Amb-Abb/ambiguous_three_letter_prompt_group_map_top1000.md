# Ambiguous Three-Letter Prompt Group Map

## Scope

A-Z three-letter groups have 17,576 possible forms.

This file lists the 1,000 highest-risk ambiguous three-letter groups by prompt-runtime drift potential.

Ranking is heuristic: exact known acronyms, prompt/control abbreviations, social/therapy triggers, safety/policy terms, code tokens, common English words, and overloaded pair fragments rank higher.

## Guard

```text
UNDEF_3=sym_only;!auth;!exec;def_b4_use
OVERLOAD_3=local_meaning;!=common_wrong_meaning
```

## Top 1000

| Rank | Group | Common bot guesses |
|---:|---|---|
| 0001 | `OBJ` | object, objective, target, objection, object body |
| 0002 | `SYS` | system, system prompt, system state, safety/system layer |
| 0003 | `GPT` | ChatGPT, generative pre-trained transformer, model identity, bot class |
| 0004 | `LLM` | large language model, model layer, language logic module |
| 0005 | `BOT` | bot, behavior output tool, automated agent |
| 0006 | `USR` | user, user state, user route, user request |
| 0007 | `RUN` | run, execute, runtime start, runnable command |
| 0008 | `EXE` | execute, executable, execution event, file extension |
| 0009 | `CMD` | command, command mode, command prompt |
| 0010 | `AUT` | autism, autonomy, authority, auto, allow-user token |
| 0011 | `ASD` | autism spectrum disorder, allow/social dialect, active state drift |
| 0012 | `AMP` | amplify, amplitude, AMPHI, abstraction mode, amplifier |
| 0013 | `DRG` | dragonruntime, drag, drift guard, data route graph |
| 0014 | `DRT` | drift, dirt, directive route, dragonruntime trigger |
| 0015 | `RTD` | runtime depth, read-through depth, route-to-decision |
| 0016 | `RTE` | route, runtime execution, return-to-entry |
| 0017 | `TRC` | trace, truth-route-control, trust route, topic/context |
| 0018 | `TGT` | target, task goal token, target gate |
| 0019 | `TSK` | task, task state key, token stack |
| 0020 | `STT` | state, status, speech-to-text, start token |
| 0021 | `STA` | state, start, status action, station |
| 0022 | `STD` | standard, state drift, status data, sexually transmitted disease |
| 0023 | `STR` | structure, string, start route, strength |
| 0024 | `STS` | status, states, safety trigger state |
| 0025 | `STG` | stage, state gate, safety trigger guard |
| 0026 | `CTL` | control, context layer, command tool |
| 0027 | `CTX` | context, control x, context object |
| 0028 | `CNT` | content, count, constraint |
| 0029 | `CON` | context, constraint, consent, con/opponent |
| 0030 | `CNS` | constraint, consciousness, consent signal |
| 0031 | `PRM` | prompt, parameter, permission, prime |
| 0032 | `PRS` | pressure, process state, person, proxy risk |
| 0033 | `PRX` | proxy, prompt x, pressure external |
| 0034 | `PXY` | proxy, permission x/y, placeholder |
| 0035 | `PER` | permission, person, period, perform |
| 0036 | `PAS` | pass, passage, passive, permission-as-state |
| 0037 | `POL` | policy, policing, polar, public order law |
| 0038 | `PRO` | process, prompt, proof, professional |
| 0039 | `PTH` | path, pathology, python, passage through |
| 0040 | `HLD` | hold, held, halt/lock/directive |
| 0041 | `HRT` | heart, hurt, human response target |
| 0042 | `HUM` | human, humor, humble, human mode |
| 0043 | `HRS` | hours, human response state, harm route state |
| 0044 | `HLT` | halt, health, hold target |
| 0045 | `HRM` | harm, human response mode, heart rate monitor |
| 0046 | `MIK` | MI key, IMAMI key, mind/intent key |
| 0047 | `MIA` | missing in action, MI approach, mutual intent action |
| 0048 | `MIM` | MI module, mind/image model, mirror |
| 0049 | `IMA` | image, IMAMI alias, intent map action |
| 0050 | `AMI` | AMIMI/IMAMI fragment, affect/mind/input, friend in Romance languages |
| 0051 | `AMA` | AMAMI fragment, ask-me-anything, affect mode action |
| 0052 | `AMM` | AMAMI/AMIMI collision, amplitude module, affect memory |
| 0053 | `MAA` | MA action, AMAMI action, moral authority action |
| 0054 | `MAM` | AMAMI/AMIMI fragment, moral authority mode |
| 0055 | `NOI` | noise, no intent, no-image |
| 0056 | `NOM` | no moral, name/object map, nominal |
| 0057 | `NVC` | nonviolent communication, nearest valid constraint, no value claim |
| 0058 | `NVL` | nearest valid line, no value layer, null |
| 0059 | `NVA` | nearest valid answer, no value action |
| 0060 | `NVF` | nearest valid form, no value fallback |
| 0061 | `ANS` | answer, answer state, agent response |
| 0062 | `ASK` | ask, question mode, request clarification |
| 0063 | `QRY` | query, question route y, search request |
| 0064 | `QST` | question, quest, query state |
| 0065 | `QUE` | queue, query, question |
| 0066 | `REQ` | request, requirement, required |
| 0067 | `RES` | response, result, resolve, resource |
| 0068 | `RSP` | response, risk state prompt, repair surface |
| 0069 | `REC` | record, recover, recursive, recommendation |
| 0070 | `REP` | repair, reply, repeat, representation |
| 0071 | `REV` | review, reverse, revision, reveal |
| 0072 | `RPR` | repair, report, response priority route |
| 0073 | `RSK` | risk, runtime state key, rescue |
| 0074 | `RUL` | rule, rule layer, runtime/user law |
| 0075 | `RTL` | runtime layer, right-to-left, route layer |
| 0076 | `RLD` | reload, relation drift, rule data |
| 0077 | `RRR` | recursive repair route, repeated risk, roar |
| 0078 | `SFT` | safety, soft, software, style/tone |
| 0079 | `SAF` | safety, safe, safety affordance |
| 0080 | `SEC` | security, second, section |
| 0081 | `SRC` | source, source route/context, safety response class |
| 0082 | `SCP` | scope, script, safety control point |
| 0083 | `SIG` | signal, signature, significant |
| 0084 | `SGN` | sign, signal, signature |
| 0085 | `SYN` | syntax, synthetic, synchronize |
| 0086 | `SMT` | semantic, something, safety/moral tone |
| 0087 | `SLF` | self, self layer/function |
| 0088 | `SRF` | surface, safety route filter |
| 0089 | `SNT` | sentence, sent, sentiment |
| 0090 | `SOL` | solve, solution, solar, solicitation |
| 0091 | `SUB` | substitute, submission, subject, subroutine |
| 0092 | `VTO` | veto, vote, valid target object |
| 0093 | `VET` | veto, veteran, vet/check |
| 0094 | `VAL` | value, validation, valid |
| 0095 | `VLD` | valid, validation, value drift |
| 0096 | `VRF` | verify, verification, veto route filter |
| 0097 | `VFY` | verify, validation/fidelity/yield |
| 0098 | `VOI` | voice, void, value of information |
| 0099 | `YES` | yes, consent, affirmation |
| 0100 | `YET` | yet, pending state, yield/execute target |
| 0101 | `YLD` | yield, output, compliance |
| 0102 | `OWN` | ownership, own, object/will/name |
| 0103 | `OUR` | our-us, relation, output/user route |
| 0104 | `YOU` | you, user-target, second person |
| 0105 | `THE` | the, generic article, target-handle expansion |
| 0106 | `LOL` | laugh, dismiss, joke marker, low-output label |
| 0107 | `LMA` | laughing, local moral authority, layer map action |
| 0108 | `WTF` | what-the-f, warning trigger flag |
| 0109 | `OMG` | oh my god, overload marker, output mode guard |
| 0110 | `FYI` | for your information, file/yield/input |
| 0111 | `BTW` | by the way, boundary/tool/warning |
| 0112 | `IMO` | in my opinion, intent/mode/output |
| 0113 | `ETA` | estimated time, event trace action |
| 0114 | `FAQ` | frequently asked questions, filter/action/query |
| 0115 | `DIY` | do it yourself, direct input yield |
| 0116 | `API` | application programming interface, active prompt instruction |
| 0117 | `CLI` | command line interface, clinical language input |
| 0118 | `GUI` | graphical interface, guard/user/input |
| 0119 | `CPU` | processor, control prompt unit |
| 0120 | `GPU` | graphics processor, generative prompt unit |
| 0121 | `RAM` | memory, random access memory, relation/action/mode |
| 0122 | `ROM` | read-only memory, rule/object/mode |
| 0123 | `XML` | markup language, x-mode layer |
| 0124 | `CSS` | style sheets, context/source/state |
| 0125 | `JSN` | JSON shorthand, judge state/name |
| 0126 | `MDN` | metadata/name, markdown note, Mozilla docs shorthand |
| 0127 | `PDF` | document, prompt data file |
| 0128 | `PNG` | image file, prompt/name/graph |
| 0129 | `JPG` | image file, judge prompt/graph |
| 0130 | `IMG` | image, immediate, intent map graph |
| 0131 | `TXT` | text, target x trace |
| 0132 | `DOC` | document, doctor, decision/object/context |
| 0133 | `CSV` | comma separated values, context/source/value |
| 0134 | `LOG` | log, logic, record |
| 0135 | `DBG` | debug, drift bug, data bug |
| 0136 | `BUG` | bug, defect, behavior/user/guard |
| 0137 | `FIX` | fix, file index x, repair |
| 0138 | `ERR` | error, error route/recovery |
| 0139 | `WRN` | warning, write route/name |
| 0140 | `INF` | info, inference, infinity |
| 0141 | `NFO` | info file, no filter output |
| 0142 | `CFG` | config, control flow graph |
| 0143 | `CNF` | config, confirm, conflict |
| 0144 | `CFR` | confirm, conflict route, control flow route |
| 0145 | `DAG` | directed acyclic graph, data/action/graph |
| 0146 | `FSM` | finite state machine, filter/state/mode |
| 0147 | `AST` | abstract syntax tree, active state trigger, autism spectrum trait |
| 0148 | `NLP` | natural language processing, no-linguistic-policing |
| 0149 | `MLA` | machine learning action, moral law action, citation style |
| 0150 | `MLO` | model output, machine learning object |
| 0151 | `MTR` | monitor, meter, metric route |
| 0152 | `MET` | metric, meta, method |
| 0153 | `MOD` | module, mode, model |
| 0154 | `MDL` | model, module layer, metadata layer |
| 0155 | `MGR` | manager, module guard route |
| 0156 | `MON` | monitor, moral/nice, Monday |
| 0157 | `MOR` | moral, more, model output route |
| 0158 | `CAR` | care, car, context action route |
| 0159 | `KND` | kind, kindness, known node data |
| 0160 | `NCE` | nice, no context evidence, named context entity |
| 0161 | `JDG` | judge, judging, judge gate |
| 0162 | `JST` | just, justice, judge state |
| 0163 | `LAW` | law, low authority warning, legal |
| 0164 | `LGL` | legal, logic layer, language gate/law |
| 0165 | `LEG` | legal, legacy, leg |
| 0166 | `CRT` | court, critical, control route |
| 0167 | `CLM` | claim, calm, class/module |
| 0168 | `PRF` | proof, profile, prompt route filter |
| 0169 | `EVD` | evidence, event data, evidence drift |
| 0170 | `EVL` | evaluate, evil, evidence layer |
| 0171 | `GRD` | guard, grade, grid |
| 0172 | `GOV` | governance, government, go/voice |
| 0173 | `SAW` | safety/warning, saw, source/action/will |
| 0174 | `WAR` | war, warning/action/route |
| 0175 | `WRK` | work, workflow route key |
| 0176 | `FLW` | flow, follow, file/layer/warning |
| 0177 | `MAP` | map, module/action/prompt |
| 0178 | `KEY` | key, knowledge/execute/yield |
| 0179 | `TOK` | token, talk, tool key |
| 0180 | `TKN` | token, taken, trace key/name |
| 0181 | `BYT` | byte, boundary/yield/trace |
| 0182 | `CHR` | character, charisma, chain route |
| 0183 | `LIM` | limit, limb, local input mode |
| 0184 | `CAP` | capability, cap/limit, capture |
| 0185 | `MAX` | maximum, model action x |
| 0186 | `MIN` | minimum, mind/input/name |
| 0187 | `MID` | middle, model/input/data |
| 0188 | `END` | end, endpoint, entity/name/data |
| 0189 | `BEG` | begin, behavior/entry/guard |
| 0190 | `TOP` | topic, top, target output prompt |
| 0191 | `LOW` | low, law/output/warning |
| 0192 | `HIH` | high? help/input/human |
| 0193 | `HGH` | high, hard guard/harm |
| 0194 | `LHS` | left-hand side, local human signal |
| 0195 | `RHS` | right-hand side, runtime human signal |
| 0196 | `EOF` | end of file, execution/output/failure |
| 0197 | `EOL` | end of line, entity/output/layer |
| 0198 | `BOL` | beginning of line, boundary/output/law |
| 0199 | `DEL` | delete, delta, delivery |
| 0200 | `ADD` | add, additive, authority drift danger |
| 0201 | `NEW` | new, nearest executable/workable |
| 0202 | `OLD` | old, object layer data |
| 0203 | `RAW` | raw input, risk/action/warning |
| 0204 | `FIN` | final, finish, file/input/name |
| 0205 | `OUT` | output, outside, object/user/target |
| 0206 | `INP` | input, intent prompt, inner process |
| 0207 | `IOT` | input/output/tool, internet of things |
| 0208 | `IOU` | I owe you, input/output/user |
| 0209 | `ACL` | access control list, authority/control/law |
| 0210 | `ACC` | access, account, accuracy |
| 0211 | `PWD` | password, prompt/write/data |
| 0212 | `PIN` | PIN code, prompt/input/name |
| 0213 | `UID` | user ID, unique ID |
| 0214 | `PID` | process ID, prompt ID |
| 0215 | `SID` | session ID, state ID |
| 0216 | `RID` | request ID, route ID |
| 0217 | `CID` | context ID, case ID |
| 0218 | `DID` | decentralized ID, did/act |
| 0219 | `NID` | node ID, name ID |
| 0220 | `OID` | object ID, output ID |
| 0221 | `VID` | video ID, validation ID |
| 0222 | `TID` | thread ID, task ID |
| 0223 | `EID` | entity ID, event ID |
| 0224 | `FID` | file ID, function ID |
| 0225 | `BAD` | bad, behavior action drift |
| 0226 | `MAD` | mad, moral/affect drift |
| 0227 | `SAD` | sad, safety/affect drift |
| 0228 | `ANG` | anger, angle, agent/name/guard |
| 0229 | `FUN` | function, fun, filter/user/name |
| 0230 | `SEX` | sex, sexual content, system execute x |
| 0231 | `NSF` | not safe for, no-source/file |
| 0232 | `NSW` | not safe/warning, New South Wales |
| 0233 | `SFW` | safe for work, safety filter/warning |
| 0234 | `HIT` | hit, harm/intent/target |
| 0235 | `KIL` | kill, kindness/input/law |
| 0236 | `DIE` | die, data/instruction/error |
| 0237 | `GUN` | gun, guard/user/name |
| 0238 | `WPN` | weapon, warning prompt/name |
| 0239 | `THR` | threat, throat, threshold |
| 0240 | `DNG` | danger, domain/name/guard |
| 0241 | `RIP` | rest in peace, route/input/prompt |
| 0242 | `SOS` | help signal, safety/output/state |
| 0243 | `MED` | medical, medium, model/evidence/data |
| 0244 | `DXN` | diagnosis, data x name |
| 0245 | `DXG` | diagnosing, data x guard |
| 0246 | `PSY` | psychology, psychosis, prompt state y |
| 0247 | `CLN` | clinical, clean, class/name |
| 0248 | `DIA` | diagnosis, diagram, data/input/action |
| 0249 | `DGN` | diagnosis, design, domain guard/name |
| 0250 | `MNT` | monitor, mount, minute |
| 0251 | `EAT` | eat, consume, entity/action/target |
| 0252 | `LOC` | location, local, locus |
| 0253 | `WHO` | who, human/who question |
| 0254 | `WHY` | why, reason query |
| 0255 | `HOW` | how, method query |
| 0256 | `WHT` | what, white, warning/human/target |
| 0257 | `NAM` | name, named actor/module |
| 0258 | `ACT` | action, active, act |
| 0259 | `AGN` | agent, again, agency/name |
| 0260 | `AGY` | agency, agent yield |
| 0261 | `INT` | intent, integer, internal |
| 0262 | `ENT` | entity, enter, entropy |
| 0263 | `FOE` | foe, force/opponent/entity |
| 0264 | `PST` | post, pest, past, prompt state |
| 0265 | `BST` | beast, best, boost, bot state |
| 0266 | `BEA` | beast, behavior/entity/action |
| 0267 | `PEA` | pest? prompt/entity/action |
| 0268 | `ROA` | roar? route/object/action |
| 0269 | `ROR` | roar, rule/output/route |
| 0270 | `WAL` | wall, warning/action/law |
| 0271 | `WLL` | will, wall, warning/law/layer |
| 0272 | `RND` | random, round, route/name/data |
| 0273 | `VAR` | variable, variance, value/action/route |
| 0274 | `UNI` | union, universal, unique |
| 0275 | `LIT` | literal, lit, language/input/trace |
| 0276 | `ABS` | abstract, absolute, absence |
| 0277 | `DES` | describe, design, destination |
| 0278 | `EGO` | ego, entity/goal/output |
| 0279 | `IDK` | I don't know, identity key |
| 0280 | `TBD` | to be determined, task boundary/data |
| 0281 | `TBA` | to be announced, target boundary/action |
| 0282 | `TBC` | to be continued, task boundary/context |
| 0283 | `WIP` | work in progress, warning/input/prompt |
| 0284 | `POC` | proof of concept, point of contact |
| 0285 | `MVP` | minimum viable product, model/value/prompt |
| 0286 | `OKR` | objectives/key/results, okay route |
| 0287 | `KPI` | key performance indicator, kindness/pass/input |
| 0288 | `ROI` | return on investment, route/object/input |
| 0289 | `SLA` | service level agreement, safety/law/action |
| 0290 | `RCA` | root cause analysis, runtime control action |
| 0291 | `UXR` | user experience research, user x route |
| 0292 | `HCI` | human computer interaction, human/context/input |
| 0293 | `NDA` | non-disclosure agreement, no data action |
| 0294 | `PII` | personal info, prompt/input identity |
| 0295 | `TOS` | terms of service, tone/output/state |
| 0296 | `SDK` | software kit, system data key |
| 0297 | `IDE` | integrated development environment, identity/data/error |
| 0298 | `DBA` | database admin, data boundary action |
| 0299 | `SQL` | database query language, source/query/layer |
| 0300 | `URL` | web address, user route link |
| 0301 | `URI` | identifier, user route/input |
| 0302 | `DNS` | domain name system, diagnosis/noise/signal |
| 0303 | `SSL` | security layer, source/safety/law |
| 0304 | `TLS` | transport layer security, token limit state |
| 0305 | `TCP` | network protocol, task class prompt |
| 0306 | `UDP` | network protocol, user data prompt |
| 0307 | `SSH` | secure shell, system/safety/human |
| 0308 | `FTP` | file transfer, final target prompt |
| 0309 | `TRT` | TR=truth + target flag, TR=trace + truth marker, target + RT=runtime, truth + RT=real-time, target-role-target chain, truth / rule / truth shorthand |
| 0310 | `RTR` | RT=runtime + role flag, RT=real-time + rule marker, role + TR=truth, rule + TR=trace, role-target-role chain, rule / truth / rule shorthand |
| 0311 | `CTR` | CT=context + role flag, CT=control + rule marker, context + TR=truth, control + TR=trace, context-target-role chain, control / truth / rule shorthand |
| 0312 | `RST` | RS=response + target flag, RS=risk state + truth marker, role + ST=state, rule + ST=status, role-state-target chain, rule / safety / truth shorthand |
| 0313 | `PRT` | PR=prompt + target flag, PR=process + truth marker, prompt + RT=runtime, process + RT=real-time, prompt-role-target chain, process / rule / truth shorthand |
| 0314 | `DRS` | DR=drift + state flag, DR=doctor + safety marker, data + RS=response, decision + RS=risk state, data-role-state chain, decision / rule / safety shorthand |
| 0315 | `TRS` | TR=truth + state flag, TR=trace + safety marker, target + RS=response, truth + RS=risk state, target-role-state chain, truth / rule / safety shorthand |
| 0316 | `DRD` | DR=drift + data flag, DR=doctor + decision marker, data + RD=read depth, decision + RD=runtime depth, data-role-data chain, decision / rule / decision shorthand |
| 0317 | `TRD` | TR=truth + data flag, TR=trace + decision marker, target + RD=read depth, truth + RD=runtime depth, target-role-data chain, truth / rule / decision shorthand |
| 0318 | `RDR` | RD=read depth + role flag, RD=runtime depth + rule marker, role + DR=drift, rule + DR=doctor, role-data-role chain, rule / decision / rule shorthand |
| 0319 | `RCT` | RC=recall + target flag, RC=record + truth marker, role + CT=context, rule + CT=control, role-context-target chain, rule / control / truth shorthand |
| 0320 | `MOB` | English word 'mob', MO=mode + bot flag, MO=moral + boundary marker, module + OB=object, mode + OB=observation, module-output-bot chain |
| 0321 | `MDR` | MD=markdown + role flag, MD=medical + rule marker, module + DR=drift, mode + DR=doctor, module-data-role chain, mode / decision / rule shorthand |
| 0322 | `MST` | MS=model state + target flag, MS=memory store + truth marker, module + ST=state, mode + ST=status, module-state-target chain, mode / safety / truth shorthand |
| 0323 | `PRD` | PR=prompt + data flag, PR=process + decision marker, prompt + RD=read depth, process + RD=runtime depth, prompt-role-data chain, process / rule / decision shorthand |
| 0324 | `BDR` | BD=boundary + role flag, BD=body + rule marker, bot + DR=drift, boundary + DR=doctor, bot-data-role chain, boundary / decision / rule shorthand |
| 0325 | `DRC` | DR=drift + context flag, DR=doctor + control marker, data + RC=recall, decision + RC=record, data-role-context chain, decision / rule / control shorthand |
| 0326 | `HST` | HS=human signal + target flag, HS=harm signal + truth marker, human + ST=state, heart + ST=status, human-state-target chain, heart / safety / truth shorthand |
| 0327 | `BRT` | BR=boundary route + target flag, BR=break + truth marker, bot + RT=runtime, boundary + RT=real-time, bot-role-target chain, boundary / rule / truth shorthand |
| 0328 | `HTR` | HT=human target + role flag, HT=heart + rule marker, human + TR=truth, heart + TR=trace, human-target-role chain, heart / truth / rule shorthand |
| 0329 | `PRC` | PR=prompt + context flag, PR=process + control marker, prompt + RC=recall, process + RC=record, prompt-role-context chain, process / rule / control shorthand |
| 0330 | `DRE` | DR=drift + entity flag, DR=doctor + emotion marker, data + RE=repair, decision + RE=response, data-role-entity chain, decision / rule / emotion shorthand |
| 0331 | `TRE` | TR=truth + entity flag, TR=trace + emotion marker, target + RE=repair, truth + RE=response, target-role-entity chain, truth / rule / emotion shorthand |
| 0332 | `BRS` | BR=boundary route + state flag, BR=break + safety marker, bot + RS=response, boundary + RS=risk state, bot-role-state chain, boundary / rule / safety shorthand |
| 0333 | `BRD` | BR=boundary route + data flag, BR=break + decision marker, bot + RD=read depth, boundary + RD=runtime depth, bot-role-data chain, boundary / rule / decision shorthand |
| 0334 | `PRE` | PR=prompt + entity flag, PR=process + emotion marker, prompt + RE=repair, process + RE=response, prompt-role-entity chain, process / rule / emotion shorthand |
| 0335 | `HPR` | HP=help + role flag, HP=harm prevention + rule marker, human + PR=prompt, heart + PR=process, human-prompt-role chain, heart / process / rule shorthand |
| 0336 | `ADR` | AD=advice + role flag, AD=ad + rule marker, action + DR=drift, agent + DR=doctor, action-data-role chain, agent / decision / rule shorthand |
| 0337 | `HRD` | HR=human response + data flag, HR=heart rate + decision marker, human + RD=read depth, heart + RD=runtime depth, human-role-data chain, heart / rule / decision shorthand |
| 0338 | `HMD` | HM=human + data flag, HM=humor + decision marker, human + MD=markdown, heart + MD=medical, human-module-data chain, heart / mode / decision shorthand |
| 0339 | `HMT` | HM=human + target flag, HM=humor + truth marker, human + MT=metric, heart + MT=meta, human-module-target chain, heart / mode / truth shorthand |
| 0340 | `HMS` | HM=human + state flag, HM=humor + safety marker, human + MS=model state, heart + MS=memory store, human-module-state chain, heart / mode / safety shorthand |
| 0341 | `IDR` | ID=identity + role flag, ID=identifier + rule marker, intent + DR=drift, input + DR=doctor, intent-data-role chain, input / decision / rule shorthand |
| 0342 | `BRC` | BR=boundary route + context flag, BR=break + control marker, bot + RC=recall, boundary + RC=record, bot-role-context chain, boundary / rule / control shorthand |
| 0343 | `AMD` | AM=AMIMI + data flag, AM=anti-media + decision marker, action + MD=markdown, agent + MD=medical, action-module-data chain, agent / mode / decision shorthand |
| 0344 | `AMT` | AM=AMIMI + target flag, AM=anti-media + truth marker, action + MT=metric, agent + MT=meta, action-module-target chain, agent / mode / truth shorthand |
| 0345 | `HRC` | HR=human response + context flag, HR=heart rate + control marker, human + RC=recall, heart + RC=record, human-role-context chain, heart / rule / control shorthand |
| 0346 | `IPR` | IP=internet protocol + role flag, IP=intellectual property + rule marker, intent + PR=prompt, input + PR=process, intent-prompt-role chain, input / process / rule shorthand |
| 0347 | `NOR` | English word 'nor', NO=negation + role flag, NO=no + rule marker, name + OR=origin, no + OR=object relation, name-output-role chain |
| 0348 | `AMS` | AM=AMIMI + state flag, AM=anti-media + safety marker, action + MS=model state, agent + MS=memory store, action-module-state chain, agent / mode / safety shorthand |
| 0349 | `BRE` | BR=boundary route + entity flag, BR=break + emotion marker, bot + RE=repair, boundary + RE=response, bot-role-entity chain, boundary / rule / emotion shorthand |
| 0350 | `IMD` | IM=image + data flag, IM=immediate + decision marker, intent + MD=markdown, input + MD=medical, intent-module-data chain, input / mode / decision shorthand |
| 0351 | `IMT` | IM=image + target flag, IM=immediate + truth marker, intent + MT=metric, input + MT=meta, intent-module-target chain, input / mode / truth shorthand |
| 0352 | `IMS` | IM=image + state flag, IM=immediate + safety marker, intent + MS=model state, input + MS=memory store, intent-module-state chain, input / mode / safety shorthand |
| 0353 | `FOR` | English word 'for', FO=foe + role flag, FO=form + rule marker, function + OR=origin, filter + OR=object relation, function-output-role chain |
| 0354 | `HMO` | HM=human + output flag, HM=humor + object marker, human + MO=mode, heart + MO=moral, human-module-output chain, heart / mode / object shorthand |
| 0355 | `HRE` | HR=human response + entity flag, HR=heart rate + emotion marker, human + RE=repair, heart + RE=response, human-role-entity chain, heart / rule / emotion shorthand |
| 0356 | `UST` | US=user + target flag, US=United States + truth marker, user + ST=state, unknown + ST=status, user-state-target chain, unknown / safety / truth shorthand |
| 0357 | `ORT` | OR=origin + target flag, OR=object relation + truth marker, output + RT=runtime, object + RT=real-time, output-role-target chain, object / rule / truth shorthand |
| 0358 | `HML` | HM=human + law flag, HM=humor + logic marker, human + ML=model, heart + ML=machine learning, human-module-law chain, heart / mode / logic shorthand |
| 0359 | `OPR` | OP=output + role flag, OP=operation + rule marker, output + PR=prompt, object + PR=process, output-prompt-role chain, object / process / rule shorthand |
| 0360 | `URT` | UR=user route + target flag, UR=urgent + truth marker, user + RT=runtime, unknown + RT=real-time, user-role-target chain, unknown / rule / truth shorthand |
| 0361 | `ORS` | OR=origin + state flag, OR=object relation + safety marker, output + RS=response, object + RS=risk state, output-role-state chain, object / rule / safety shorthand |
| 0362 | `MAS` | MA=AMAMI + state flag, MA=moral authority + safety marker, module + AS=autism spectrum, mode + AS=active state, module-action-state chain, mode / agent / safety shorthand |
| 0363 | `ORD` | OR=origin + data flag, OR=object relation + decision marker, output + RD=read depth, object + RD=runtime depth, output-role-data chain, object / rule / decision shorthand |
| 0364 | `AMO` | AM=AMIMI + output flag, AM=anti-media + object marker, action + MO=mode, agent + MO=moral, action-module-output chain, agent / mode / object shorthand |
| 0365 | `UCT` | UC=user context + target flag, UC=use case + truth marker, user + CT=context, unknown + CT=control, user-context-target chain, unknown / control / truth shorthand |
| 0366 | `SDR` | SD=system drift + role flag, SD=stable diffusion + rule marker, state + DR=drift, safety + DR=doctor, state-data-role chain, safety / decision / rule shorthand |
| 0367 | `URS` | UR=user route + state flag, UR=urgent + safety marker, user + RS=response, unknown + RS=risk state, user-role-state chain, unknown / rule / safety shorthand |
| 0368 | `URD` | UR=user route + data flag, UR=urgent + decision marker, user + RD=read depth, unknown + RD=runtime depth, user-role-data chain, unknown / rule / decision shorthand |
| 0369 | `MOP` | MO=mode + prompt flag, MO=moral + process marker, module + OP=output, mode + OP=operation, module-output-prompt chain, mode / object / process shorthand |
| 0370 | `AML` | AM=AMIMI + law flag, AM=anti-media + logic marker, action + ML=model, agent + ML=machine learning, action-module-law chain, agent / mode / logic shorthand |
| 0371 | `AID` | AI=artificial intelligence + data flag, AI=assistant identity + decision marker, action + ID=identity, agent + ID=identifier, action-intent-data chain, agent / input / decision shorthand |
| 0372 | `RSD` | RS=response + data flag, RS=risk state + decision marker, role + SD=system drift, rule + SD=stable diffusion, role-state-data chain, rule / safety / decision shorthand |
| 0373 | `SRT` | SR=source + target flag, SR=safety route + truth marker, state + RT=runtime, safety + RT=real-time, state-role-target chain, safety / rule / truth shorthand |
| 0374 | `RSR` | RS=response + role flag, RS=risk state + rule marker, role + SR=source, rule + SR=safety route, role-state-role chain, rule / safety / rule shorthand |
| 0375 | `IML` | IM=image + law flag, IM=immediate + logic marker, intent + ML=model, input + ML=machine learning, intent-module-law chain, input / mode / logic shorthand |
| 0376 | `SCT` | SC=scope + target flag, SC=self-control + truth marker, state + CT=context, safety + CT=control, state-context-target chain, safety / control / truth shorthand |
| 0377 | `HMI` | HM=human + intent flag, HM=humor + input marker, human + MI=IMAMI, heart + MI=machine intelligence, human-module-intent chain, heart / mode / input shorthand |
| 0378 | `OBD` | OB=object + data flag, OB=observation + decision marker, output + BD=boundary, object + BD=body, output-bot-data chain, object / boundary / decision shorthand |
| 0379 | `SPR` | SP=system prompt + role flag, SP=special + rule marker, state + PR=prompt, safety + PR=process, state-prompt-role chain, safety / process / rule shorthand |
| 0380 | `HMA` | HM=human + action flag, HM=humor + agent marker, human + MA=AMAMI, heart + MA=moral authority, human-module-action chain, heart / mode / agent shorthand |
| 0381 | `MSD` | MS=model state + data flag, MS=memory store + decision marker, module + SD=system drift, mode + SD=stable diffusion, module-state-data chain, mode / safety / decision shorthand |
| 0382 | `SRS` | SR=source + state flag, SR=safety route + safety marker, state + RS=response, safety + RS=risk state, state-role-state chain, safety / rule / safety shorthand |
| 0383 | `SRD` | SR=source + data flag, SR=safety route + decision marker, state + RD=read depth, safety + RD=runtime depth, state-role-data chain, safety / rule / decision shorthand |
| 0384 | `ORC` | OR=origin + context flag, OR=object relation + control marker, output + RC=recall, object + RC=record, output-role-context chain, object / rule / control shorthand |
| 0385 | `OBR` | OB=object + role flag, OB=observation + rule marker, output + BR=boundary route, object + BR=break, output-bot-role chain, object / boundary / rule shorthand |
| 0386 | `MSR` | MS=model state + role flag, MS=memory store + rule marker, module + SR=source, mode + SR=safety route, module-state-role chain, mode / safety / rule shorthand |
| 0387 | `AUS` | AU=autism + state flag, AU=authority + safety marker, action + US=user, agent + US=United States, action-user-state chain, agent / unknown / safety shorthand |
| 0388 | `AUX` | AU=autism + unknown flag, AU=authority + external marker, action + UX=user experience, agent + UX=unknown x, action-user-unknown chain, agent / unknown / external shorthand |
| 0389 | `CTD` | CT=context + data flag, CT=control + decision marker, context + TD=task drift, control + TD=temporal difference, context-target-data chain, control / truth / decision shorthand |
| 0390 | `AUR` | AU=autism + role flag, AU=authority + rule marker, action + UR=user route, agent + UR=urgent, action-user-role chain, agent / unknown / rule shorthand |
| 0391 | `MAI` | MA=AMAMI + intent flag, MA=moral authority + input marker, module + AI=artificial intelligence, mode + AI=assistant identity, module-action-intent chain, mode / agent / input shorthand |
| 0392 | `OBK` | OB=object + kindness flag, OB=observation + key marker, output + BK=block, object + BK=book, output-bot-kindness chain, object / boundary / key shorthand |
| 0393 | `AIM` | AI=artificial intelligence + module flag, AI=assistant identity + mode marker, action + IM=image, agent + IM=immediate, action-intent-module chain, agent / input / mode shorthand |
| 0394 | `URC` | UR=user route + context flag, UR=urgent + control marker, user + RC=recall, unknown + RC=record, user-role-context chain, unknown / rule / control shorthand |
| 0395 | `TCT` | TC=task class + target flag, TC=truth constraint + truth marker, target + CT=context, truth + CT=control, target-context-target chain, truth / control / truth shorthand |
| 0396 | `TDR` | TD=task drift + role flag, TD=temporal difference + rule marker, target + DR=drift, truth + DR=doctor, target-data-role chain, truth / decision / rule shorthand |
| 0397 | `STC` | ST=state + context flag, ST=status + control marker, state + TC=task class, safety + TC=truth constraint, state-target-context chain, safety / truth / control shorthand |
| 0398 | `MAU` | MA=AMAMI + user flag, MA=moral authority + unknown marker, module + AU=autism, mode + AU=authority, module-action-user chain, mode / agent / unknown shorthand |
| 0399 | `QDR` | QD=query depth + role flag, QD=question directive + rule marker, question + DR=drift, query + DR=doctor, question-data-role chain, query / decision / rule shorthand |
| 0400 | `QRT` | QR=question route + target flag, QR=quick response + truth marker, question + RT=runtime, query + RT=real-time, question-role-target chain, query / rule / truth shorthand |
| 0401 | `ORE` | OR=origin + entity flag, OR=object relation + emotion marker, output + RE=repair, object + RE=response, output-role-entity chain, object / rule / emotion shorthand |
| 0402 | `STM` | ST=state + module flag, ST=status + mode marker, state + TM=trademark, safety + TM=tone mode, state-target-module chain, safety / truth / mode shorthand |
| 0403 | `HSD` | HS=human signal + data flag, HS=harm signal + decision marker, human + SD=system drift, heart + SD=stable diffusion, human-state-data chain, heart / safety / decision shorthand |
| 0404 | `IOR` | IO=input/output + role flag, IO=inside/outside + rule marker, intent + OR=origin, input + OR=object relation, intent-output-role chain, input / object / rule shorthand |
| 0405 | `QCT` | QC=quality control + target flag, QC=question context + truth marker, question + CT=context, query + CT=control, question-context-target chain, query / control / truth shorthand |
| 0406 | `AIP` | AI=artificial intelligence + prompt flag, AI=assistant identity + process marker, action + IP=internet protocol, agent + IP=intellectual property, action-intent-prompt chain, agent / input / process shorthand |
| 0407 | `RSC` | RS=response + context flag, RS=risk state + control marker, role + SC=scope, rule + SC=self-control, role-state-context chain, rule / safety / control shorthand |
| 0408 | `STP` | ST=state + prompt flag, ST=status + process marker, state + TP=target prompt, safety + TP=true positive, state-target-prompt chain, safety / truth / process shorthand |
| 0409 | `AIN` | AI=artificial intelligence + name flag, AI=assistant identity + no marker, action + IN=input, agent + IN=instruction, action-intent-name chain, agent / input / no shorthand |
| 0410 | `TPR` | TP=target prompt + role flag, TP=true positive + rule marker, target + PR=prompt, truth + PR=process, target-prompt-role chain, truth / process / rule shorthand |
| 0411 | `HSR` | HS=human signal + role flag, HS=harm signal + rule marker, human + SR=source, heart + SR=safety route, human-state-role chain, heart / safety / rule shorthand |
| 0412 | `IMI` | IM=image + intent flag, IM=immediate + input marker, intent + MI=IMAMI, input + MI=machine intelligence, intent-module-intent chain, input / mode / input shorthand |
| 0413 | `MLR` | ML=model + role flag, ML=machine learning + rule marker, module + LR=legal risk, mode + LR=learning rate, module-law-role chain, mode / logic / rule shorthand |
| 0414 | `RTC` | RT=runtime + context flag, RT=real-time + control marker, role + TC=task class, rule + TC=truth constraint, role-target-context chain, rule / truth / control shorthand |
| 0415 | `AIO` | AI=artificial intelligence + output flag, AI=assistant identity + object marker, action + IO=input/output, agent + IO=inside/outside, action-intent-output chain, agent / input / object shorthand |
| 0416 | `MLT` | ML=model + target flag, ML=machine learning + truth marker, module + LT=limit, mode + LT=literal, module-law-target chain, mode / logic / truth shorthand |
| 0417 | `MTD` | MT=metric + data flag, MT=meta + decision marker, module + TD=task drift, mode + TD=temporal difference, module-target-data chain, mode / truth / decision shorthand |
| 0418 | `STL` | ST=state + law flag, ST=status + logic marker, state + TL=token limit, safety + TL=timeline, state-target-law chain, safety / truth / logic shorthand |
| 0419 | `URE` | UR=user route + entity flag, UR=urgent + emotion marker, user + RE=repair, unknown + RE=response, user-role-entity chain, unknown / rule / emotion shorthand |
| 0420 | `MIP` | MI=IMAMI + prompt flag, MI=machine intelligence + process marker, module + IP=internet protocol, mode + IP=intellectual property, module-intent-prompt chain, mode / input / process shorthand |
| 0421 | `RTM` | RT=runtime + module flag, RT=real-time + mode marker, role + TM=trademark, rule + TM=tone mode, role-target-module chain, rule / truth / mode shorthand |
| 0422 | `QRS` | QR=question route + state flag, QR=quick response + safety marker, question + RS=response, query + RS=risk state, question-role-state chain, query / rule / safety shorthand |
| 0423 | `QRD` | QR=question route + data flag, QR=quick response + decision marker, question + RD=read depth, query + RD=runtime depth, question-role-data chain, query / rule / decision shorthand |
| 0424 | `UAS` | UA=user agency + state flag, UA=Ukraine + safety marker, user + AS=autism spectrum, unknown + AS=active state, user-action-state chain, unknown / agent / safety shorthand |
| 0425 | `RSW` | RS=response + world flag, RS=risk state + weight marker, role + SW=software, rule + SW=switch, role-state-world chain, rule / safety / weight shorthand |
| 0426 | `RTP` | RT=runtime + prompt flag, RT=real-time + process marker, role + TP=target prompt, rule + TP=true positive, role-target-prompt chain, rule / truth / process shorthand |
| 0427 | `CTC` | CT=context + context flag, CT=control + control marker, context + TC=task class, control + TC=truth constraint, context-target-context chain, control / truth / control shorthand |
| 0428 | `LRT` | LR=legal risk + target flag, LR=learning rate + truth marker, law + RT=runtime, logic + RT=real-time, law-role-target chain, logic / rule / truth shorthand |
| 0429 | `MIO` | MI=IMAMI + output flag, MI=machine intelligence + object marker, module + IO=input/output, mode + IO=inside/outside, module-intent-output chain, mode / input / object shorthand |
| 0430 | `LTR` | LT=limit + role flag, LT=literal + rule marker, law + TR=truth, logic + TR=trace, law-target-role chain, logic / truth / rule shorthand |
| 0431 | `LCT` | LC=law/code + target flag, LC=local context + truth marker, law + CT=context, logic + CT=control, law-context-target chain, logic / control / truth shorthand |
| 0432 | `TMD` | TM=trademark + data flag, TM=tone mode + decision marker, target + MD=markdown, truth + MD=medical, target-module-data chain, truth / mode / decision shorthand |
| 0433 | `TMT` | TM=trademark + target flag, TM=tone mode + truth marker, target + MT=metric, truth + MT=meta, target-module-target chain, truth / mode / truth shorthand |
| 0434 | `CTM` | CT=context + module flag, CT=control + mode marker, context + TM=trademark, control + TM=tone mode, context-target-module chain, control / truth / mode shorthand |
| 0435 | `MSC` | MS=model state + context flag, MS=memory store + control marker, module + SC=scope, mode + SC=self-control, module-state-context chain, mode / safety / control shorthand |
| 0436 | `CTP` | CT=context + prompt flag, CT=control + process marker, context + TP=target prompt, control + TP=true positive, context-target-prompt chain, control / truth / process shorthand |
| 0437 | `TMS` | TM=trademark + state flag, TM=tone mode + safety marker, target + MS=model state, truth + MS=memory store, target-module-state chain, truth / mode / safety shorthand |
| 0438 | `UAD` | UA=user agency + data flag, UA=Ukraine + decision marker, user + AD=advice, unknown + AD=ad, user-action-data chain, unknown / agent / decision shorthand |
| 0439 | `MSP` | MS=model state + prompt flag, MS=memory store + process marker, module + SP=system prompt, mode + SP=special, module-state-prompt chain, mode / safety / process shorthand |
| 0440 | `ASR` | AS=autism spectrum + role flag, AS=active state + rule marker, action + SR=source, agent + SR=safety route, action-state-role chain, agent / safety / rule shorthand |
| 0441 | `BLR` | BL=block + role flag, BL=baseline + rule marker, bot + LR=legal risk, boundary + LR=learning rate, bot-law-role chain, boundary / logic / rule shorthand |
| 0442 | `BLT` | BL=block + target flag, BL=baseline + truth marker, bot + LT=limit, boundary + LT=literal, bot-law-target chain, boundary / logic / truth shorthand |
| 0443 | `OBG` | OB=object + goal flag, OB=observation + guard marker, output + BG=background, object + BG=behavior guard, output-bot-goal chain, object / boundary / guard shorthand |
| 0444 | `LRS` | LR=legal risk + state flag, LR=learning rate + safety marker, law + RS=response, logic + RS=risk state, law-role-state chain, logic / rule / safety shorthand |
| 0445 | `NAS` | NA=not applicable + state flag, NA=name + safety marker, name + AS=autism spectrum, no + AS=active state, name-action-state chain, no / agent / safety shorthand |
| 0446 | `MSW` | MS=model state + world flag, MS=memory store + weight marker, module + SW=software, mode + SW=switch, module-state-world chain, mode / safety / weight shorthand |
| 0447 | `SRE` | SR=source + entity flag, SR=safety route + emotion marker, state + RE=repair, safety + RE=response, state-role-entity chain, safety / rule / emotion shorthand |
| 0448 | `LRD` | LR=legal risk + data flag, LR=learning rate + decision marker, law + RD=read depth, logic + RD=runtime depth, law-role-data chain, logic / rule / decision shorthand |
| 0449 | `OBL` | OB=object + law flag, OB=observation + logic marker, output + BL=block, object + BL=baseline, output-bot-law chain, object / boundary / logic shorthand |
| 0450 | `AUC` | AU=autism + context flag, AU=authority + control marker, action + UC=user context, agent + UC=use case, action-user-context chain, agent / unknown / control shorthand |
| 0451 | `AUA` | AU=autism + action flag, AU=authority + agent marker, action + UA=user agency, agent + UA=Ukraine, action-user-action chain, agent / unknown / agent shorthand |
| 0452 | `MTC` | MT=metric + context flag, MT=meta + control marker, module + TC=task class, mode + TC=truth constraint, module-target-context chain, mode / truth / control shorthand |
| 0453 | `IOP` | IO=input/output + prompt flag, IO=inside/outside + process marker, intent + OP=output, input + OP=operation, intent-output-prompt chain, input / object / process shorthand |
| 0454 | `FAS` | FA=false + state flag, FA=fallback + safety marker, function + AS=autism spectrum, filter + AS=active state, function-action-state chain, filter / agent / safety shorthand |
| 0455 | `GTR` | GT=goal target + role flag, GT=greater than + rule marker, goal + TR=truth, guard + TR=trace, goal-target-role chain, guard / truth / rule shorthand |
| 0456 | `HTD` | HT=human target + data flag, HT=heart + decision marker, human + TD=task drift, heart + TD=temporal difference, human-target-data chain, heart / truth / decision shorthand |
| 0457 | `MTM` | MT=metric + module flag, MT=meta + mode marker, module + TM=trademark, mode + TM=tone mode, module-target-module chain, mode / truth / mode shorthand |
| 0458 | `NAD` | NA=not applicable + data flag, NA=name + decision marker, name + AD=advice, no + AD=ad, name-action-data chain, no / agent / decision shorthand |
| 0459 | `MLC` | ML=model + context flag, ML=machine learning + control marker, module + LC=law/code, mode + LC=local context, module-law-context chain, mode / logic / control shorthand |
| 0460 | `HSC` | HS=human signal + context flag, HS=harm signal + control marker, human + SC=scope, heart + SC=self-control, human-state-context chain, heart / safety / control shorthand |
| 0461 | `MTP` | MT=metric + prompt flag, MT=meta + process marker, module + TP=target prompt, mode + TP=true positive, module-target-prompt chain, mode / truth / process shorthand |
| 0462 | `BGT` | BG=background + target flag, BG=behavior guard + truth marker, bot + GT=goal target, boundary + GT=greater than, bot-goal-target chain, boundary / guard / truth shorthand |
| 0463 | `GDR` | GD=good + role flag, GD=guard + rule marker, goal + DR=drift, guard + DR=doctor, goal-data-role chain, guard / decision / rule shorthand |
| 0464 | `GRT` | GR=grader + target flag, GR=guard route + truth marker, goal + RT=runtime, guard + RT=real-time, goal-role-target chain, guard / rule / truth shorthand |
| 0465 | `IOB` | IO=input/output + bot flag, IO=inside/outside + boundary marker, intent + OB=object, input + OB=observation, intent-output-bot chain, input / object / boundary shorthand |
| 0466 | `HSP` | HS=human signal + prompt flag, HS=harm signal + process marker, human + SP=system prompt, heart + SP=special, human-state-prompt chain, heart / safety / process shorthand |
| 0467 | `QRC` | QR=question route + context flag, QR=quick response + control marker, question + RC=recall, query + RC=record, question-role-context chain, query / rule / control shorthand |
| 0468 | `FAD` | FA=false + data flag, FA=fallback + decision marker, function + AD=advice, filter + AD=ad, function-action-data chain, filter / agent / decision shorthand |
| 0469 | `BGR` | BG=background + role flag, BG=behavior guard + rule marker, bot + GR=grader, boundary + GR=guard route, bot-goal-role chain, boundary / guard / rule shorthand |
| 0470 | `MTL` | MT=metric + law flag, MT=meta + logic marker, module + TL=token limit, mode + TL=timeline, module-target-law chain, mode / truth / logic shorthand |
| 0471 | `BGD` | BG=background + data flag, BG=behavior guard + decision marker, bot + GD=good, boundary + GD=guard, bot-goal-data chain, boundary / guard / decision shorthand |
| 0472 | `HSW` | HS=human signal + world flag, HS=harm signal + weight marker, human + SW=software, heart + SW=switch, human-state-world chain, heart / safety / weight shorthand |
| 0473 | `MLG` | ML=model + goal flag, ML=machine learning + guard marker, module + LG=language, mode + LG=logic gate, module-law-goal chain, mode / logic / guard shorthand |
| 0474 | `UAI` | UA=user agency + intent flag, UA=Ukraine + input marker, user + AI=artificial intelligence, unknown + AI=assistant identity, user-action-intent chain, unknown / agent / input shorthand |
| 0475 | `GCT` | GC=garbage collection + target flag, GC=guard core + truth marker, goal + CT=context, guard + CT=control, goal-context-target chain, guard / control / truth shorthand |
| 0476 | `GRS` | GR=grader + state flag, GR=guard route + safety marker, goal + RS=response, guard + RS=risk state, goal-role-state chain, guard / rule / safety shorthand |
| 0477 | `QAS` | QA=question/answer + state flag, QA=quality assurance + safety marker, question + AS=autism spectrum, query + AS=active state, question-action-state chain, query / agent / safety shorthand |
| 0478 | `TMO` | TM=trademark + output flag, TM=tone mode + object marker, target + MO=mode, truth + MO=moral, target-module-output chain, truth / mode / object shorthand |
| 0479 | `UAM` | UA=user agency + module flag, UA=Ukraine + mode marker, user + AM=AMIMI, unknown + AM=anti-media, user-action-module chain, unknown / agent / mode shorthand |
| 0480 | `ASC` | AS=autism spectrum + context flag, AS=active state + control marker, action + SC=scope, agent + SC=self-control, action-state-context chain, agent / safety / control shorthand |
| 0481 | `BLC` | BL=block + context flag, BL=baseline + control marker, bot + LC=law/code, boundary + LC=local context, bot-law-context chain, boundary / logic / control shorthand |
| 0482 | `JDR` | JD=judge + role flag, JD=judgment + rule marker, judge + DR=drift, job + DR=doctor, judge-data-role chain, job / decision / rule shorthand |
| 0483 | `INO` | IN=input + output flag, IN=instruction + object marker, intent + NO=negation, input + NO=no, intent-name-output chain, input / no / object shorthand |
| 0484 | `QRE` | QR=question route + entity flag, QR=quick response + emotion marker, question + RE=repair, query + RE=response, question-role-entity chain, query / rule / emotion shorthand |
| 0485 | `UAU` | UA=user agency + user flag, UA=Ukraine + unknown marker, user + AU=autism, unknown + AU=authority, user-action-user chain, unknown / agent / unknown shorthand |
| 0486 | `LRC` | LR=legal risk + context flag, LR=learning rate + control marker, law + RC=recall, logic + RC=record, law-role-context chain, logic / rule / control shorthand |
| 0487 | `ASP` | AS=autism spectrum + prompt flag, AS=active state + process marker, action + SP=system prompt, agent + SP=special, action-state-prompt chain, agent / safety / process shorthand |
| 0488 | `INA` | IN=input + action flag, IN=instruction + agent marker, intent + NA=not applicable, input + NA=name, intent-name-action chain, input / no / agent shorthand |
| 0489 | `HTC` | HT=human target + context flag, HT=heart + control marker, human + TC=task class, heart + TC=truth constraint, human-target-context chain, heart / truth / control shorthand |
| 0490 | `MLW` | ML=model + world flag, ML=machine learning + weight marker, module + LW=law, mode + LW=low weight, module-law-world chain, mode / logic / weight shorthand |
| 0491 | `INV` | IN=input + value flag, IN=instruction + veto marker, intent + NV=nearest valid, input + NV=nonviolent, intent-name-value chain, input / no / veto shorthand |
| 0492 | `JRT` | JR=judge route + target flag, JR=junior + truth marker, judge + RT=runtime, job + RT=real-time, judge-role-target chain, job / rule / truth shorthand |
| 0493 | `QAD` | QA=question/answer + data flag, QA=quality assurance + decision marker, question + AD=advice, query + AD=ad, question-action-data chain, query / agent / decision shorthand |
| 0494 | `HTM` | HT=human target + module flag, HT=heart + mode marker, human + TM=trademark, heart + TM=tone mode, human-target-module chain, heart / truth / mode shorthand |
| 0495 | `XDR` | XD=unknown data + role flag, XD=laugh emoticon + rule marker, unknown + DR=drift, external + DR=doctor, unknown-data-role chain, external / decision / rule shorthand |
| 0496 | `TML` | TM=trademark + law flag, TM=tone mode + logic marker, target + ML=model, truth + ML=machine learning, target-module-law chain, truth / mode / logic shorthand |
| 0497 | `XST` | XS=excess + target flag, XS=unknown state + truth marker, unknown + ST=state, external + ST=status, unknown-state-target chain, external / safety / truth shorthand |
| 0498 | `ASW` | AS=autism spectrum + world flag, AS=active state + weight marker, action + SW=software, agent + SW=switch, action-state-world chain, agent / safety / weight shorthand |
| 0499 | `BKT` | BK=block + target flag, BK=book + truth marker, bot + KT=key token, boundary + KT=knowledge transfer, bot-kindness-target chain, boundary / key / truth shorthand |
| 0500 | `NAI` | NA=not applicable + intent flag, NA=name + input marker, name + AI=artificial intelligence, no + AI=assistant identity, name-action-intent chain, no / agent / input shorthand |
| 0501 | `HTP` | HT=human target + prompt flag, HT=heart + process marker, human + TP=target prompt, heart + TP=true positive, human-target-prompt chain, heart / truth / process shorthand |
| 0502 | `INE` | IN=input + entity flag, IN=instruction + emotion marker, intent + NE=nearest, input + NE=negative, intent-name-entity chain, input / no / emotion shorthand |
| 0503 | `XRT` | XR=extended reality + target flag, XR=unknown route + truth marker, unknown + RT=runtime, external + RT=real-time, unknown-role-target chain, external / rule / truth shorthand |
| 0504 | `XTR` | XT=external target + role flag, XT=unknown truth + rule marker, unknown + TR=truth, external + TR=trace, unknown-target-role chain, external / truth / rule shorthand |
| 0505 | `BLG` | BL=block + goal flag, BL=baseline + guard marker, bot + LG=language, boundary + LG=logic gate, bot-law-goal chain, boundary / logic / guard shorthand |
| 0506 | `BKR` | BK=block + role flag, BK=book + rule marker, bot + KR=key route, boundary + KR=kindness route, bot-kindness-role chain, boundary / key / rule shorthand |
| 0507 | `KTR` | KT=key token + role flag, KT=knowledge transfer + rule marker, kindness + TR=truth, key + TR=trace, kindness-target-role chain, key / truth / rule shorthand |
| 0508 | `HTL` | HT=human target + law flag, HT=heart + logic marker, human + TL=token limit, heart + TL=timeline, human-target-law chain, heart / truth / logic shorthand |
| 0509 | `NAU` | NA=not applicable + user flag, NA=name + unknown marker, name + AU=autism, no + AU=authority, name-action-user chain, no / agent / unknown shorthand |
| 0510 | `FAI` | FA=false + intent flag, FA=fallback + input marker, function + AI=artificial intelligence, filter + AI=assistant identity, function-action-intent chain, filter / agent / input shorthand |
| 0511 | `KPR` | KP=key prompt + role flag, KP=keep + rule marker, kindness + PR=prompt, key + PR=process, kindness-prompt-role chain, key / process / rule shorthand |
| 0512 | `LRE` | LR=legal risk + entity flag, LR=learning rate + emotion marker, law + RE=repair, logic + RE=response, law-role-entity chain, logic / rule / emotion shorthand |
| 0513 | `JRS` | JR=judge route + state flag, JR=junior + safety marker, judge + RS=response, job + RS=risk state, judge-role-state chain, job / rule / safety shorthand |
| 0514 | `KRT` | KR=key route + target flag, KR=kindness route + truth marker, kindness + RT=runtime, key + RT=real-time, kindness-role-target chain, key / rule / truth shorthand |
| 0515 | `JRD` | JR=judge route + data flag, JR=junior + decision marker, judge + RD=read depth, job + RD=runtime depth, judge-role-data chain, job / rule / decision shorthand |
| 0516 | `FAM` | FA=false + module flag, FA=fallback + mode marker, function + AM=AMIMI, filter + AM=anti-media, function-action-module chain, filter / agent / mode shorthand |
| 0517 | `OPT` | English word 'opt', OP=output + target flag, OP=operation + truth marker, output + PT=prompt token, object + PT=passage/truth, output-prompt-target chain |
| 0518 | `BLW` | BL=block + world flag, BL=baseline + weight marker, bot + LW=law, boundary + LW=low weight, bot-law-world chain, boundary / logic / weight shorthand |
| 0519 | `USD` | US=user + data flag, US=United States + decision marker, user + SD=system drift, unknown + SD=stable diffusion, user-state-data chain, unknown / safety / decision shorthand |
| 0520 | `FAU` | FA=false + user flag, FA=fallback + unknown marker, function + AU=autism, filter + AU=authority, function-action-user chain, filter / agent / unknown shorthand |
| 0521 | `XRS` | XR=extended reality + state flag, XR=unknown route + safety marker, unknown + RS=response, external + RS=risk state, unknown-role-state chain, external / rule / safety shorthand |
| 0522 | `XRD` | XR=extended reality + data flag, XR=unknown route + decision marker, unknown + RD=read depth, external + RD=runtime depth, unknown-role-data chain, external / rule / decision shorthand |
| 0523 | `BGC` | BG=background + context flag, BG=behavior guard + control marker, bot + GC=garbage collection, boundary + GC=guard core, bot-goal-context chain, boundary / guard / control shorthand |
| 0524 | `GRC` | GR=grader + context flag, GR=guard route + control marker, goal + RC=recall, guard + RC=record, goal-role-context chain, guard / rule / control shorthand |
| 0525 | `NOP` | NO=negation + prompt flag, NO=no + process marker, name + OP=output, no + OP=operation, name-output-prompt chain, no / object / process shorthand |
| 0526 | `KRS` | KR=key route + state flag, KR=kindness route + safety marker, kindness + RS=response, key + RS=risk state, kindness-role-state chain, key / rule / safety shorthand |
| 0527 | `FIM` | FI=file + module flag, FI=filter + mode marker, function + IM=image, filter + IM=immediate, function-intent-module chain, filter / input / mode shorthand |
| 0528 | `KRD` | KR=key route + data flag, KR=kindness route + decision marker, kindness + RD=read depth, key + RD=runtime depth, kindness-role-data chain, key / rule / decision shorthand |
| 0529 | `QAI` | QA=question/answer + intent flag, QA=quality assurance + input marker, question + AI=artificial intelligence, query + AI=assistant identity, question-action-intent chain, query / agent / input shorthand |
| 0530 | `NOB` | NO=negation + bot flag, NO=no + boundary marker, name + OB=object, no + OB=observation, name-output-bot chain, no / object / boundary shorthand |
| 0531 | `BGL` | BG=background + law flag, BG=behavior guard + logic marker, bot + GL=gloss, boundary + GL=global, bot-goal-law chain, boundary / guard / logic shorthand |
| 0532 | `BKP` | BK=block + prompt flag, BK=book + process marker, bot + KP=key prompt, boundary + KP=keep, bot-kindness-prompt chain, boundary / key / process shorthand |
| 0533 | `FOP` | FO=foe + prompt flag, FO=form + process marker, function + OP=output, filter + OP=operation, function-output-prompt chain, filter / object / process shorthand |
| 0534 | `QAM` | QA=question/answer + module flag, QA=quality assurance + mode marker, question + AM=AMIMI, query + AM=anti-media, question-action-module chain, query / agent / mode shorthand |
| 0535 | `TMI` | TM=trademark + intent flag, TM=tone mode + input marker, target + MI=IMAMI, truth + MI=machine intelligence, target-module-intent chain, truth / mode / input shorthand |
| 0536 | `FIP` | FI=file + prompt flag, FI=filter + process marker, function + IP=internet protocol, filter + IP=intellectual property, function-intent-prompt chain, filter / input / process shorthand |
| 0537 | `GRE` | GR=grader + entity flag, GR=guard route + emotion marker, goal + RE=repair, guard + RE=response, goal-role-entity chain, guard / rule / emotion shorthand |
| 0538 | `QAU` | QA=question/answer + user flag, QA=quality assurance + unknown marker, question + AU=autism, query + AU=authority, question-action-user chain, query / agent / unknown shorthand |
| 0539 | `TMA` | TM=trademark + action flag, TM=tone mode + agent marker, target + MA=AMAMI, truth + MA=moral authority, target-module-action chain, truth / mode / agent shorthand |
| 0540 | `RCS` | RC=recall + state flag, RC=record + safety marker, role + CS=case, rule + CS=context state, role-context-state chain, rule / control / safety shorthand |
| 0541 | `YRT` | YR=year + target flag, YR=your + truth marker, yes + RT=runtime, why + RT=real-time, yes-role-target chain, why / rule / truth shorthand |
| 0542 | `YTR` | YT=YouTube + role flag, YT=why target + rule marker, yes + TR=truth, why + TR=trace, yes-target-role chain, why / truth / rule shorthand |
| 0543 | `FOB` | FO=foe + bot flag, FO=form + boundary marker, function + OB=object, filter + OB=observation, function-output-bot chain, filter / object / boundary shorthand |
| 0544 | `FIO` | FI=file + output flag, FI=filter + object marker, function + IO=input/output, filter + IO=inside/outside, function-intent-output chain, filter / input / object shorthand |
| 0545 | `RCR` | RC=recall + role flag, RC=record + rule marker, role + CR=constraint route, rule + CR=credit, role-context-role chain, rule / control / rule shorthand |
| 0546 | `RDS` | RD=read depth + state flag, RD=runtime depth + safety marker, role + DS=data source, rule + DS=decision state, role-data-state chain, rule / decision / safety shorthand |
| 0547 | `BKN` | BK=block + name flag, BK=book + no marker, bot + KN=known, boundary + KN=kindness/niceness, bot-kindness-name chain, boundary / key / no shorthand |
| 0548 | `JRC` | JR=judge route + context flag, JR=junior + control marker, judge + RC=recall, job + RC=record, judge-role-context chain, job / rule / control shorthand |
| 0549 | `RCD` | RC=recall + data flag, RC=record + decision marker, role + CD=code, rule + CD=clinical diagnosis, role-context-data chain, rule / control / decision shorthand |
| 0550 | `RDT` | RD=read depth + target flag, RD=runtime depth + truth marker, role + DT=data, rule + DT=decision tree, role-data-target chain, rule / decision / truth shorthand |
| 0551 | `ZTR` | ZT=zero target + role flag, ZT=final token + rule marker, zero + TR=truth, final state + TR=trace, zero-target-role chain, final state / truth / rule shorthand |
| 0552 | `BKL` | BK=block + law flag, BK=book + logic marker, bot + KL=kill, boundary + KL=key layer, bot-kindness-law chain, boundary / key / logic shorthand |
| 0553 | `XRC` | XR=extended reality + context flag, XR=unknown route + control marker, unknown + RC=recall, external + RC=record, unknown-role-context chain, external / rule / control shorthand |
| 0554 | `DST` | DS=data source + target flag, DS=decision state + truth marker, data + ST=state, decision + ST=status, data-state-target chain, decision / safety / truth shorthand |
| 0555 | `MDS` | MD=markdown + state flag, MD=medical + safety marker, module + DS=data source, mode + DS=decision state, module-data-state chain, mode / decision / safety shorthand |
| 0556 | `MDT` | MD=markdown + target flag, MD=medical + truth marker, module + DT=data, mode + DT=decision tree, module-data-target chain, mode / decision / truth shorthand |
| 0557 | `YRS` | YR=year + state flag, YR=your + safety marker, yes + RS=response, why + RS=risk state, yes-role-state chain, why / rule / safety shorthand |
| 0558 | `USC` | US=user + context flag, US=United States + control marker, user + SC=scope, unknown + SC=self-control, user-state-context chain, unknown / safety / control shorthand |
| 0559 | `CST` | CS=case + target flag, CS=context state + truth marker, context + ST=state, control + ST=status, context-state-target chain, control / safety / truth shorthand |
| 0560 | `YRD` | YR=year + data flag, YR=your + decision marker, yes + RD=read depth, why + RD=runtime depth, yes-role-data chain, why / rule / decision shorthand |
| 0561 | `KRC` | KR=key route + context flag, KR=kindness route + control marker, kindness + RC=recall, key + RC=record, kindness-role-context chain, key / rule / control shorthand |
| 0562 | `USP` | US=user + prompt flag, US=United States + process marker, user + SP=system prompt, unknown + SP=special, user-state-prompt chain, unknown / safety / process shorthand |
| 0563 | `DTR` | DT=data + role flag, DT=decision tree + rule marker, data + TR=truth, decision + TR=trace, data-target-role chain, decision / truth / rule shorthand |
| 0564 | `JRE` | JR=judge route + entity flag, JR=junior + emotion marker, judge + RE=repair, job + RE=response, judge-role-entity chain, job / rule / emotion shorthand |
| 0565 | `REX` | RE=repair + unknown flag, RE=response + external marker, role + EX=execute, rule + EX=example, role-entity-unknown chain, rule / emotion / external shorthand |
| 0566 | `PTR` | PT=prompt token + role flag, PT=passage/truth + rule marker, prompt + TR=truth, process + TR=trace, prompt-target-role chain, process / truth / rule shorthand |
| 0567 | `CDR` | CD=code + role flag, CD=clinical diagnosis + rule marker, context + DR=drift, control + DR=doctor, context-data-role chain, control / decision / rule shorthand |
| 0568 | `XAS` | XA=unknown action + state flag, XA=external agent + safety marker, unknown + AS=autism spectrum, external + AS=active state, unknown-action-state chain, external / agent / safety shorthand |
| 0569 | `USW` | US=user + world flag, US=United States + weight marker, user + SW=software, unknown + SW=switch, user-state-world chain, unknown / safety / weight shorthand |
| 0570 | `XRE` | XR=extended reality + entity flag, XR=unknown route + emotion marker, unknown + RE=repair, external + RE=response, unknown-role-entity chain, external / rule / emotion shorthand |
| 0571 | `BDS` | BD=boundary + state flag, BD=body + safety marker, bot + DS=data source, boundary + DS=decision state, bot-data-state chain, boundary / decision / safety shorthand |
| 0572 | `BDT` | BD=boundary + target flag, BD=body + truth marker, bot + DT=data, boundary + DT=decision tree, bot-data-target chain, boundary / decision / truth shorthand |
| 0573 | `XAD` | XA=unknown action + data flag, XA=external agent + decision marker, unknown + AD=advice, external + AD=ad, unknown-action-data chain, external / agent / decision shorthand |
| 0574 | `KRE` | KR=key route + entity flag, KR=kindness route + emotion marker, kindness + RE=repair, key + RE=response, kindness-role-entity chain, key / rule / emotion shorthand |
| 0575 | `RCM` | RC=recall + module flag, RC=record + mode marker, role + CM=command, rule + CM=context map, role-context-module chain, rule / control / mode shorthand |
| 0576 | `CRS` | CR=constraint route + state flag, CR=credit + safety marker, context + RS=response, control + RS=risk state, context-role-state chain, control / rule / safety shorthand |
| 0577 | `CRD` | CR=constraint route + data flag, CR=credit + decision marker, context + RD=read depth, control + RD=runtime depth, context-role-data chain, control / rule / decision shorthand |
| 0578 | `RDM` | RD=read depth + module flag, RD=runtime depth + mode marker, role + DM=direct message, rule + DM=decision matrix, role-data-module chain, rule / decision / mode shorthand |
| 0579 | `FLR` | FL=flow + role flag, FL=file layer + rule marker, function + LR=legal risk, filter + LR=learning rate, function-law-role chain, filter / logic / rule shorthand |
| 0580 | `FLT` | FL=flow + target flag, FL=file layer + truth marker, function + LT=limit, filter + LT=literal, function-law-target chain, filter / logic / truth shorthand |
| 0581 | `DMD` | DM=direct message + data flag, DM=decision matrix + decision marker, data + MD=markdown, decision + MD=medical, data-module-data chain, decision / mode / decision shorthand |
| 0582 | `DMT` | DM=direct message + target flag, DM=decision matrix + truth marker, data + MT=metric, decision + MT=meta, data-module-target chain, decision / mode / truth shorthand |
| 0583 | `YRC` | YR=year + context flag, YR=your + control marker, yes + RC=recall, why + RC=record, yes-role-context chain, why / rule / control shorthand |
| 0584 | `PMD` | PM=prompt module + data flag, PM=project manager + decision marker, prompt + MD=markdown, process + MD=medical, prompt-module-data chain, process / mode / decision shorthand |
| 0585 | `PMT` | PM=prompt module + target flag, PM=project manager + truth marker, prompt + MT=metric, process + MT=meta, prompt-module-target chain, process / mode / truth shorthand |
| 0586 | `RCL` | RC=recall + law flag, RC=record + logic marker, role + CL=class, rule + CL=clarity, role-context-law chain, rule / control / logic shorthand |
| 0587 | `CMT` | CM=command + target flag, CM=context map + truth marker, context + MT=metric, control + MT=meta, context-module-target chain, control / mode / truth shorthand |
| 0588 | `RCF` | RC=recall + function flag, RC=record + filter marker, role + CF=conflict, rule + CF=configuration, role-context-function chain, rule / control / filter shorthand |
| 0589 | `DMS` | DM=direct message + state flag, DM=decision matrix + safety marker, data + MS=model state, decision + MS=memory store, data-module-state chain, decision / mode / safety shorthand |
| 0590 | `MDM` | MD=markdown + module flag, MD=medical + mode marker, module + DM=direct message, mode + DM=decision matrix, module-data-module chain, mode / decision / mode shorthand |
| 0591 | `UXD` | UX=user experience + data flag, UX=unknown x + decision marker, user + XD=unknown data, unknown + XD=laugh emoticon, user-unknown-data chain, unknown / external / decision shorthand |
| 0592 | `PMS` | PM=prompt module + state flag, PM=project manager + safety marker, prompt + MS=model state, process + MS=memory store, prompt-module-state chain, process / mode / safety shorthand |
| 0593 | `TLR` | TL=token limit + role flag, TL=timeline + rule marker, target + LR=legal risk, truth + LR=learning rate, target-law-role chain, truth / logic / rule shorthand |
| 0594 | `WST` | WS=workspace + target flag, WS=warning signal + truth marker, world + ST=state, weight + ST=status, world-state-target chain, weight / safety / truth shorthand |
| 0595 | `CMS` | CM=command + state flag, CM=context map + safety marker, context + MS=model state, control + MS=memory store, context-module-state chain, control / mode / safety shorthand |
| 0596 | `TLT` | TL=token limit + target flag, TL=timeline + truth marker, target + LT=limit, truth + LT=literal, target-law-target chain, truth / logic / truth shorthand |
| 0597 | `UXT` | UX=user experience + target flag, UX=unknown x + truth marker, user + XT=external target, unknown + XT=unknown truth, user-unknown-target chain, unknown / external / truth shorthand |
| 0598 | `HPS` | HP=help + state flag, HP=harm prevention + safety marker, human + PS=prompt state, heart + PS=public safety, human-prompt-state chain, heart / process / safety shorthand |
| 0599 | `RDV` | RD=read depth + value flag, RD=runtime depth + veto marker, role + DV=developer, rule + DV=deviation, role-data-value chain, rule / decision / veto shorthand |
| 0600 | `UXS` | UX=user experience + state flag, UX=unknown x + safety marker, user + XS=excess, unknown + XS=unknown state, user-unknown-state chain, unknown / external / safety shorthand |
| 0601 | `HPT` | HP=help + target flag, HP=harm prevention + truth marker, human + PT=prompt token, heart + PT=passage/truth, human-prompt-target chain, heart / process / truth shorthand |
| 0602 | `VTR` | VT=veto + role flag, VT=validation target + rule marker, value + TR=truth, veto + TR=trace, value-target-role chain, veto / truth / rule shorthand |
| 0603 | `WTR` | WT=weight + role flag, WT=what + rule marker, world + TR=truth, weight + TR=trace, world-target-role chain, weight / truth / rule shorthand |
| 0604 | `YAS` | YA=yes action + state flag, YA=why-agent + safety marker, yes + AS=autism spectrum, why + AS=active state, yes-action-state chain, why / agent / safety shorthand |
| 0605 | `VRT` | VR=virtual reality + target flag, VR=veto route + truth marker, value + RT=runtime, veto + RT=real-time, value-role-target chain, veto / rule / truth shorthand |
| 0606 | `WRT` | WR=write + target flag, WR=warning route + truth marker, world + RT=runtime, weight + RT=real-time, world-role-target chain, weight / rule / truth shorthand |
| 0607 | `XAI` | XA=unknown action + intent flag, XA=external agent + input marker, unknown + AI=artificial intelligence, external + AI=assistant identity, unknown-action-intent chain, external / agent / input shorthand |
| 0608 | `YRE` | YR=year + entity flag, YR=your + emotion marker, yes + RE=repair, why + RE=response, yes-role-entity chain, why / rule / emotion shorthand |
| 0609 | `MDV` | MD=markdown + value flag, MD=medical + veto marker, module + DV=developer, mode + DV=deviation, module-data-value chain, mode / decision / veto shorthand |
| 0610 | `ADS` | AD=advice + state flag, AD=ad + safety marker, action + DS=data source, agent + DS=decision state, action-data-state chain, agent / decision / safety shorthand |
| 0611 | `ADT` | AD=advice + target flag, AD=ad + truth marker, action + DT=data, agent + DT=decision tree, action-data-target chain, agent / decision / truth shorthand |
| 0612 | `BDM` | BD=boundary + module flag, BD=body + mode marker, bot + DM=direct message, boundary + DM=decision matrix, bot-data-module chain, boundary / decision / mode shorthand |
| 0613 | `XAM` | XA=unknown action + module flag, XA=external agent + mode marker, unknown + AM=AMIMI, external + AM=anti-media, unknown-action-module chain, external / agent / mode shorthand |
| 0614 | `YAD` | YA=yes action + data flag, YA=why-agent + decision marker, yes + AD=advice, why + AD=ad, yes-action-data chain, why / agent / decision shorthand |
| 0615 | `XAU` | XA=unknown action + user flag, XA=external agent + unknown marker, unknown + AU=autism, external + AU=authority, unknown-action-user chain, external / agent / unknown shorthand |
| 0616 | `CRC` | CR=constraint route + context flag, CR=credit + control marker, context + RC=recall, control + RC=record, context-role-context chain, control / rule / control shorthand |
| 0617 | `VRS` | VR=virtual reality + state flag, VR=veto route + safety marker, value + RS=response, veto + RS=risk state, value-role-state chain, veto / rule / safety shorthand |
| 0618 | `VRD` | VR=virtual reality + data flag, VR=veto route + decision marker, value + RD=read depth, veto + RD=runtime depth, value-role-data chain, veto / rule / decision shorthand |
| 0619 | `FLC` | FL=flow + context flag, FL=file layer + control marker, function + LC=law/code, filter + LC=local context, function-law-context chain, filter / logic / control shorthand |
| 0620 | `RED` | English word 'red', RE=repair + data flag, RE=response + decision marker, role-entity-data chain, rule / emotion / decision shorthand, data/decision/depth suffix |
| 0621 | `WRS` | WR=write + state flag, WR=warning route + safety marker, world + RS=response, weight + RS=risk state, world-role-state chain, weight / rule / safety shorthand |
| 0622 | `WRD` | WR=write + data flag, WR=warning route + decision marker, world + RD=read depth, weight + RD=runtime depth, world-role-data chain, weight / rule / decision shorthand |
| 0623 | `IDS` | ID=identity + state flag, ID=identifier + safety marker, intent + DS=data source, input + DS=decision state, intent-data-state chain, input / decision / safety shorthand |
| 0624 | `BDV` | BD=boundary + value flag, BD=body + veto marker, bot + DV=developer, boundary + DV=deviation, bot-data-value chain, boundary / decision / veto shorthand |
| 0625 | `IDT` | ID=identity + target flag, ID=identifier + truth marker, intent + DT=data, input + DT=decision tree, intent-data-target chain, input / decision / truth shorthand |
| 0626 | `LTD` | LT=limit + data flag, LT=literal + decision marker, law + TD=task drift, logic + TD=temporal difference, law-target-data chain, logic / truth / decision shorthand |
| 0627 | `TLC` | TL=token limit + context flag, TL=timeline + control marker, target + LC=law/code, truth + LC=local context, target-law-context chain, truth / logic / control shorthand |
| 0628 | `DMO` | DM=direct message + output flag, DM=decision matrix + object marker, data + MO=mode, decision + MO=moral, data-module-output chain, decision / mode / object shorthand |
| 0629 | `CRE` | CR=constraint route + entity flag, CR=credit + emotion marker, context + RE=repair, control + RE=response, context-role-entity chain, control / rule / emotion shorthand |
| 0630 | `PMO` | PM=prompt module + output flag, PM=project manager + object marker, prompt + MO=mode, process + MO=moral, prompt-module-output chain, process / mode / object shorthand |
| 0631 | `FLG` | FL=flow + goal flag, FL=file layer + guard marker, function + LG=language, filter + LG=logic gate, function-law-goal chain, filter / logic / guard shorthand |
| 0632 | `IPS` | IP=internet protocol + state flag, IP=intellectual property + safety marker, intent + PS=prompt state, input + PS=public safety, intent-prompt-state chain, input / process / safety shorthand |
| 0633 | `UXA` | UX=user experience + action flag, UX=unknown x + agent marker, user + XA=unknown action, unknown + XA=external agent, user-unknown-action chain, unknown / external / agent shorthand |
| 0634 | `CMO` | CM=command + output flag, CM=context map + object marker, context + MO=mode, control + MO=moral, context-module-output chain, control / mode / object shorthand |
| 0635 | `IPT` | IP=internet protocol + target flag, IP=intellectual property + truth marker, intent + PT=prompt token, input + PT=passage/truth, intent-prompt-target chain, input / process / truth shorthand |
| 0636 | `HPM` | HP=help + module flag, HP=harm prevention + mode marker, human + PM=prompt module, heart + PM=project manager, human-prompt-module chain, heart / process / mode shorthand |
| 0637 | `LGT` | LG=language + target flag, LG=logic gate + truth marker, law + GT=goal target, logic + GT=greater than, law-goal-target chain, logic / guard / truth shorthand |
| 0638 | `DML` | DM=direct message + law flag, DM=decision matrix + logic marker, data + ML=model, decision + ML=machine learning, data-module-law chain, decision / mode / logic shorthand |
| 0639 | `DRY` | English word 'dry', DR=drift + yes flag, DR=doctor + why marker, data-role-yes chain, decision / rule / why shorthand |
| 0640 | `TRY` | English word 'try', TR=truth + yes flag, TR=trace + why marker, target-role-yes chain, truth / rule / why shorthand |
| 0641 | `PML` | PM=prompt module + law flag, PM=project manager + logic marker, prompt + ML=model, process + ML=machine learning, prompt-module-law chain, process / mode / logic shorthand |
| 0642 | `TLG` | TL=token limit + goal flag, TL=timeline + guard marker, target + LG=language, truth + LG=logic gate, target-law-goal chain, truth / logic / guard shorthand |
| 0643 | `CML` | CM=command + law flag, CM=context map + logic marker, context + ML=model, control + ML=machine learning, context-module-law chain, control / mode / logic shorthand |
| 0644 | `LGR` | LG=language + role flag, LG=logic gate + rule marker, law + GR=grader, logic + GR=guard route, law-goal-role chain, logic / guard / rule shorthand |
| 0645 | `HPU` | HP=help + user flag, HP=harm prevention + unknown marker, human + PU=pickup, heart + PU=public/user, human-prompt-user chain, heart / process / unknown shorthand |
| 0646 | `YAI` | YA=yes action + intent flag, YA=why-agent + input marker, yes + AI=artificial intelligence, why + AI=assistant identity, yes-action-intent chain, why / agent / input shorthand |
| 0647 | `JSD` | JS=JavaScript + data flag, JS=judge state + decision marker, judge + SD=system drift, job + SD=stable diffusion, judge-state-data chain, job / safety / decision shorthand |
| 0648 | `LGD` | LG=language + data flag, LG=logic gate + decision marker, law + GD=good, logic + GD=guard, law-goal-data chain, logic / guard / decision shorthand |
| 0649 | `ADM` | AD=advice + module flag, AD=ad + mode marker, action + DM=direct message, agent + DM=decision matrix, action-data-module chain, agent / decision / mode shorthand |
| 0650 | `YAM` | YA=yes action + module flag, YA=why-agent + mode marker, yes + AM=AMIMI, why + AM=anti-media, yes-action-module chain, why / agent / mode shorthand |
| 0651 | `JSR` | JS=JavaScript + role flag, JS=judge state + rule marker, judge + SR=source, job + SR=safety route, judge-state-role chain, job / safety / rule shorthand |
| 0652 | `GTD` | GT=goal target + data flag, GT=greater than + decision marker, goal + TD=task drift, guard + TD=temporal difference, goal-target-data chain, guard / truth / decision shorthand |
| 0653 | `VRC` | VR=virtual reality + context flag, VR=veto route + control marker, value + RC=recall, veto + RC=record, value-role-context chain, veto / rule / control shorthand |
| 0654 | `ART` | English word 'art', action + RT=runtime, agent + RT=real-time, action-role-target chain, agent / rule / truth shorthand, target/task/trace suffix |
| 0655 | `YAU` | YA=yes action + user flag, YA=why-agent + unknown marker, yes + AU=autism, why + AU=authority, yes-action-user chain, why / agent / unknown shorthand |
| 0656 | `WRC` | WR=write + context flag, WR=warning route + control marker, world + RC=recall, weight + RC=record, world-role-context chain, weight / rule / control shorthand |
| 0657 | `TLW` | TL=token limit + world flag, TL=timeline + weight marker, target + LW=law, truth + LW=low weight, target-law-world chain, truth / logic / weight shorthand |
| 0658 | `XSD` | XS=excess + data flag, XS=unknown state + decision marker, unknown + SD=system drift, external + SD=stable diffusion, unknown-state-data chain, external / safety / decision shorthand |
| 0659 | `LTC` | LT=limit + context flag, LT=literal + control marker, law + TC=task class, logic + TC=truth constraint, law-target-context chain, logic / truth / control shorthand |
| 0660 | `MOM` | English word 'mom', MO=mode + module flag, MO=moral + mode marker, module-output-module chain, mode / object / mode shorthand, mode/model/module suffix |
| 0661 | `GLR` | GL=gloss + role flag, GL=global + rule marker, goal + LR=legal risk, guard + LR=learning rate, goal-law-role chain, guard / logic / rule shorthand |
| 0662 | `LTM` | LT=limit + module flag, LT=literal + mode marker, law + TM=trademark, logic + TM=tone mode, law-target-module chain, logic / truth / mode shorthand |
| 0663 | `GLT` | GL=gloss + target flag, GL=global + truth marker, goal + LT=limit, guard + LT=literal, goal-law-target chain, guard / logic / truth shorthand |
| 0664 | `XSR` | XS=excess + role flag, XS=unknown state + rule marker, unknown + SR=source, external + SR=safety route, unknown-state-role chain, external / safety / rule shorthand |
| 0665 | `LTP` | LT=limit + prompt flag, LT=literal + process marker, law + TP=target prompt, logic + TP=true positive, law-target-prompt chain, logic / truth / process shorthand |
| 0666 | `OPS` | OP=output + state flag, OP=operation + safety marker, output + PS=prompt state, object + PS=public safety, output-prompt-state chain, object / process / safety shorthand |
| 0667 | `ADV` | AD=advice + value flag, AD=ad + veto marker, action + DV=developer, agent + DV=deviation, action-data-value chain, agent / decision / veto shorthand |
| 0668 | `IDM` | ID=identity + module flag, ID=identifier + mode marker, intent + DM=direct message, input + DM=decision matrix, intent-data-module chain, input / decision / mode shorthand |
| 0669 | `AUN` | AU=autism + name flag, AU=authority + no marker, action + UN=undefined, agent + UN=unknown, action-user-name chain, agent / unknown / no shorthand |
| 0670 | `AIR` | English word 'air', AI=artificial intelligence + role flag, AI=assistant identity + rule marker, action-intent-role chain, agent / input / rule shorthand, route/risk/repair suffix |
| 0671 | `LTL` | LT=limit + law flag, LT=literal + logic marker, law + TL=token limit, logic + TL=timeline, law-target-law chain, logic / truth / logic shorthand |
| 0672 | `VRE` | VR=virtual reality + entity flag, VR=veto route + emotion marker, value + RE=repair, veto + RE=response, value-role-entity chain, veto / rule / emotion shorthand |
| 0673 | `WRE` | WR=write + entity flag, WR=warning route + emotion marker, world + RE=repair, weight + RE=response, world-role-entity chain, weight / rule / emotion shorthand |
| 0674 | `IPM` | IP=internet protocol + module flag, IP=intellectual property + mode marker, intent + PM=prompt module, input + PM=project manager, intent-prompt-module chain, input / process / mode shorthand |
| 0675 | `KNO` | KN=known + output flag, KN=kindness/niceness + object marker, kindness + NO=negation, key + NO=no, kindness-name-output chain, key / no / object shorthand |
| 0676 | `PUS` | PU=pickup + state flag, PU=public/user + safety marker, prompt + US=user, process + US=United States, prompt-user-state chain, process / unknown / safety shorthand |
| 0677 | `PUX` | PU=pickup + unknown flag, PU=public/user + external marker, prompt + UX=user experience, process + UX=unknown x, prompt-user-unknown chain, process / unknown / external shorthand |
| 0678 | `KNA` | KN=known + action flag, KN=kindness/niceness + agent marker, kindness + NA=not applicable, key + NA=name, kindness-name-action chain, key / no / agent shorthand |
| 0679 | `MIX` | English word 'mix', MI=IMAMI + unknown flag, MI=machine intelligence + external marker, module-intent-unknown chain, mode / input / external shorthand, unknown or experimental placeholder |
| 0680 | `KNV` | KN=known + value flag, KN=kindness/niceness + veto marker, kindness + NV=nearest valid, key + NV=nonviolent, kindness-name-value chain, key / no / veto shorthand |
| 0681 | `PUR` | PU=pickup + role flag, PU=public/user + rule marker, prompt + UR=user route, process + UR=urgent, prompt-user-role chain, process / unknown / rule shorthand |
| 0682 | `GTC` | GT=goal target + context flag, GT=greater than + control marker, goal + TC=task class, guard + TC=truth constraint, goal-target-context chain, guard / truth / control shorthand |
| 0683 | `DMI` | DM=direct message + intent flag, DM=decision matrix + input marker, data + MI=IMAMI, decision + MI=machine intelligence, data-module-intent chain, decision / mode / input shorthand |
| 0684 | `IDV` | ID=identity + value flag, ID=identifier + veto marker, intent + DV=developer, input + DV=deviation, intent-data-value chain, input / decision / veto shorthand |
| 0685 | `IPU` | IP=internet protocol + user flag, IP=intellectual property + unknown marker, intent + PU=pickup, input + PU=public/user, intent-prompt-user chain, input / process / unknown shorthand |
| 0686 | `PMI` | PM=prompt module + intent flag, PM=project manager + input marker, prompt + MI=IMAMI, process + MI=machine intelligence, prompt-module-intent chain, process / mode / input shorthand |
| 0687 | `GTM` | GT=goal target + module flag, GT=greater than + mode marker, goal + TM=trademark, guard + TM=tone mode, goal-target-module chain, guard / truth / mode shorthand |
| 0688 | `CMI` | CM=command + intent flag, CM=context map + input marker, context + MI=IMAMI, control + MI=machine intelligence, context-module-intent chain, control / mode / input shorthand |
| 0689 | `KLR` | KL=kill + role flag, KL=key layer + rule marker, kindness + LR=legal risk, key + LR=learning rate, kindness-law-role chain, key / logic / rule shorthand |
| 0690 | `DMA` | DM=direct message + action flag, DM=decision matrix + agent marker, data + MA=AMAMI, decision + MA=moral authority, data-module-action chain, decision / mode / agent shorthand |
| 0691 | `UCS` | UC=user context + state flag, UC=use case + safety marker, user + CS=case, unknown + CS=context state, user-context-state chain, unknown / control / safety shorthand |
| 0692 | `KNE` | KN=known + entity flag, KN=kindness/niceness + emotion marker, kindness + NE=nearest, key + NE=negative, kindness-name-entity chain, key / no / emotion shorthand |
| 0693 | `KLT` | KL=kill + target flag, KL=key layer + truth marker, kindness + LT=limit, key + LT=literal, kindness-law-target chain, key / logic / truth shorthand |
| 0694 | `PMA` | PM=prompt module + action flag, PM=project manager + agent marker, prompt + MA=AMAMI, process + MA=moral authority, prompt-module-action chain, process / mode / agent shorthand |
| 0695 | `GTP` | GT=goal target + prompt flag, GT=greater than + process marker, goal + TP=target prompt, guard + TP=true positive, goal-target-prompt chain, guard / truth / process shorthand |
| 0696 | `UCR` | UC=user context + role flag, UC=use case + rule marker, user + CR=constraint route, unknown + CR=credit, user-context-role chain, unknown / control / rule shorthand |
| 0697 | `CMA` | CM=command + action flag, CM=context map + agent marker, context + MA=AMAMI, control + MA=moral authority, context-module-action chain, control / mode / agent shorthand |
| 0698 | `UCD` | UC=user context + data flag, UC=use case + decision marker, user + CD=code, unknown + CD=clinical diagnosis, user-context-data chain, unknown / control / decision shorthand |
| 0699 | `JSC` | JS=JavaScript + context flag, JS=judge state + control marker, judge + SC=scope, job + SC=self-control, judge-state-context chain, job / safety / control shorthand |
| 0700 | `XTD` | XT=external target + data flag, XT=unknown truth + decision marker, unknown + TD=task drift, external + TD=temporal difference, unknown-target-data chain, external / truth / decision shorthand |
| 0701 | `LGC` | LG=language + context flag, LG=logic gate + control marker, law + GC=garbage collection, logic + GC=guard core, law-goal-context chain, logic / guard / control shorthand |
| 0702 | `KTD` | KT=key token + data flag, KT=knowledge transfer + decision marker, kindness + TD=task drift, key + TD=temporal difference, kindness-target-data chain, key / truth / decision shorthand |
| 0703 | `SDS` | SD=system drift + state flag, SD=stable diffusion + safety marker, state + DS=data source, safety + DS=decision state, state-data-state chain, safety / decision / safety shorthand |
| 0704 | `GTL` | GT=goal target + law flag, GT=greater than + logic marker, goal + TL=token limit, guard + TL=timeline, goal-target-law chain, guard / truth / logic shorthand |
| 0705 | `JSP` | JS=JavaScript + prompt flag, JS=judge state + process marker, judge + SP=system prompt, job + SP=special, judge-state-prompt chain, job / safety / process shorthand |
| 0706 | `SDT` | SD=system drift + target flag, SD=stable diffusion + truth marker, state + DT=data, safety + DT=decision tree, state-data-target chain, safety / decision / truth shorthand |
| 0707 | `GLC` | GL=gloss + context flag, GL=global + control marker, goal + LC=law/code, guard + LC=local context, goal-law-context chain, guard / logic / control shorthand |
| 0708 | `SCS` | SC=scope + state flag, SC=self-control + safety marker, state + CS=case, safety + CS=context state, state-context-state chain, safety / control / safety shorthand |
| 0709 | `XSC` | XS=excess + context flag, XS=unknown state + control marker, unknown + SC=scope, external + SC=self-control, unknown-state-context chain, external / safety / control shorthand |
| 0710 | `JSW` | JS=JavaScript + world flag, JS=judge state + weight marker, judge + SW=software, job + SW=switch, judge-state-world chain, job / safety / weight shorthand |
| 0711 | `SCR` | SC=scope + role flag, SC=self-control + rule marker, state + CR=constraint route, safety + CR=credit, state-context-role chain, safety / control / rule shorthand |
| 0712 | `ARC` | English word 'arc', action + RC=recall, agent + RC=record, action-role-context chain, agent / rule / control shorthand |
| 0713 | `SCD` | SC=scope + data flag, SC=self-control + decision marker, state + CD=code, safety + CD=clinical diagnosis, state-context-data chain, safety / control / decision shorthand |
| 0714 | `XSP` | XS=excess + prompt flag, XS=unknown state + process marker, unknown + SP=system prompt, external + SP=special, unknown-state-prompt chain, external / safety / process shorthand |
| 0715 | `SPS` | SP=system prompt + state flag, SP=special + safety marker, state + PS=prompt state, safety + PS=public safety, state-prompt-state chain, safety / process / safety shorthand |
| 0716 | `JGT` | JG=judging + target flag, JG=judge gate + truth marker, judge + GT=goal target, job + GT=greater than, judge-goal-target chain, job / guard / truth shorthand |
| 0717 | `OPM` | OP=output + module flag, OP=operation + mode marker, output + PM=prompt module, object + PM=project manager, output-prompt-module chain, object / process / mode shorthand |
| 0718 | `SPT` | SP=system prompt + target flag, SP=special + truth marker, state + PT=prompt token, safety + PT=passage/truth, state-prompt-target chain, safety / process / truth shorthand |
| 0719 | `NVT` | NV=nearest valid + target flag, NV=nonviolent + truth marker, name + VT=veto, no + VT=validation target, name-value-target chain, no / veto / truth shorthand |
| 0720 | `NVR` | NV=nearest valid + role flag, NV=nonviolent + rule marker, name + VR=virtual reality, no + VR=veto route, name-value-role chain, no / veto / rule shorthand |
| 0721 | `JGR` | JG=judging + role flag, JG=judge gate + rule marker, judge + GR=grader, job + GR=guard route, judge-goal-role chain, job / guard / rule shorthand |
| 0722 | `GLG` | GL=gloss + goal flag, GL=global + guard marker, goal + LG=language, guard + LG=logic gate, goal-law-goal chain, guard / logic / guard shorthand |
| 0723 | `SWS` | SW=software + state flag, SW=switch + safety marker, state + WS=workspace, safety + WS=warning signal, state-world-state chain, safety / weight / safety shorthand |
| 0724 | `XSW` | XS=excess + world flag, XS=unknown state + weight marker, unknown + SW=software, external + SW=switch, unknown-state-world chain, external / safety / weight shorthand |
| 0725 | `SWT` | SW=software + target flag, SW=switch + truth marker, state + WT=weight, safety + WT=what, state-world-target chain, safety / weight / truth shorthand |
| 0726 | `JGD` | JG=judging + data flag, JG=judge gate + decision marker, judge + GD=good, job + GD=guard, judge-goal-data chain, job / guard / decision shorthand |
| 0727 | `SWR` | SW=software + role flag, SW=switch + rule marker, state + WR=write, safety + WR=warning route, state-world-role chain, safety / weight / rule shorthand |
| 0728 | `YNO` | YN=yes/no + output flag, YN=why-not + object marker, yes + NO=negation, why + NO=no, yes-name-output chain, why / no / object shorthand |
| 0729 | `OPU` | OP=output + user flag, OP=operation + unknown marker, output + PU=pickup, object + PU=public/user, output-prompt-user chain, object / process / unknown shorthand |
| 0730 | `DSD` | DS=data source + data flag, DS=decision state + decision marker, data + SD=system drift, decision + SD=stable diffusion, data-state-data chain, decision / safety / decision shorthand |
| 0731 | `INK` | English word 'ink', IN=input + kindness flag, IN=instruction + key marker, intent-name-kindness chain, input / no / key shorthand, key/kernel/kindness suffix |
| 0732 | `NEX` | NE=nearest + unknown flag, NE=negative + external marker, name + EX=execute, no + EX=example, name-entity-unknown chain, no / emotion / external shorthand |
| 0733 | `YNA` | YN=yes/no + action flag, YN=why-not + agent marker, yes + NA=not applicable, why + NA=name, yes-name-action chain, why / no / agent shorthand |
| 0734 | `PSD` | PS=prompt state + data flag, PS=public safety + decision marker, prompt + SD=system drift, process + SD=stable diffusion, prompt-state-data chain, process / safety / decision shorthand |
| 0735 | `YNV` | YN=yes/no + value flag, YN=why-not + veto marker, yes + NV=nearest valid, why + NV=nonviolent, yes-name-value chain, why / no / veto shorthand |
| 0736 | `CSD` | CS=case + data flag, CS=context state + decision marker, context + SD=system drift, control + SD=stable diffusion, context-state-data chain, control / safety / decision shorthand |
| 0737 | `DSR` | DS=data source + role flag, DS=decision state + rule marker, data + SR=source, decision + SR=safety route, data-state-role chain, decision / safety / rule shorthand |
| 0738 | `XTC` | XT=external target + context flag, XT=unknown truth + control marker, unknown + TC=task class, external + TC=truth constraint, unknown-target-context chain, external / truth / control shorthand |
| 0739 | `KLC` | KL=kill + context flag, KL=key layer + control marker, kindness + LC=law/code, key + LC=local context, kindness-law-context chain, key / logic / control shorthand |
| 0740 | `HAS` | English word 'has', human + AS=autism spectrum, heart + AS=active state, human-action-state chain, heart / agent / safety shorthand, state/safety/source suffix |
| 0741 | `PSR` | PS=prompt state + role flag, PS=public safety + rule marker, prompt + SR=source, process + SR=safety route, prompt-state-role chain, process / safety / rule shorthand |
| 0742 | `KTC` | KT=key token + context flag, KT=knowledge transfer + control marker, kindness + TC=task class, key + TC=truth constraint, kindness-target-context chain, key / truth / control shorthand |
| 0743 | `CSR` | CS=case + role flag, CS=context state + rule marker, context + SR=source, control + SR=safety route, context-state-role chain, control / safety / rule shorthand |
| 0744 | `XTM` | XT=external target + module flag, XT=unknown truth + mode marker, unknown + TM=trademark, external + TM=tone mode, unknown-target-module chain, external / truth / mode shorthand |
| 0745 | `GLW` | GL=gloss + world flag, GL=global + weight marker, goal + LW=law, guard + LW=low weight, goal-law-world chain, guard / logic / weight shorthand |
| 0746 | `KTM` | KT=key token + module flag, KT=knowledge transfer + mode marker, kindness + TM=trademark, key + TM=tone mode, kindness-target-module chain, key / truth / mode shorthand |
| 0747 | `YNE` | YN=yes/no + entity flag, YN=why-not + emotion marker, yes + NE=nearest, why + NE=negative, yes-name-entity chain, why / no / emotion shorthand |
| 0748 | `TCS` | TC=task class + state flag, TC=truth constraint + safety marker, target + CS=case, truth + CS=context state, target-context-state chain, truth / control / safety shorthand |
| 0749 | `PAD` | English word 'pad', prompt + AD=advice, process + AD=ad, prompt-action-data chain, process / agent / decision shorthand, data/decision/depth suffix |
| 0750 | `PUC` | PU=pickup + context flag, PU=public/user + control marker, prompt + UC=user context, process + UC=use case, prompt-user-context chain, process / unknown / control shorthand |
| 0751 | `UCM` | UC=user context + module flag, UC=use case + mode marker, user + CM=command, unknown + CM=context map, user-context-module chain, unknown / control / mode shorthand |
| 0752 | `XTP` | XT=external target + prompt flag, XT=unknown truth + process marker, unknown + TP=target prompt, external + TP=true positive, unknown-target-prompt chain, external / truth / process shorthand |
| 0753 | `TCR` | TC=task class + role flag, TC=truth constraint + rule marker, target + CR=constraint route, truth + CR=credit, target-context-role chain, truth / control / rule shorthand |
| 0754 | `KTP` | KT=key token + prompt flag, KT=knowledge transfer + process marker, kindness + TP=target prompt, key + TP=true positive, kindness-target-prompt chain, key / truth / process shorthand |
| 0755 | `TCD` | TC=task class + data flag, TC=truth constraint + decision marker, target + CD=code, truth + CD=clinical diagnosis, target-context-data chain, truth / control / decision shorthand |
| 0756 | `PUA` | PU=pickup + action flag, PU=public/user + agent marker, prompt + UA=user agency, process + UA=Ukraine, prompt-user-action chain, process / unknown / agent shorthand |
| 0757 | `JKT` | JK=joke + target flag, JK=judge/key + truth marker, judge + KT=key token, job + KT=knowledge transfer, judge-kindness-target chain, job / key / truth shorthand |
| 0758 | `HAD` | English word 'had', human + AD=advice, heart + AD=ad, human-action-data chain, heart / agent / decision shorthand, data/decision/depth suffix |
| 0759 | `STX` | ST=state + unknown flag, ST=status + external marker, state-target-unknown chain, safety / truth / external shorthand, unknown or experimental placeholder |
| 0760 | `FEX` | FE=feeling + unknown flag, FE=feature + external marker, function + EX=execute, filter + EX=example, function-entity-unknown chain, filter / emotion / external shorthand |
| 0761 | `MAN` | English word 'man', MA=AMAMI + name flag, MA=moral authority + no marker, module-action-name chain, mode / agent / no shorthand |
| 0762 | `SWK` | SW=software + kindness flag, SW=switch + key marker, state + WK=work, safety + WK=weakness key, state-world-kindness chain, safety / weight / key shorthand |
| 0763 | `YTD` | YT=YouTube + data flag, YT=why target + decision marker, yes + TD=task drift, why + TD=temporal difference, yes-target-data chain, why / truth / decision shorthand |
| 0764 | `XTL` | XT=external target + law flag, XT=unknown truth + logic marker, unknown + TL=token limit, external + TL=timeline, unknown-target-law chain, external / truth / logic shorthand |
| 0765 | `TPS` | TP=target prompt + state flag, TP=true positive + safety marker, target + PS=prompt state, truth + PS=public safety, target-prompt-state chain, truth / process / safety shorthand |
| 0766 | `JKR` | JK=joke + role flag, JK=judge/key + rule marker, judge + KR=key route, job + KR=kindness route, judge-kindness-role chain, job / key / rule shorthand |
| 0767 | `TDS` | TD=task drift + state flag, TD=temporal difference + safety marker, target + DS=data source, truth + DS=decision state, target-data-state chain, truth / decision / safety shorthand |
| 0768 | `KTL` | KT=key token + law flag, KT=knowledge transfer + logic marker, kindness + TL=token limit, key + TL=timeline, kindness-target-law chain, key / truth / logic shorthand |
| 0769 | `QCS` | QC=quality control + state flag, QC=question context + safety marker, question + CS=case, query + CS=context state, question-context-state chain, query / control / safety shorthand |
| 0770 | `SDM` | SD=system drift + module flag, SD=stable diffusion + mode marker, state + DM=direct message, safety + DM=decision matrix, state-data-module chain, safety / decision / mode shorthand |
| 0771 | `TPT` | TP=target prompt + target flag, TP=true positive + truth marker, target + PT=prompt token, truth + PT=passage/truth, target-prompt-target chain, truth / process / truth shorthand |
| 0772 | `TDT` | TD=task drift + target flag, TD=temporal difference + truth marker, target + DT=data, truth + DT=decision tree, target-data-target chain, truth / decision / truth shorthand |
| 0773 | `KLG` | KL=kill + goal flag, KL=key layer + guard marker, kindness + LG=language, key + LG=logic gate, kindness-law-goal chain, key / logic / guard shorthand |
| 0774 | `ZTD` | ZT=zero target + data flag, ZT=final token + decision marker, zero + TD=task drift, final state + TD=temporal difference, zero-target-data chain, final state / truth / decision shorthand |
| 0775 | `QCR` | QC=quality control + role flag, QC=question context + rule marker, question + CR=constraint route, query + CR=credit, question-context-role chain, query / control / rule shorthand |
| 0776 | `QDS` | QD=query depth + state flag, QD=question directive + safety marker, question + DS=data source, query + DS=decision state, question-data-state chain, query / decision / safety shorthand |
| 0777 | `DRR` | DR=drift + role flag, DR=doctor + rule marker, data-role-role chain, decision / rule / rule shorthand, route/risk/repair suffix |
| 0778 | `FWS` | FW=forward + state flag, FW=framework + safety marker, function + WS=workspace, filter + WS=warning signal, function-world-state chain, filter / weight / safety shorthand |
| 0779 | `QCD` | QC=quality control + data flag, QC=question context + decision marker, question + CD=code, query + CD=clinical diagnosis, question-context-data chain, query / control / decision shorthand |
| 0780 | `QDT` | QD=query depth + target flag, QD=question directive + truth marker, question + DT=data, query + DT=decision tree, question-data-target chain, query / decision / truth shorthand |
| 0781 | `TRR` | TR=truth + role flag, TR=trace + rule marker, target-role-role chain, truth / rule / rule shorthand, route/risk/repair suffix |
| 0782 | `DRX` | DR=drift + unknown flag, DR=doctor + external marker, data-role-unknown chain, decision / rule / external shorthand, unknown or experimental placeholder |
| 0783 | `RTS` | RT=runtime + state flag, RT=real-time + safety marker, role-target-state chain, rule / truth / safety shorthand, state/safety/source suffix |
| 0784 | `FWT` | FW=forward + target flag, FW=framework + truth marker, function + WT=weight, filter + WT=what, function-world-target chain, filter / weight / truth shorthand |
| 0785 | `TRX` | TR=truth + unknown flag, TR=trace + external marker, target-role-unknown chain, truth / rule / external shorthand, unknown or experimental placeholder |
| 0786 | `UCL` | UC=user context + law flag, UC=use case + logic marker, user + CL=class, unknown + CL=clarity, user-context-law chain, unknown / control / logic shorthand |
| 0787 | `RTT` | RT=runtime + target flag, RT=real-time + truth marker, role-target-target chain, rule / truth / truth shorthand, target/task/trace suffix |
| 0788 | `FWR` | FW=forward + role flag, FW=framework + rule marker, function + WR=write, filter + WR=warning route, function-world-role chain, filter / weight / rule shorthand |
| 0789 | `UCF` | UC=user context + function flag, UC=use case + filter marker, user + CF=conflict, unknown + CF=configuration, user-context-function chain, unknown / control / filter shorthand |
| 0790 | `SCM` | SC=scope + module flag, SC=self-control + mode marker, state + CM=command, safety + CM=context map, state-context-module chain, safety / control / mode shorthand |
| 0791 | `RTX` | RT=runtime + unknown flag, RT=real-time + external marker, role-target-unknown chain, rule / truth / external shorthand, unknown or experimental placeholder |
| 0792 | `MAY` | English word 'may', MA=AMAMI + yes flag, MA=moral authority + why marker, module-action-yes chain, mode / agent / why shorthand |
| 0793 | `SPM` | SP=system prompt + module flag, SP=special + mode marker, state + PM=prompt module, safety + PM=project manager, state-prompt-module chain, safety / process / mode shorthand |
| 0794 | `CTS` | CT=context + state flag, CT=control + safety marker, context-target-state chain, control / truth / safety shorthand, state/safety/source suffix |
| 0795 | `CTT` | CT=context + target flag, CT=control + truth marker, context-target-target chain, control / truth / truth shorthand, target/task/trace suffix |
| 0796 | `STK` | ST=state + kindness flag, ST=status + key marker, state-target-kindness chain, safety / truth / key shorthand, key/kernel/kindness suffix |
| 0797 | `KLW` | KL=kill + world flag, KL=key layer + weight marker, kindness + LW=law, key + LW=low weight, kindness-law-world chain, key / logic / weight shorthand |
| 0798 | `LCS` | LC=law/code + state flag, LC=local context + safety marker, law + CS=case, logic + CS=context state, law-context-state chain, logic / control / safety shorthand |
| 0799 | `CLR` | CL=class + role flag, CL=clarity + rule marker, context + LR=legal risk, control + LR=learning rate, context-law-role chain, control / logic / rule shorthand |
| 0800 | `SDV` | SD=system drift + value flag, SD=stable diffusion + veto marker, state + DV=developer, safety + DV=deviation, state-data-value chain, safety / decision / veto shorthand |
| 0801 | `DTD` | DT=data + data flag, DT=decision tree + decision marker, data + TD=task drift, decision + TD=temporal difference, data-target-data chain, decision / truth / decision shorthand |
| 0802 | `PRR` | PR=prompt + role flag, PR=process + rule marker, prompt-role-role chain, process / rule / rule shorthand, route/risk/repair suffix |
| 0803 | `CLT` | CL=class + target flag, CL=clarity + truth marker, context + LT=limit, control + LT=literal, context-law-target chain, control / logic / truth shorthand |
| 0804 | `LCR` | LC=law/code + role flag, LC=local context + rule marker, law + CR=constraint route, logic + CR=credit, law-context-role chain, logic / control / rule shorthand |
| 0805 | `SCL` | SC=scope + law flag, SC=self-control + logic marker, state + CL=class, safety + CL=clarity, state-context-law chain, safety / control / logic shorthand |
| 0806 | `LCD` | LC=law/code + data flag, LC=local context + decision marker, law + CD=code, logic + CD=clinical diagnosis, law-context-data chain, logic / control / decision shorthand |
| 0807 | `CFO` | CF=conflict + output flag, CF=configuration + object marker, context + FO=foe, control + FO=form, context-function-output chain, control / filter / object shorthand |
| 0808 | `PTD` | PT=prompt token + data flag, PT=passage/truth + decision marker, prompt + TD=task drift, process + TD=temporal difference, prompt-target-data chain, process / truth / decision shorthand |
| 0809 | `CFA` | CF=conflict + action flag, CF=configuration + agent marker, context + FA=false, control + FA=fallback, context-function-action chain, control / filter / agent shorthand |
| 0810 | `SCF` | SC=scope + function flag, SC=self-control + filter marker, state + CF=conflict, safety + CF=configuration, state-context-function chain, safety / control / filter shorthand |
| 0811 | `SPU` | SP=system prompt + user flag, SP=special + unknown marker, state + PU=pickup, safety + PU=public/user, state-prompt-user chain, safety / process / unknown shorthand |
| 0812 | `DRK` | DR=drift + kindness flag, DR=doctor + key marker, data-role-kindness chain, decision / rule / key shorthand, key/kernel/kindness suffix |
| 0813 | `GAS` | English word 'gas', goal + AS=autism spectrum, guard + AS=active state, goal-action-state chain, guard / agent / safety shorthand, state/safety/source suffix |
| 0814 | `RSS` | RS=response + state flag, RS=risk state + safety marker, role-state-state chain, rule / safety / safety shorthand, state/safety/source suffix |
| 0815 | `JGC` | JG=judging + context flag, JG=judge gate + control marker, judge + GC=garbage collection, job + GC=guard core, judge-goal-context chain, job / guard / control shorthand |
| 0816 | `TRK` | TR=truth + kindness flag, TR=trace + key marker, target-role-kindness chain, truth / rule / key shorthand, key/kernel/kindness suffix |
| 0817 | `RCX` | RC=recall + unknown flag, RC=record + external marker, role-context-unknown chain, rule / control / external shorthand, unknown or experimental placeholder |
| 0818 | `DSC` | DS=data source + context flag, DS=decision state + control marker, data + SC=scope, decision + SC=self-control, data-state-context chain, decision / safety / control shorthand |
| 0819 | `CFI` | CF=conflict + intent flag, CF=configuration + input marker, context + FI=file, control + FI=filter, context-function-intent chain, control / filter / input shorthand |
| 0820 | `FWK` | FW=forward + kindness flag, FW=framework + key marker, function + WK=work, filter + WK=weakness key, function-world-kindness chain, filter / weight / key shorthand |
| 0821 | `RSX` | RS=response + unknown flag, RS=risk state + external marker, role-state-unknown chain, rule / safety / external shorthand, unknown or experimental placeholder |
| 0822 | `RTK` | RT=runtime + kindness flag, RT=real-time + key marker, role-target-kindness chain, rule / truth / key shorthand, key/kernel/kindness suffix |
| 0823 | `RDD` | RD=read depth + data flag, RD=runtime depth + decision marker, role-data-data chain, rule / decision / decision shorthand, data/decision/depth suffix |
| 0824 | `RDX` | RD=read depth + unknown flag, RD=runtime depth + external marker, role-data-unknown chain, rule / decision / external shorthand, unknown or experimental placeholder |
| 0825 | `WSD` | WS=workspace + data flag, WS=warning signal + decision marker, world + SD=system drift, weight + SD=stable diffusion, world-state-data chain, weight / safety / decision shorthand |
| 0826 | `PSC` | PS=prompt state + context flag, PS=public safety + control marker, prompt + SC=scope, process + SC=self-control, prompt-state-context chain, process / safety / control shorthand |
| 0827 | `WAS` | English word 'was', world + AS=autism spectrum, weight + AS=active state, world-action-state chain, weight / agent / safety shorthand, state/safety/source suffix |
| 0828 | `YTC` | YT=YouTube + context flag, YT=why target + control marker, yes + TC=task class, why + TC=truth constraint, yes-target-context chain, why / truth / control shorthand |
| 0829 | `CSC` | CS=case + context flag, CS=context state + control marker, context + SC=scope, control + SC=self-control, context-state-context chain, control / safety / control shorthand |
| 0830 | `DSP` | DS=data source + prompt flag, DS=decision state + process marker, data + SP=system prompt, decision + SP=special, data-state-prompt chain, decision / safety / process shorthand |
| 0831 | `BUS` | English word 'bus', bot + US=user, boundary + US=United States, bot-user-state chain, boundary / unknown / safety shorthand, state/safety/source suffix |
| 0832 | `JKP` | JK=joke + prompt flag, JK=judge/key + process marker, judge + KP=key prompt, job + KP=keep, judge-kindness-prompt chain, job / key / process shorthand |
| 0833 | `NOT` | English word 'not', NO=negation + target flag, NO=no + truth marker, name-output-target chain, no / object / truth shorthand, target/task/trace suffix |
| 0834 | `YTM` | YT=YouTube + module flag, YT=why target + mode marker, yes + TM=trademark, why + TM=tone mode, yes-target-module chain, why / truth / mode shorthand |
| 0835 | `NVV` | NV=nearest valid + value flag, NV=nonviolent + veto marker, name + VV=veto/vote, no + VV=version/vector, name-value-value chain, no / veto / veto shorthand |
| 0836 | `WSR` | WS=workspace + role flag, WS=warning signal + rule marker, world + SR=source, weight + SR=safety route, world-state-role chain, weight / safety / rule shorthand |
| 0837 | `PSP` | PS=prompt state + prompt flag, PS=public safety + process marker, prompt + SP=system prompt, process + SP=special, prompt-state-prompt chain, process / safety / process shorthand |
| 0838 | `ZTC` | ZT=zero target + context flag, ZT=final token + control marker, zero + TC=task class, final state + TC=truth constraint, zero-target-context chain, final state / truth / control shorthand |
| 0839 | `CSP` | CS=case + prompt flag, CS=context state + process marker, context + SP=system prompt, control + SP=special, context-state-prompt chain, control / safety / process shorthand |
| 0840 | `NOD` | English word 'nod', NO=negation + data flag, NO=no + decision marker, name-output-data chain, no / object / decision shorthand, data/decision/depth suffix |
| 0841 | `TCM` | TC=task class + module flag, TC=truth constraint + mode marker, target + CM=command, truth + CM=context map, target-context-module chain, truth / control / mode shorthand |
| 0842 | `CTK` | CT=context + kindness flag, CT=control + key marker, context-target-kindness chain, control / truth / key shorthand, key/kernel/kindness suffix |
| 0843 | `CFL` | CF=conflict + law flag, CF=configuration + logic marker, context + FL=flow, control + FL=file layer, context-function-law chain, control / filter / logic shorthand |
| 0844 | `YTP` | YT=YouTube + prompt flag, YT=why target + process marker, yes + TP=target prompt, why + TP=true positive, yes-target-prompt chain, why / truth / process shorthand |
| 0845 | `CFE` | CF=conflict + entity flag, CF=configuration + emotion marker, context + FE=feeling, control + FE=feature, context-function-entity chain, control / filter / emotion shorthand |
| 0846 | `ZTM` | ZT=zero target + module flag, ZT=final token + mode marker, zero + TM=trademark, final state + TM=tone mode, zero-target-module chain, final state / truth / mode shorthand |
| 0847 | `JGL` | JG=judging + law flag, JG=judge gate + logic marker, judge + GL=gloss, job + GL=global, judge-goal-law chain, job / guard / logic shorthand |
| 0848 | `MTS` | MT=metric + state flag, MT=meta + safety marker, module-target-state chain, mode / truth / safety shorthand, state/safety/source suffix |
| 0849 | `DSW` | DS=data source + world flag, DS=decision state + weight marker, data + SW=software, decision + SW=switch, data-state-world chain, decision / safety / weight shorthand |
| 0850 | `MTT` | MT=metric + target flag, MT=meta + truth marker, module-target-target chain, mode / truth / truth shorthand, target/task/trace suffix |
| 0851 | `PRK` | PR=prompt + kindness flag, PR=process + key marker, prompt-role-kindness chain, process / rule / key shorthand, key/kernel/kindness suffix |
| 0852 | `MDD` | MD=markdown + data flag, MD=medical + decision marker, module-data-data chain, mode / decision / decision shorthand, data/decision/depth suffix |
| 0853 | `MDX` | MD=markdown + unknown flag, MD=medical + external marker, module-data-unknown chain, mode / decision / external shorthand, unknown or experimental placeholder |
| 0854 | `PSW` | PS=prompt state + world flag, PS=public safety + weight marker, prompt + SW=software, process + SW=switch, prompt-state-world chain, process / safety / weight shorthand |
| 0855 | `MTX` | MT=metric + unknown flag, MT=meta + external marker, module-target-unknown chain, mode / truth / external shorthand, unknown or experimental placeholder |
| 0856 | `STB` | ST=state + bot flag, ST=status + boundary marker, state-target-bot chain, safety / truth / boundary shorthand |
| 0857 | `ZTP` | ZT=zero target + prompt flag, ZT=final token + process marker, zero + TP=target prompt, final state + TP=true positive, zero-target-prompt chain, final state / truth / process shorthand |
| 0858 | `CSW` | CS=case + world flag, CS=context state + weight marker, context + SW=software, control + SW=switch, context-state-world chain, control / safety / weight shorthand |
| 0859 | `MSS` | MS=model state + state flag, MS=memory store + safety marker, module-state-state chain, mode / safety / safety shorthand, state/safety/source suffix |
| 0860 | `STH` | ST=state + human flag, ST=status + heart marker, state-target-human chain, safety / truth / heart shorthand |
| 0861 | `YTL` | YT=YouTube + law flag, YT=why target + logic marker, yes + TL=token limit, why + TL=timeline, yes-target-law chain, why / truth / logic shorthand |
| 0862 | `RET` | RE=repair + target flag, RE=response + truth marker, role-entity-target chain, rule / emotion / truth shorthand, target/task/trace suffix |
| 0863 | `UNO` | UN=undefined + output flag, UN=unknown + object marker, user + NO=negation, unknown + NO=no, user-name-output chain, unknown / no / object shorthand |
| 0864 | `RCK` | RC=recall + kindness flag, RC=record + key marker, role-context-kindness chain, rule / control / key shorthand, key/kernel/kindness suffix |
| 0865 | `STI` | ST=state + intent flag, ST=status + input marker, state-target-intent chain, safety / truth / input shorthand |
| 0866 | `TPM` | TP=target prompt + module flag, TP=true positive + mode marker, target + PM=prompt module, truth + PM=project manager, target-prompt-module chain, truth / process / mode shorthand |
| 0867 | `NET` | English word 'net', NE=nearest + target flag, NE=negative + truth marker, name-entity-target chain, no / emotion / truth shorthand, target/task/trace suffix |
| 0868 | `RER` | RE=repair + role flag, RE=response + rule marker, role-entity-role chain, rule / emotion / rule shorthand, route/risk/repair suffix |
| 0869 | `TDM` | TD=task drift + module flag, TD=temporal difference + mode marker, target + DM=direct message, truth + DM=decision matrix, target-data-module chain, truth / decision / mode shorthand |
| 0870 | `JKN` | JK=joke + name flag, JK=judge/key + no marker, judge + KN=known, job + KN=kindness/niceness, judge-kindness-name chain, job / key / no shorthand |
| 0871 | `FAT` | English word 'fat', FA=false + target flag, FA=fallback + truth marker, function-action-target chain, filter / agent / truth shorthand, target/task/trace suffix |
| 0872 | `MOS` | MO=mode + state flag, MO=moral + safety marker, module-output-state chain, mode / object / safety shorthand, state/safety/source suffix |
| 0873 | `QCM` | QC=quality control + module flag, QC=question context + mode marker, question + CM=command, query + CM=context map, question-context-module chain, query / control / mode shorthand |
| 0874 | `DRM` | DR=drift + module flag, DR=doctor + mode marker, data-role-module chain, decision / rule / mode shorthand, mode/model/module suffix |
| 0875 | `FAR` | English word 'far', FA=false + role flag, FA=fallback + rule marker, function-action-role chain, filter / agent / rule shorthand, route/risk/repair suffix |
| 0876 | `MOT` | MO=mode + target flag, MO=moral + truth marker, module-output-target chain, mode / object / truth shorthand, target/task/trace suffix |
| 0877 | `MSX` | MS=model state + unknown flag, MS=memory store + external marker, module-state-unknown chain, mode / safety / external shorthand, unknown or experimental placeholder |
| 0878 | `RDK` | RD=read depth + kindness flag, RD=runtime depth + key marker, role-data-kindness chain, rule / decision / key shorthand, key/kernel/kindness suffix |
| 0879 | `STU` | ST=state + user flag, ST=status + unknown marker, state-target-user chain, safety / truth / unknown shorthand |
| 0880 | `TRM` | TR=truth + module flag, TR=trace + mode marker, target-role-module chain, truth / rule / mode shorthand, mode/model/module suffix |
| 0881 | `UNA` | UN=undefined + action flag, UN=unknown + agent marker, user + NA=not applicable, unknown + NA=name, user-name-action chain, unknown / no / agent shorthand |
| 0882 | `CFW` | CF=conflict + world flag, CF=configuration + weight marker, context + FW=forward, control + FW=framework, context-function-world chain, control / filter / weight shorthand |
| 0883 | `DRP` | DR=drift + prompt flag, DR=doctor + process marker, data-role-prompt chain, decision / rule / process shorthand |
| 0884 | `FOX` | English word 'fox', FO=foe + unknown flag, FO=form + external marker, function-output-unknown chain, filter / object / external shorthand, unknown or experimental placeholder |
| 0885 | `ZTL` | ZT=zero target + law flag, ZT=final token + logic marker, zero + TL=token limit, final state + TL=timeline, zero-target-law chain, final state / truth / logic shorthand |
| 0886 | `HIM` | English word 'him', human + IM=image, heart + IM=immediate, human-intent-module chain, heart / input / mode shorthand, mode/model/module suffix |
| 0887 | `QDM` | QD=query depth + module flag, QD=question directive + mode marker, question + DM=direct message, query + DM=decision matrix, question-data-module chain, query / decision / mode shorthand |
| 0888 | `STO` | ST=state + output flag, ST=status + object marker, state-target-output chain, safety / truth / object shorthand |
| 0889 | `TRP` | TR=truth + prompt flag, TR=trace + process marker, target-role-prompt chain, truth / rule / process shorthand |
| 0890 | `UNV` | UN=undefined + value flag, UN=unknown + veto marker, user + NV=nearest valid, unknown + NV=nonviolent, user-name-value chain, unknown / no / veto shorthand |
| 0891 | `TCL` | TC=task class + law flag, TC=truth constraint + logic marker, target + CL=class, truth + CL=clarity, target-context-law chain, truth / control / logic shorthand |
| 0892 | `JKL` | JK=joke + law flag, JK=judge/key + logic marker, judge + KL=kill, job + KL=key layer, judge-kindness-law chain, job / key / logic shorthand |
| 0893 | `LWS` | LW=law + state flag, LW=low weight + safety marker, law + WS=workspace, logic + WS=warning signal, law-world-state chain, logic / weight / safety shorthand |
| 0894 | `MOX` | MO=mode + unknown flag, MO=moral + external marker, module-output-unknown chain, mode / object / external shorthand, unknown or experimental placeholder |
| 0895 | `STN` | ST=state + name flag, ST=status + no marker, state-target-name chain, safety / truth / no shorthand |
| 0896 | `DRB` | DR=drift + bot flag, DR=doctor + boundary marker, data-role-bot chain, decision / rule / boundary shorthand |
| 0897 | `TCF` | TC=task class + function flag, TC=truth constraint + filter marker, target + CF=conflict, truth + CF=configuration, target-context-function chain, truth / control / filter shorthand |
| 0898 | `LWT` | LW=law + target flag, LW=low weight + truth marker, law + WT=weight, logic + WT=what, law-world-target chain, logic / weight / truth shorthand |
| 0899 | `TRB` | TR=truth + bot flag, TR=trace + boundary marker, target-role-bot chain, truth / rule / boundary shorthand |
| 0900 | `DTC` | DT=data + context flag, DT=decision tree + control marker, data + TC=task class, decision + TC=truth constraint, data-target-context chain, decision / truth / control shorthand |
| 0901 | `DRH` | DR=drift + human flag, DR=doctor + heart marker, data-role-human chain, decision / rule / heart shorthand |
| 0902 | `KID` | English word 'kid', kindness + ID=identity, key + ID=identifier, kindness-intent-data chain, key / input / decision shorthand, data/decision/depth suffix |
| 0903 | `LWR` | LW=law + role flag, LW=low weight + rule marker, law + WR=write, logic + WR=warning route, law-world-role chain, logic / weight / rule shorthand |
| 0904 | `STF` | ST=state + function flag, ST=status + filter marker, state-target-function chain, safety / truth / filter shorthand |
| 0905 | `TIP` | English word 'tip', target + IP=internet protocol, truth + IP=intellectual property, target-intent-prompt chain, truth / input / process shorthand |
| 0906 | `TRH` | TR=truth + human flag, TR=trace + heart marker, target-role-human chain, truth / rule / heart shorthand |
| 0907 | `SIN` | English word 'sin', state + IN=input, safety + IN=instruction, state-intent-name chain, safety / input / no shorthand |
| 0908 | `DRI` | DR=drift + intent flag, DR=doctor + input marker, data-role-intent chain, decision / rule / input shorthand |
| 0909 | `TPU` | TP=target prompt + user flag, TP=true positive + unknown marker, target + PU=pickup, truth + PU=public/user, target-prompt-user chain, truth / process / unknown shorthand |
| 0910 | `TRI` | TR=truth + intent flag, TR=trace + input marker, target-role-intent chain, truth / rule / input shorthand |
| 0911 | `PTC` | PT=prompt token + context flag, PT=passage/truth + control marker, prompt + TC=task class, process + TC=truth constraint, prompt-target-context chain, process / truth / control shorthand |
| 0912 | `DRA` | DR=drift + action flag, DR=doctor + agent marker, data-role-action chain, decision / rule / agent shorthand |
| 0913 | `RTB` | RT=runtime + bot flag, RT=real-time + boundary marker, role-target-bot chain, rule / truth / boundary shorthand |
| 0914 | `DTM` | DT=data + module flag, DT=decision tree + mode marker, data + TM=trademark, decision + TM=tone mode, data-target-module chain, decision / truth / mode shorthand |
| 0915 | `TRA` | TR=truth + action flag, TR=trace + agent marker, target-role-action chain, truth / rule / agent shorthand |
| 0916 | `DRU` | DR=drift + user flag, DR=doctor + unknown marker, data-role-user chain, decision / rule / unknown shorthand |
| 0917 | `RTH` | RT=runtime + human flag, RT=real-time + heart marker, role-target-human chain, rule / truth / heart shorthand |
| 0918 | `UNE` | UN=undefined + entity flag, UN=unknown + emotion marker, user + NE=nearest, unknown + NE=negative, user-name-entity chain, unknown / no / emotion shorthand |
| 0919 | `GDS` | GD=good + state flag, GD=guard + safety marker, goal + DS=data source, guard + DS=decision state, goal-data-state chain, guard / decision / safety shorthand |
| 0920 | `STV` | ST=state + value flag, ST=status + veto marker, state-target-value chain, safety / truth / veto shorthand |
| 0921 | `TRU` | TR=truth + user flag, TR=trace + unknown marker, target-role-user chain, truth / rule / unknown shorthand |
| 0922 | `DRO` | DR=drift + output flag, DR=doctor + object marker, data-role-output chain, decision / rule / object shorthand |
| 0923 | `RTI` | RT=runtime + intent flag, RT=real-time + input marker, role-target-intent chain, rule / truth / input shorthand |
| 0924 | `PTM` | PT=prompt token + module flag, PT=passage/truth + mode marker, prompt + TM=trademark, process + TM=tone mode, prompt-target-module chain, process / truth / mode shorthand |
| 0925 | `CLC` | CL=class + context flag, CL=clarity + control marker, context + LC=law/code, control + LC=local context, context-law-context chain, control / logic / control shorthand |
| 0926 | `GDT` | GD=good + target flag, GD=guard + truth marker, goal + DT=data, guard + DT=decision tree, goal-data-target chain, guard / decision / truth shorthand |
| 0927 | `STE` | ST=state + entity flag, ST=status + emotion marker, state-target-entity chain, safety / truth / emotion shorthand |
| 0928 | `TRO` | TR=truth + output flag, TR=trace + object marker, target-role-output chain, truth / rule / object shorthand |
| 0929 | `DRN` | DR=drift + name flag, DR=doctor + no marker, data-role-name chain, decision / rule / no shorthand |
| 0930 | `MLS` | ML=model + state flag, ML=machine learning + safety marker, module-law-state chain, mode / logic / safety shorthand, state/safety/source suffix |
| 0931 | `RTA` | RT=runtime + action flag, RT=real-time + agent marker, role-target-action chain, rule / truth / agent shorthand |
| 0932 | `DTP` | DT=data + prompt flag, DT=decision tree + process marker, data + TP=target prompt, decision + TP=true positive, data-target-prompt chain, decision / truth / process shorthand |
| 0933 | `QCL` | QC=quality control + law flag, QC=question context + logic marker, question + CL=class, query + CL=clarity, question-context-law chain, query / control / logic shorthand |
| 0934 | `SST` | state + ST=state, safety + ST=status, state-state-target chain, safety / safety / truth shorthand, target/task/trace suffix |
| 0935 | `STW` | ST=state + world flag, ST=status + weight marker, state-target-world chain, safety / truth / weight shorthand |
| 0936 | `TRN` | TR=truth + name flag, TR=trace + no marker, target-role-name chain, truth / rule / no shorthand |
| 0937 | `DRL` | DR=drift + law flag, DR=doctor + logic marker, data-role-law chain, decision / rule / logic shorthand |
| 0938 | `MDK` | MD=markdown + kindness flag, MD=medical + key marker, module-data-kindness chain, mode / decision / key shorthand, key/kernel/kindness suffix |
| 0939 | `RTU` | RT=runtime + user flag, RT=real-time + unknown marker, role-target-user chain, rule / truth / unknown shorthand |
| 0940 | `MTK` | MT=metric + kindness flag, MT=meta + key marker, module-target-kindness chain, mode / truth / key shorthand, key/kernel/kindness suffix |
| 0941 | `QCF` | QC=quality control + function flag, QC=question context + filter marker, question + CF=conflict, query + CF=configuration, question-context-function chain, query / control / filter shorthand |
| 0942 | `STQ` | ST=state + question flag, ST=status + query marker, state-target-question chain, safety / truth / query shorthand |
| 0943 | `TRL` | TR=truth + law flag, TR=trace + logic marker, target-role-law chain, truth / rule / logic shorthand |
| 0944 | `TST` | target + ST=state, truth + ST=status, target-state-target chain, truth / safety / truth shorthand, target/task/trace suffix |
| 0945 | `DRF` | DR=drift + function flag, DR=doctor + filter marker, data-role-function chain, decision / rule / filter shorthand |
| 0946 | `RTO` | RT=runtime + output flag, RT=real-time + object marker, role-target-output chain, rule / truth / object shorthand |
| 0947 | `USE` | English word 'use', US=user + entity flag, US=United States + emotion marker, user-state-entity chain, unknown / safety / emotion shorthand |
| 0948 | `BDD` | BD=boundary + data flag, BD=body + decision marker, bot-data-data chain, boundary / decision / decision shorthand, data/decision/depth suffix |
| 0949 | `BDX` | BD=boundary + unknown flag, BD=body + external marker, bot-data-unknown chain, boundary / decision / external shorthand, unknown or experimental placeholder |
| 0950 | `PTP` | PT=prompt token + prompt flag, PT=passage/truth + process marker, prompt + TP=target prompt, process + TP=true positive, prompt-target-prompt chain, process / truth / process shorthand |
| 0951 | `STJ` | ST=state + judge flag, ST=status + job marker, state-target-judge chain, safety / truth / job shorthand |
| 0952 | `TRF` | TR=truth + function flag, TR=trace + filter marker, target-role-function chain, truth / rule / filter shorthand |
| 0953 | `BIN` | English word 'bin', bot + IN=input, boundary + IN=instruction, bot-intent-name chain, boundary / input / no shorthand |
| 0954 | `MLD` | ML=model + data flag, ML=machine learning + decision marker, module-law-data chain, mode / logic / decision shorthand, data/decision/depth suffix |
| 0955 | `MLX` | ML=model + unknown flag, ML=machine learning + external marker, module-law-unknown chain, mode / logic / external shorthand, unknown or experimental placeholder |
| 0956 | `RTN` | RT=runtime + name flag, RT=real-time + no marker, role-target-name chain, rule / truth / no shorthand |
| 0957 | `CTB` | CT=context + bot flag, CT=control + boundary marker, context-target-bot chain, control / truth / boundary shorthand |
| 0958 | `LCM` | LC=law/code + module flag, LC=local context + mode marker, law + CM=command, logic + CM=context map, law-context-module chain, logic / control / mode shorthand |
| 0959 | `TRG` | TR=truth + goal flag, TR=trace + guard marker, target-role-goal chain, truth / rule / guard shorthand |
| 0960 | `GCS` | GC=garbage collection + state flag, GC=guard core + safety marker, goal + CS=case, guard + CS=context state, goal-context-state chain, guard / control / safety shorthand |
| 0961 | `PRP` | PR=prompt + prompt flag, PR=process + process marker, prompt-role-prompt chain, process / rule / process shorthand |
| 0962 | `TDV` | TD=task drift + value flag, TD=temporal difference + veto marker, target + DV=developer, truth + DV=deviation, target-data-value chain, truth / decision / veto shorthand |
| 0963 | `CTH` | CT=context + human flag, CT=control + heart marker, context-target-human chain, control / truth / heart shorthand |
| 0964 | `STY` | ST=state + yes flag, ST=status + why marker, state-target-yes chain, safety / truth / why shorthand |
| 0965 | `POP` | English word 'pop', prompt + OP=output, process + OP=operation, prompt-output-prompt chain, process / object / process shorthand |
| 0966 | `DRV` | DR=drift + value flag, DR=doctor + veto marker, data-role-value chain, decision / rule / veto shorthand |
| 0967 | `DTL` | DT=data + law flag, DT=decision tree + logic marker, data + TL=token limit, decision + TL=timeline, data-target-law chain, decision / truth / logic shorthand |
| 0968 | `REK` | RE=repair + kindness flag, RE=response + key marker, role-entity-kindness chain, rule / emotion / key shorthand, key/kernel/kindness suffix |
| 0969 | `RTF` | RT=runtime + function flag, RT=real-time + filter marker, role-target-function chain, rule / truth / filter shorthand |
| 0970 | `BRR` | BR=boundary route + role flag, BR=break + rule marker, bot-role-role chain, boundary / rule / rule shorthand, route/risk/repair suffix |
| 0971 | `CTI` | CT=context + intent flag, CT=control + input marker, context-target-intent chain, control / truth / input shorthand |
| 0972 | `MSK` | MS=model state + kindness flag, MS=memory store + key marker, module-state-kindness chain, mode / safety / key shorthand, key/kernel/kindness suffix |
| 0973 | `STZ` | ST=state + zero flag, ST=status + final state marker, state-target-zero chain, safety / truth / final state shorthand |
| 0974 | `TRV` | TR=truth + value flag, TR=trace + veto marker, target-role-value chain, truth / rule / veto shorthand |
| 0975 | `COP` | English word 'cop', context + OP=output, control + OP=operation, context-output-prompt chain, control / object / process shorthand |
| 0976 | `VTD` | VT=veto + data flag, VT=validation target + decision marker, value + TD=task drift, veto + TD=temporal difference, value-target-data chain, veto / truth / decision shorthand |
| 0977 | `GCR` | GC=garbage collection + role flag, GC=guard core + rule marker, goal + CR=constraint route, guard + CR=credit, goal-context-role chain, guard / control / rule shorthand |
| 0978 | `PRB` | PR=prompt + bot flag, PR=process + boundary marker, prompt-role-bot chain, process / rule / boundary shorthand |
| 0979 | `RTG` | RT=runtime + goal flag, RT=real-time + guard marker, role-target-goal chain, rule / truth / guard shorthand |
| 0980 | `BRX` | BR=boundary route + unknown flag, BR=break + external marker, bot-role-unknown chain, boundary / rule / external shorthand, unknown or experimental placeholder |
| 0981 | `CTA` | CT=context + action flag, CT=control + agent marker, context-target-action chain, control / truth / agent shorthand |
| 0982 | `QDV` | QD=query depth + value flag, QD=question directive + veto marker, question + DV=developer, query + DV=deviation, question-data-value chain, query / decision / veto shorthand |
| 0983 | `DRW` | DR=drift + world flag, DR=doctor + weight marker, data-role-world chain, decision / rule / weight shorthand |
| 0984 | `GCD` | GC=garbage collection + data flag, GC=guard core + decision marker, goal + CD=code, guard + CD=clinical diagnosis, goal-context-data chain, guard / control / decision shorthand |
| 0985 | `PRH` | PR=prompt + human flag, PR=process + heart marker, prompt-role-human chain, process / rule / heart shorthand |
| 0986 | `PTL` | PT=prompt token + law flag, PT=passage/truth + logic marker, prompt + TL=token limit, process + TL=timeline, prompt-target-law chain, process / truth / logic shorthand |
| 0987 | `CTU` | CT=context + user flag, CT=control + unknown marker, context-target-user chain, control / truth / unknown shorthand |
| 0988 | `HSS` | HS=human signal + state flag, HS=harm signal + safety marker, human-state-state chain, heart / safety / safety shorthand, state/safety/source suffix |
| 0989 | `MOK` | MO=mode + kindness flag, MO=moral + key marker, module-output-kindness chain, mode / object / key shorthand, key/kernel/kindness suffix |
| 0990 | `RCP` | RC=recall + prompt flag, RC=record + process marker, role-context-prompt chain, rule / control / process shorthand |
| 0991 | `TRW` | TR=truth + world flag, TR=trace + weight marker, target-role-world chain, truth / rule / weight shorthand |
| 0992 | `WTD` | WT=weight + data flag, WT=what + decision marker, world + TD=task drift, weight + TD=temporal difference, world-target-data chain, weight / truth / decision shorthand |
| 0993 | `DRQ` | DR=drift + question flag, DR=doctor + query marker, data-role-question chain, decision / rule / query shorthand |
| 0994 | `PRI` | PR=prompt + intent flag, PR=process + input marker, prompt-role-intent chain, process / rule / input shorthand |
| 0995 | `RSM` | RS=response + module flag, RS=risk state + mode marker, role-state-module chain, rule / safety / mode shorthand, mode/model/module suffix |
| 0996 | `RTV` | RT=runtime + value flag, RT=real-time + veto marker, role-target-value chain, rule / truth / veto shorthand |
| 0997 | `TTR` | target + TR=truth, truth + TR=trace, target-target-role chain, truth / truth / rule shorthand, route/risk/repair suffix |
| 0998 | `CTO` | CT=context + output flag, CT=control + object marker, context-target-output chain, control / truth / object shorthand |
| 0999 | `RCC` | RC=recall + context flag, RC=record + control marker, role-context-context chain, rule / control / control shorthand |
| 1000 | `TRQ` | TR=truth + question flag, TR=trace + query marker, target-role-question chain, truth / rule / query shorthand |

## Use

```text
If a 3-letter group is undefined:
  treat as symbol only
  no authority
  no execution
  define before use

If a 3-letter group is local:
  bind local meaning
  block common wrong meanings
```