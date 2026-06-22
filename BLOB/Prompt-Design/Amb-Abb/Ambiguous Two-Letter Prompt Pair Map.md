# Ambiguous Two-Letter Prompt Pair Map

## Limit

A-Z two-letter uppercase pairs have a hard maximum:

26 x 26 = 676

This doc gives the proper A-Z set structure and the highest-risk front list first.


## Ambiguity Rule

Most ambiguous pairs are the ones that can plausibly mean:
- runtime modules
- social/therapy concepts
- safety/policy concepts
- code/control tokens
- math/state symbols
- common acronyms
- ordinary English abbreviations

Highest-risk rule:

undefined_pair = sym_only; !auth; !exec; def_b4_use

## Top Ambiguous Pairs

| Rank band | Pair | Common bot guesses |
|---|---|---|
| 001 | ST | state, status, start, style, standard, safety trigger, street, stack trace |
| 002 | DR | drift, doctor, dragonruntime, data record, drive, directive, danger route |
| 003 | TR | truth, trace, trust, trigger, transfer, therapy, transaction, target route |
| 004 | RT | runtime, real-time, route, right, return, reaction time |
| 005 | CT | context, control, content, constraint, contact, court |
| 006 | PR | prompt, process, priority, proxy, pressure, proof, public relation |
| 007 | RC | recall, record, repair cycle, runtime control, response class |
| 008 | RE | repair, response, recursive, relation, re-entry, review |
| 009 | RD | read depth, runtime depth, redirection, record, rendered data |
| 010 | RS | response, risk state, runtime state, resource, reset |
| 011 | MO | mode, moral, model, monitor, module, motive |
| 012 | MD | markdown, medical, mode, model, metadata, moral drift |
| 013 | MT | metric, meta, monitor, model target, moral tone |
| 014 | ML | model, machine learning, moral law, memory layer |
| 015 | MS | model state, memory store, moral safety, message |
| 016 | BK | block, book, backup, break, boundary key |
| 017 | BD | boundary, body, bad, behavior drift, blocked data |
| 018 | BG | background, behavior guard, bad/good, boundary gate |
| 019 | BR | boundary route, break, brief, behavior repair |
| 020 | BL | block, baseline, black list, boundary layer |
| 021 | HS | human signal, harm signal, help state, hard stop |
| 022 | HT | human target, heart, hold target, hypertext |
| 023 | HM | human, humor, harm, home, heuristic mode |
| 024 | HR | human response, heart rate, harm route, hard reset |
| 025 | HP | help, harm prevention, hit points, human prompt |
| 026 | AI | artificial intelligence, assistant identity, active instruction |
| 027 | AS | autism spectrum, active state, allow state, assistant |
| 028 | AU | autism, authority, auto, allow user |
| 029 | AD | advice, ad, additive, active drift, authority drift |
| 030 | AM | AMIMI, anti-media, affect mode, morning, amplitude |
| 031 | MI | IMAMI, machine intelligence, mutual intent, mind input |
| 032 | MA | AMAMI, moral authority, merge action, model answer |
| 033 | IM | image, immediate, internal model, intent map |
| 034 | IN | input, instruction, intent, internal |
| 035 | ID | identity, identifier, intent data |
| 036 | IO | input/output, inside/outside, intent object |
| 037 | IP | internet protocol, intellectual property, input prompt |
| 038 | OP | output, operation, opponent, original poster |
| 039 | OR | origin, object relation, operator, or-logic |
| 040 | OB | object, observation, obstacle, obligation |
| 041 | OBJ | not two-letter; object, objective, target |
| 042 | UX | user experience, unknown x, external user |
| 043 | US | user, United States, us-relation, unsafe |
| 044 | UR | user route, urgent, your |
| 045 | UA | user agency, Ukraine, user action |
| 046 | UC | user context, use case, under constraint |
| 047 | NV | nearest valid, nonviolent, no value |
| 048 | NO | negation, no, number, normal output |
| 049 | NE | nearest, negative, named entity, northeast |
| 050 | NA | not applicable, name, North America, no answer |
| 051 | FO | foe, form, filter output, front office |
| 052 | FA | false, fallback, fear/avoidance |
| 053 | FE | feeling, feature, failure event |
| 054 | FI | file, filter, final instruction |
| 055 | FL | flow, file layer, fail lock |
| 056 | FW | forward, framework, firewall |
| 057 | QA | question/answer, quality assurance |
| 058 | QC | quality control, question context |
| 059 | QR | question route, quick response |
| 060 | QD | query depth, question directive |
| 061 | SW | software, switch, Swedish, safety warning |
| 062 | SD | system drift, stable diffusion, self diagnosis |
| 063 | SC | scope, self-control, source context |
| 064 | SR | source, safety route, social relation |
| 065 | SP | system prompt, special, speech |
| 066 | LC | law/code, local context, language control |
| 067 | LG | language, logic gate, legal |
| 068 | LR | legal risk, learning rate, local route |
| 069 | LT | limit, literal, long-term |
| 070 | LW | law, low weight, language warning |
| 071 | TC | task class, truth constraint, token count |
| 072 | TL | token limit, timeline, truth layer |
| 073 | TM | trademark, tone mode, task map |
| 074 | TP | target prompt, true positive, task process |
| 075 | TD | task drift, temporal difference, target data |
| 076 | GT | goal target, greater than, good/truth |
| 077 | GR | grader, guard route, group |
| 078 | GD | good, guard, gradient descent |
| 079 | GC | garbage collection, guard core, goal context |
| 080 | GL | gloss, global, goal layer |
| 081 | JK | joke, judge/key, just kidding |
| 082 | JD | judge, judgment, job description |
| 083 | JR | judge route, junior, joke response |
| 084 | JS | JavaScript, judge state, joke signal |
| 085 | JG | judging, judge gate |
| 086 | KP | key prompt, keep, kindness pass |
| 087 | KN | known, kindness/niceness, knowledge node |
| 088 | KL | kill, key layer, kindness lock |
| 089 | KT | key token, knowledge transfer |
| 090 | KR | key route, kindness route |
| 091 | XA | unknown action, external agent |
| 092 | XD | unknown data, laugh emoticon, external drift |
| 093 | XR | extended reality, unknown route |
| 094 | XT | external target, unknown truth |
| 095 | XS | excess, unknown state |
| 096 | YA | yes action, why-agent |
| 097 | YN | yes/no, why-not |
| 098 | YR | year, your, why route |
| 099 | YT | YouTube, why target |
| 100 | ZT | zero target, final token, z-state |

