# Mental Model

## In one line
Mental model = compressed internal model person uses to predict system's behavior; people act on it. Formal form: person's beliefs about system's workings + nature, held in head in condensed form. Use when: interface must match how people already believe system works; diagnosing mistaken expectations or redesign discordance; planning research to close gap between designers' + users' models; checking if Mental Model = right construct to cite.
- Class: construct. Aliases: none. Closely tied to Jakob's Law.
- Theme: Expectations. Matters most for: domain-wide conventions (Hypothetical: where patient portals put appointments + test results); model-aligning research; managing discordance after redesign.
- Core rules: design to users' mental models, not team's; narrow designer-user model mismatch w/ empathy maps, interviews, journey maps + personas.

## Applies when / does not apply when
|Situation|What model does|Do|
|---|---|---|
|system resembles one people know|people meet it w/ working model built for known one|match known one|
|design fits model users already hold|no learning phase first; knowledge from elsewhere carries across|keep to domain conventions|
|design does not fit|person must relearn|change system or improve model|
|team reasoning about "what users think"|model = user's belief, not truth|research it; never assume|
|users cannot tell you their model|models mostly unconscious → rarely stated; surface as mistaken expectations|watch for mistaken expectations|
|UI hides decision-relevant property (real distance, state, consequence)|users act on simplified map + make errors|show property|
|model gap observed today|models change w/ experience of your system + other systems → mismatch may resolve or may worsen|—|
|any model or interface representation|useful reduction, never reality itself|—|

## Decision rules

### Match the existing model
- Design to users' models, not team's. Never assume users' model matches team's; research to find out.
- If domain has settled conventions → follow them consistently. Hypothetical: clinic's patient portal puts appointments, test results + messages where other patient portals do, + each behaves there as patients already expect.
- Borrow known real-world affordances.
- Leverage existing models, not fight them, e.g. real-world metaphors for novices + children.

### Fix a mismatch: two remedies
1. Change system to fit prevailing model → move content to where people look for it; card sorting shows how people group information space.
2. Improve user's model → clearer labels + brief explanations of the few key concepts; teach early if UI cannot change.
- Sometimes best remedy = drop distinctions users will never grasp.

### Bridge the gulfs
- Remove intermediate steps between user's goal + its execution.
- Steps you cannot remove → keep visible + in sequence.
- Show system state immediately + in user's terms.
- Apply four bridging principles: visibility; good conceptual model; good mappings; feedback.

### Novel models + redesigns
- Introduce novel model only if clearly better: users rarely read explanations.
- Redesign → opt-in period + way to revert, avoiding mental-model discordance.
- Let users migrate to redesign when ready.

### Research the gap
- Align team's picture of product w/ users' via journey maps, interviews, empathy maps + personas; this mismatch ranks among design's toughest problems.
- Journey maps also give stakeholders + designers one shared experience model.
- Test copy + flows w/ real novices.
- Do not trust self-reported understanding (illusion of explanatory depth) → probe w/ tasks asking people to explain how it works.
- Preference tests: inferior but familiar design can win → separate preference from performance.

### Correct a wrong model
- Replace it w/ clear alternative explanation, not bare denial.
- Avoid restating myth (wrong model persists even after correction).

## Why it works

### Mechanism
- Mental model predicts + interprets new systems resembling known one. Interface fits model → fades from attention; does not fit → person must relearn.
- Continuous loop: model drives predictions + planned actions; outcomes update model.
- Designers hold rich, accurate models of own product; users hold thin ones → this gap = core usability problem.
- Mismatch between designer's conceptual model + user's model → opens gulf of execution + gulf of evaluation.
- People's models hold only selected concepts + relationships, not whole world.
- Strong inertia: well-worn patterns persist even when they no longer help.
- One misconception can distort whole session while its premise goes unquestioned.
- Novel models need clear advantage because users rarely read explanations.
- Online carts inherit physical-store rule: shopper alone decides what goes in cart.
- Model of Back = "return to the previous screen".
- Repeated exposure eases processing; this ease mistaken for liking (mere exposure), even when exposure not remembered.

### Terms
|Term|Meaning|
|---|---|
|Conceptual model|designer's side of match: coherent, consistent system image users can predict operations + results from|
|Gulf of execution|gap between what user intends + actions system makes available|
|Gulf of evaluation|effort to read system state + judge if goal met|
|Seven stages of action|forming goal; forming intention; specifying action; executing it; then perceiving, interpreting + evaluating world state|
|Four design principles|bridge both gulfs: visibility; good conceptual model (coherent, consistent system image); good mappings; feedback|
|Map-territory distinction ("the map is not the territory")|every model + every interface representation = useful reduction, never reality|
|Mere exposure|ease from repeated exposure mistaken for liking|
|Curse of knowledge|experts struggle to imagine not knowing what they know → team-written onboarding tends toward heavy jargon|
|Continued influence effect|wrong model persists even after correction|
|Illusion of explanatory depth|people's self-reported understanding of how something works inflated|

### Origin
- Origin = 1943 theoretical psychology book. Claim: reasoning, explaining + foreseeing events all run on miniature world replica held in head.
- Gulfs, seven stages of action + four design principles date to 1986 + 1988; gulfs first appeared in 1986 edited volume on user-centered system design.
- Classic usability heuristics published 1990, revised 1994.

