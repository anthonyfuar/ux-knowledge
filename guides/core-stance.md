# Core stance and working rules

## Use when
- Read first, before any design / review / rationale / ethics task; every other guide assumes this stance.

## 1. How to hold the laws
- Fitting = product's job: shape it to regularities psychology charted in how people perceive, remember, attend + decide; person never asked to adjust.
- Design bends to people; people never made to fit product.
- Good looks = no protection: product cutting against those regularities can still fail.
- UX laws = heuristics to weigh; not formulas, never mandates.
- Law = hypothesis to verify w/ people; user research + project data always outrank any law.
- If research / analytics already answer question → follow data; law only explains it.
- Know why pattern works before copying it; law behind it = its why. Why explained via its law → shared, defensible rationale for stakeholders → defend-a-decision.md.
- Knowledge making product intuitive can also make it compulsive → check every persuasive lever against user's own goals (../ethics/influence-vs-manipulation.md).
- Principles outlast technology: new devices + AI change examples + constraints, not psychology.

Why psychology first: argument, not research finding.
- Argument: one extra skill non-negotiable for any designer = basic psychology, scoped to what people do at interfaces + how they engage w/ them.
- Argument: rank knowledge designer can add beyond craft itself by worth → psychology possibly first.
- Argument: business sense, programming + writing = recurring candidates for designer's extra skills; each pays off, though arguably none required.

## 2. Kinds of law: predictive models vs lenses
Three UX laws = predictive models; all others = lenses.

|Kind|Laws|What it gives|
|---|---|---|
|Predictive model, quantitative|../laws/fittss-law.md, ../laws/hicks-law.md|fitted equations|
|Predictive model, directional|../laws/jakobs-law.md|prediction: familiar design beats novel one on first use → test w/ learning curves (method dating to 1980 work)|
|Lens|every other UX law|lens for spotting risks, not predictive model|

Two UX-law families (../laws/index.md arranges both by theme across all 30):

|Family|Count|Members|Role|
|---|---|---|---|
|Cognitive constructs|7|../laws/chunking.md, ../laws/cognitive-bias.md, ../laws/cognitive-load.md, ../laws/flow.md, ../laws/mental-model.md, ../laws/selective-attention.md, ../laws/working-memory.md|explain behaviour|
|Named effects + principles|23|remaining UX laws|describe / predict behaviour|

- Constructs explain behaviour; named effects predict / prescribe it.

## 3. Ground design in real people
- Techniques: user interviews, contextual inquiry, usability tests, eye-tracking, journey maps, empathy maps, personas, design critiques (../methods/design-critique.md).

|Risk|Do|Why|
|---|---|---|
|Self-report bias|prefer behavioural data + anonymous formats over self-report|people over-report good + under-report bad behaviour|
|Researcher expectations|neutral scripts + blind analysis in usability tests|expectations shape both participants + interpretation|
|Survivorship bias|interview people having left product, not only active users|—|
|Overfitting|avoid over-tuning design to a few participants / loud feedback|—|
|Random variation|avoid reading patterns into random metric variation|→ 'superstitious' changes|
|Conjunction fallacy|prioritize by frequency data, not vivid persona stories|such stories feel more plausible than warranted|

- More counters to research + team biases → ../methods/debiasing.md.

## 4. People over metrics
- Core stance: people over metrics. Attention = scarce.
- Many products monetize personal data, harvest attention + exploit known weak spots in human psychology, when they could extend what people can do.
- Whoever ships product owns its effects. Artifact embodies values regardless of makers' motive.
- Misuse nobody imagined = design failure, not excuse.
- Humane design = people-over-metrics stance turned into framework people can review. Parts:

|Part|Files|
|---|---|
|7 named principles|[principles index](../principles/index.md)|
|Pattern + anti-pattern catalog|[pattern catalog](../patterns/index.md), [anti-patterns w/ humane alternatives](../ethics/anti-patterns-and-humane-alternatives.md), [deceptive-pattern taxonomy](../ethics/deceptive-patterns.md)|
|Audit checklists|../checklists/humane-design-audit.md, ../checklists/calm-technology-scorecard.md, ../checklists/interruption-decision-rules.md|
|Foresight methods|[methods index](../methods/index.md)|
|Metrics keeping growth honest|../methods/counter-metrics.md, ../methods/measure-what-you-value.md|
|Evidence backing recommendations, w/ rules for citing it + its caveats|../evidence/stating-evidence.md, ../evidence/citation-caveats.md|