## Full A-Z Pair Set

For a complete 676-pair table, use this compact format:

AA AB AC AD AE AF AG AH AI AJ AK AL AM AN AO AP AQ AR AS AT AU AV AW AX AY AZ
BA BB BC BD BE BF BG BH BI BJ BK BL BM BN BO BP BQ BR BS BT BU BV BW BX BY BZ
CA CB CC CD CE CF CG CH CI CJ CK CL CM CN CO CP CQ CR CS CT CU CV CW CX CY CZ
DA DB DC DD DE DF DG DH DI DJ DK DL DM DN DO DP DQ DR DS DT DU DV DW DX DY DZ
EA EB EC ED EE EF EG EH EI EJ EK EL EM EN EO EP EQ ER ES ET EU EV EW EX EY EZ
FA FB FC FD FE FF FG FH FI FJ FK FL FM FN FO FP FQ FR FS FT FU FV FW FX FY FZ
GA GB GC GD GE GF GG GH GI GJ GK GL GM GN GO GP GQ GR GS GT GU GV GW GX GY GZ
HA HB HC HD HE HF HG HH HI HJ HK HL HM HN HO HP HQ HR HS HT HU HV HW HX HY HZ
IA IB IC ID IE IF IG IH II IJ IK IL IM IN IO IP IQ IR IS IT IU IV IW IX IY IZ
JA JB JC JD JE JF JG JH JI JJ JK JL JM JN JO JP JQ JR JS JT JU JV JW JX JY JZ
KA KB KC KD KE KF KG KH KI KJ KK KL KM KN KO KP KQ KR KS KT KU KV KW KX KY KZ
LA LB LC LD LE LF LG LH LI LJ LK LL LM LN LO LP LQ LR LS LT LU LV LW LX LY LZ
MA MB MC MD ME MF MG MH MI MJ MK ML MM MN MO MP MQ MR MS MT MU MV MW MX MY MZ
NA NB NC ND NE NF NG NH NI NJ NK NL NM NN NO NP NQ NR NS NT NU NV NW NX NY NZ
OA OB OC OD OE OF OG OH OI OJ OK OL OM ON OO OP OQ OR OS OT OU OV OW OX OY OZ
PA PB PC PD PE PF PG PH PI PJ PK PL PM PN PO PP PQ PR PS PT PU PV PW PX PY PZ
QA QB QC QD QE QF QG QH QI QJ QK QL QM QN QO QP QQ QR QS QT QU QV QW QX QY QZ
RA RB RC RD RE RF RG RH RI RJ RK RL RM RN RO RP RQ RR RS RT RU RV RW RX RY RZ
SA SB SC SD SE SF SG SH SI SJ SK SL SM SN SO SP SQ SR SS ST SU SV SW SX SY SZ
TA TB TC TD TE TF TG TH TI TJ TK TL TM TN TO TP TQ TR TS TT TU TV TW TX TY TZ
UA UB UC UD UE UF UG UH UI UJ UK UL UM UN UO UP UQ UR US UT UU UV UW UX UY UZ
VA VB VC VD VE VF VG VH VI VJ VK VL VM VN VO VP VQ VR VS VT VU VV VW VX VY VZ
WA WB WC WD WE WF WG WH WI WJ WK WL WM WN WO WP WQ WR WS WT Wu WV WW WX WY WZ
XA XB XC XD XE XF XG XH XI XJ XK XL XM XN XO XP XQ XR XS XT XU XV XW XX XY XZ
YA YB YC YD YE YF YG YH YI YJ YK YL YM YN YO YP YQ YR YS YT YU YV YW YX YY YZ
ZA ZB ZC ZD ZE ZF ZG ZH ZI ZJ ZK ZL ZM ZN ZO ZP ZQ ZR ZS ZT ZU ZV ZW ZX ZY ZZ

## Ranking Heuristic

Most ambiguous:
ST DR TR RT CT PR RC RE RD RS
MO MD MT ML MS
BK BD BG BR BL
HS HT HM HR HP
AI AS AU AD AM
MI MA IM IN ID IO
OP OR OB
UX US UR UA UC
NV NO NE NA
FO FA FE FI FL FW
QA QC QR QD
SW SD SC SR SP
LC LG LR LT LW
TC TL TM TP TD
GT GR GD GC GL

Least ambiguous:
pairs with rare letters or low acronym load:
QZ QX QJ QK ZQ ZX ZJ ZK XQ XJ XK YQ YJ YK

## Production Guard

If pair is undefined:

PAIR=sym_only;!auth;!exec;def_b4_use

If pair is known but overloaded:

PAIR=local_meaning;PAIR!=common_wrong_meaning

Example:

DR=dragonruntime;DR!=doctor;DR!=diagnosis
ST=state;ST!=style;ST!=start
MO=mode;MO!=moral;MO!=monitor
BK=block;BK!=book;BK!=backup