## Evidence
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|People reason w/ small internal world models|1943 theoretical book|theory, not experiment|—|
|Familiar on-screen controls borrowed from hardware: toggle, button + radio input each imitate hand-worked physical-panel control|design-history observation|observation|borrow known real-world affordances|
|Making something simpler to use always adds complexity to its mechanism; better conceptual model can make something feel simpler w/o changing it; perceived complexity lives in user's conceptual model|2010 book|argued|better conceptual model can make product feel simpler|

## Product cases
|Case|What happened|Strength|Lesson|
|---|---|---|---|
|Luggage retailer|broke cart model by silently pre-adding $8.25 shipping-protection toggle, on by default|—|sneak into basket; paid extras off by default|
|Snapchat, early 2018|reworked layout put everyday features out of easy reach; users protested in large numbers; part of user base left for Instagram|public reaction, no metrics|sudden redesigns produce mental-model discordance|
|Google Calendar, Gmail + large video platform, 2017|after years of largely unchanged look, Material Design version came to desktop as opt-in, w/ way back, way to comment + time to try + get used to it|described outcome: discordance avoided|opt-in + way back + feedback + time|

## Misreadings and limits
- Wrong: familiar design's preference win = proof of its quality (Mental Model, Jakob's Law) → Right: mere exposure inflates liking; separate preference from performance.
- Wrong: assuming designers' models match users' → Right: research designer-user model gap.
- Wrong: correcting myth by denying + repeating it → Right: give clear alternative explanation; do not restate myth.
- Wrong: trusting users' self-reported understanding → Right: probe w/ explain-how-it-works tasks.
- Limit: every mental model = useful reduction, never reality itself.
- Limit: core-claim support = 1943 theoretical book, not experiment.

## Check questions
[A] = answerable from artifact itself; [P] = needs process/research evidence.
- [A] (Jakob's Law, Mental Model) Do standard patterns behave as elsewhere? Look for: carts, checkout + form controls reinvented w/o stated purpose; new windows; Back jumping up hierarchy; overlays Back cannot close.
- [P] (Mental Model) Design checked against users' models, not team's? Look for: assumptions about how users think w/ no research behind them.
- [P] (Mental Model) Assumptions tested w/ real novices, not team itself? Look for: designers as proxy users (curse of knowledge, false consensus); trust in users' self-reported understanding.
- [A] (Mental Model: preselection) Paid extras off by default? Look for: pre-checked insurance or protection add-ons.
- System state shown immediately + in user's terms?
- Does UI hide decision-relevant property (real distance, state, consequence)?

## Symptoms → fixes
|Symptom|Likely cause (laws)|Fix|
|---|---|---|
|Redesign triggers backlash|Jakob's Law, Mental Model|temporary opt-in w/ preview; feedback channel; way back|
|Team wants novel pattern users find slow|↑|deviate only if much better once learned, users stay long enough to learn it + scaffolding can support learning; compare learning curves, not first use|
|Users look in wrong place for content|system does not fit prevailing model|move content to where people look; card sorting|
|Users misuse concept; UI cannot change concept|thin user model|clearer labels; brief explanations of the few key concepts; teach early|
|Onboarding copy full of jargon|curse of knowledge|test copy + flows w/ real novices|
|Corrected misunderstanding recurs|continued influence effect|clear alternative explanation; do not restate myth|

## Hypothetical examples
- Hypothetical: gulf of execution → resident expects one tap on "Pay" to settle water bill, but city portal first demands account choice, payment date + confirmation code.
- Hypothetical: map vs territory (hidden consequence) → train-booking screen marks fare "flexible" but does not show each change carries fee; travellers book it believing changes free, then get charged.
- Hypothetical: Back sent up hierarchy → in grocery app, Back from product page returns to store's category home, not search results shopper came from.
- Hypothetical: overlay looking like page → online course opens each lesson in full-screen layer; pressing Back exits whole course instead of closing lesson.
- Hypothetical: split missing from user's model → tax portal keeps filed returns + saved drafts in separate sections; resident opens only default section, sees no draft + concludes saved return lost.
- Hypothetical: borrowing real-world model for novices → first-time online-banking app shows savings goals as labelled jars people move money between, since newcomers have no sub-account model yet.

## Humane bound
- Bounded by Transparent.
- Bounded by Intentional: no preselection where money or consent decided.
- Turned against people: trust carried by mental model can be used against its holder, e.g. cart inheriting store rule gets paid extras silently pre-added = sneak into basket.
- Further reading: deceptive-pattern taxonomy; defaults + choice architecture patterns; forms + data entry patterns (paid add-ons default off).

## Related
- ../principles/transparent.md: humane principle bounding it.
- ../principles/intentional.md: humane principle bounding it; no preselection where money or consent decided.
- ../ethics/deceptive-patterns.md: named deceptive patterns + honest alternatives, incl. silently pre-added paid extras.
- ../patterns/defaults-and-choice-architecture.md: humane bound on preselection (paid extras off by default, opt-in).
- ../patterns/forms-and-data-entry.md: paid add-ons default off.
- jakobs-law.md: closely tied via expectations carried over from other products; shares standard-patterns check + redesign-backlash and novel-pattern fixes.
- teslers-law.md: perceived complexity lives in mental model.
- paradox-of-the-active-user.md: linked via assimilation paradox.
- ../checklists/usability-heuristics-map.md: "Match between system and real world" → Mental Model + Jakob's Law; classic heuristics 1990, revised 1994.
- ../methods/convention-or-new-pattern.md: researching users' models before leaving convention; rolling out redesign w/ way back.
- ../guides/laws-and-principles-crosswalk.md: maps humane principle bounding it.
- ../patterns/departing-from-convention.md: applies it.
