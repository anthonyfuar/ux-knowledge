# Answering a product-ethics question

## Use when
- Asked whether to build / ship feature, mechanic / product practice.
- 5 steps, in order: classify gate → apply tests → ground answer in humane principles → bring evidence + precedent → attribute correctly.
- If question needs more than answer → how-deep-to-go.md decides standard review vs full treatment.
- If feature heads to launch → run ../ethics/ethics-review-workflow.md steps.
- If principles conflict → ranking in core-stance.md: rights over time + effort, over delight.

## Step 1. Classify the gate
|Gate|Question|Ethical dilemma?|
|---|---|---|
|Able|can we build it?|no|
|Allowed|may we build it?|no; legality not ceiling; allowed does not settle whether to do it|
|Should|ought we build it?|yes; only gate = actual ethical dilemma|

- Method: ../methods/three-gate-check.md.

## Step 2. Apply the tests
|Test|Ask|Set out in|
|---|---|---|
|If-they-knew|how would person feel seeing exactly what design does to them? would they choose it?|../patterns/transparency-and-honesty.md, ../methods/stakeholder-arguments.md|
|Reciprocity|would you accept design used on own parent / child?|../patterns/transparency-and-honesty.md, ../methods/stakeholder-arguments.md|
|Persuasion vs manipulation|(1) whose goal does influence serve? (2) would person endorse it if understood?|closing test of ../ethics/deceptive-patterns.md; lever-by-lever version: ../ethics/influence-vs-manipulation.md|
|Purpose consistency|does mechanic contradict product's stated purpose?|../patterns/transparency-and-honesty.md|

- Purpose consistency: set mechanic against product's stated purpose; contradiction = finding itself.
- State purpose contradiction as finding → shape: write-a-finding.md.
- Hypothetical: team calendar tool sold as meeting-overload cure invites whole department to every new meeting by default → mechanic contradicts purpose → finding.
- Hypothetical: school reading program meant to build love of reading posts public leaderboard ranking classmates by pages read → contradiction → finding.

## Step 3. Ground the answer in humane principles
- Name each humane-design principle decision implicates; use its definition + review questions.
- Seven principles, own file each: ../principles/respectful.md, ../principles/finite.md, ../principles/empowering.md, ../principles/intentional.md, ../principles/inclusive.md, ../principles/resilient.md, ../principles/transparent.md; [principles index](../principles/index.md) shows them together.
- Each principle file: review questions in `Audit questions` section.
- Each principle used → also check its neighbours (its 'also check' set, see [principles index](../principles/index.md)).
- Psychological lever each principle guards → laws-and-principles-crosswalk.md.

## Step 4. Bring evidence + precedent
Pull comparable historical cases + research findings from evidence files.

|Question touches|Precedent / research in|
|---|---|
|Routing apps|../evidence/unintended-consequences.md (cities + societies)|
|Item trackers|../evidence/safety-and-abuse.md|
|Engagement-ranked feeds|../evidence/filter-bubbles-and-polarization.md, ../evidence/addiction-and-variable-rewards.md|
|Subscription cancellation|../evidence/business-cost-of-deception.md|
|Defaults|../evidence/decision-fatigue-and-choice.md|
|Attention + distraction|../evidence/attention-and-distraction.md|
|Children + adolescents|../evidence/children-and-adolescents.md|
|Personalization + surveillance|../evidence/personalization-and-surveillance.md|
|Convenience + friction|../evidence/convenience-and-friction.md|
|Inclusion + exclusion cost|../evidence/inclusion-and-exclusion-costs.md|

- Respect caveats on each finding / case → ../evidence/citation-caveats.md.

## Step 5. Attribute correctly
- If answer names concept (e.g. calm technology, deceptive patterns, computers extending human thinking, futures wheel, premortem) → check reference files before stating it.

|To check|Look in|
|---|---|
|Thinker behind idea|../lookup/humane-design-ideas.md|
|Book / foundational work|../lookup/timeline.md|
|Organization|../lookup/organizations-and-toolkits.md|
|Glossary term|../lookup/glossary.md (alphabetical)|

## Related
- core-stance.md: conflict ranking, rights over time + effort, over delight.
- how-deep-to-go.md: when question needs standard review / full treatment, not only answer.
- ../ethics/ethics-review-workflow.md: steps for ethics review of feature before launch.
- ../ethics/using-psychology-responsibly.md: guardrails for every psychological lever.
- ../ethics/anti-patterns-and-humane-alternatives.md: what to ship instead of common harmful patterns.
- write-a-finding.md: shape for stating purpose contradiction as finding.
- defend-a-decision.md: usability-side rationale, law, origin year, mechanism, evidence, metric.
- laws-and-principles-crosswalk.md: psychological lever each humane principle guards.
- ../methods/three-gate-check.md: step 1's three gates.
- ../ethics/influence-vs-manipulation.md: lever-by-lever persuasion test.
- ../ethics/deceptive-patterns.md: taxonomy, closes w/ persuasion-vs-manipulation test.
- [Principles index](../principles/index.md): seven principles side by side.