- Humane-design principles = critique lens for any product decision.

## 5. Working rules
- Retire word "user" from team talk; say "people". State success as people's goals, not DAUs / conversions: vocabulary decides what counts as success.
- Choose smallest intervention giving choice back: off by default, visible end, confirmation, or label.
- Name pattern: shared label (e.g. roach motel, sneak into basket, bottomless bowl) turns vague discomfort into objection stakeholder can hear. Always pair name w/ its honest alternative; both in ../ethics/deceptive-patterns.md.
- Count people, not percentages: 1% of platform w/ two billion accounts = 20 million humans.
- Ask whether assumed future worth building.
- Capabilities shipped + capabilities on by default = team decision.
- Hardware keeps shrinking + gaining senses.
- Inevitability talk ('this is where things are going anyway') = argument to answer, not fact.

## 6. Resolving conflicts
- Satisfying one principle often quietly breaks another → check neighbours via each principle's 'also check' set ([principles index](../principles/index.md)).
- Ranking: (1) human rights (privacy, security, accessibility) → (2) people's time + effort → (3) delight, last.
- Order review findings + severities by same ranking; finding shape + severity levels → write-a-finding.md.

## 7. Which guide for which task
|Task|Open|
|---|---|
|Design new screen, component, flow, navigation, form, onboarding, search, menu, dashboard, CTA, loading / error state, or touch layout|design-a-screen-or-flow.md: steps bringing laws + humane principles into new design|
|Review / audit existing interface, prototype, screenshot / spec|review-an-interface.md: steps for combined usability + humane-design review|
|Diagnose why interface feels hard, slow, cluttered, confusing / forgettable|symptom-to-fix-index.md|
|Cut cognitive load, option counts / decision time|../methods/lightening-mental-effort.md, ../laws/hicks-law.md, ../laws/choice-overload.md|
|Write rationale, critique / stakeholder argument w/ years + study facts|defend-a-decision.md|
|Check whether persuasive pattern (progress, delay, emphasis) becomes manipulation|../ethics/influence-vs-manipulation.md|
|Any product decision via humane lens|depth → how-deep-to-go.md (quick pass, standard review, full treatment); acceptability questions → answer-an-ethics-question.md|

## 8. When this knowledge does not apply
|Situation|Do instead|
|---|---|
|Pure visual-brand, illustration / copy-tone question w/ no usability angle|usability laws not for it|
|Implementation question (CSS, frameworks, performance engineering) beyond response-time budget|usability laws not for it; budget itself → ../methods/thresholds-and-formulas.md|
|Product-ethics audit deeper than influence-vs-manipulation test|humane-design side: ../checklists/humane-design-audit.md, ../ethics/ethics-review-workflow.md|
|Research / analytics already answer question|follow data; law only explains it|
|Pure visual styling, copy polish / layout w/ no behavioural, data, attention / safety dimension|do not reach for humane-design principles|
|Legal-compliance-only question|lawyer's domain; this knowledge sets bar above compliance; legality = floor|
|Request to maximize engagement / conversion at any cost|humane principles not tool for this; use this knowledge to show request's cost (../evidence/business-cost-of-deception.md) + propose honest alternative (../ethics/anti-patterns-and-humane-alternatives.md)|
|Detailed accessibility conformance testing|not conformance-testing manual; this knowledge frames inclusion + points to WCAG's four principles (../principles/inclusive.md, ../patterns/inclusive-and-accessible-design.md)|

## Related
- design-a-screen-or-flow.md: steps bringing laws + humane principles into new design.
- review-an-interface.md: steps for combined usability + humane-design review.
- how-deep-to-go.md: quick pass vs standard review vs full treatment.
- common-mistakes.md: most damaging misuses, usability + humane sides.
- laws-and-principles-crosswalk.md: principle bounding each law + lever each principle guards.
- ../laws/index.md: all 30 UX laws by theme, w/ decision matrix + two families.
- [Principles index](../principles/index.md): seven humane-design principles side by side w/ neighbours.
- ../ethics/using-psychology-responsibly.md: guardrails for every psychological lever.
- ../methods/debiasing.md: counters to research + team biases.
- write-a-finding.md: finding shape + severity levels.
