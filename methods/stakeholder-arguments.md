# Stakeholder arguments

## Use when
- Defending usability decision or humane-design choice to stakeholders, clients or leadership.
- Two parts: usability arguments (why name law, 5-step argument, arguments that tend to land) · humane-design arguments (12-row set + caution on leaning on business case).

## Part 1: usability arguments

### Why name the law
- UX laws give shared, defensible rationale → helps win buy-in.
- Experienced designers apply laws by instinct; naming principle + year + prediction turns hunch into argument surviving client/stakeholder review.
- Caveat: "law" used loosely; UX laws = rules of thumb. Research + project data decide, not law itself.

### Five-step argument
1. **Observed problem**: behavior/metric showing problem. Hypothetical: many applicants in library-card sign-up quit at proof-of-address upload.
2. **Law + mechanism**: law's name + year first described; causal mechanism in one sentence.
3. **Evidence**: origin study (sample, condition, finding) + comparable product cases.
4. **Change**: exactly what will differ.
5. **Prediction + test**: expected metric shift + how research will confirm/refute it.
- In argument, law = hypothesis; data decides.

### Arguments that tend to land
|Argument|Law|Case to make|Caveat|
|---|---|---|---|
|Cost arithmetic|../laws/teslers-law.md|Build cost (single engineer-week) vs total user time lost (one minute apiece × one million people). Original audience pitched: outside software makers + Apple's management.||
|Response-time economics|(1982 paper)|Saved user time's value (seconds saved × interactions × users × hourly cost) vs infrastructure cost. Paper's worked illustration, under own assumptions, claimed up to 4.1 hours saved/user/day at 0.3 s vs 3.0 s response.|Label figures as vendor-authored estimates. Plan capacity when speeding up system: faster response raises total load.|
|Precedent|../laws/jakobs-law.md|Snapchat 2018 redesign backlash vs YouTube's 2017 opt-in redesign → cost of discordance.||
|Response-time standard|../laws/doherty-threshold.md|1982 IBM paper: productivity climbs steeply when response time below 1 s. 400 ms = widely used practitioner threshold from same paper.||
|Memory over averages|../laws/peak-end-rule.md|Cold-water + colonoscopy findings support investing in endings over uniform polish.||
|Prediction|../laws/hicks-law.md, ../laws/fittss-law.md|Fewer + clearer choices, bigger + closer targets → predictably take less time.||
|Where to invest|../laws/pareto-principle.md|Put effort where most users gain.||
|Alignment tools||Journey maps; stated reasons in critique (below).||
|Live stress test||Stress ideal version in front of stakeholders (below).||
|Counters to common objections|../laws/choice-overload.md|Familiarity, features, options (below).||

### Alignment tools + live stress test
- Journey maps → stakeholders + designers share one mental model of customer experience.
- In critique, no decision passes w/o its reason stated.
- Start each wireframe w/ two lists: user's goals for screen; every required element, down to privacy link + ads.
- Live stress test in review: ideal version first, then stress it in front of stakeholders: vary viewport width, raise default font size, paste long names + real outlier content. Reveals hidden design dimensions + prevents disappointing reveal after launch.

### Familiarity, feature + option objections
|Objection|Answer|
|---|---|
|"The web will get boring"|Value of familiarity.|
|"More features bring more satisfaction"|Choice overload + decision paralysis. One 2009 account: people, teams included, report wanting more choice + information than they can process, yet large option set can stop them choosing entirely.|
|"Users are asking for more options"|Smart defaults: options kept; common path becomes one simple decision.|

## Part 2: humane-design arguments
12 arguments for humane choices, then caution applying to all.

### 1 Long-term business health
- Deception → results spike, then reverse.
- Cases: subscription service simplifying cancellation saw refunds rise 30% + subscriptions fall 15%, exposing revenue previously extracted by friction. Budget airline dropped opt-out add-ons only after its profit fell.
- Trust = the asset. Honest design becomes advantage as blocking, tracking protection + privacy law spread.

### 2 Legal + PR risk
- Enforcement against deceptive patterns now reaches up to nine figures.
- Cases: game publisher paid 245 million dollars; diet app paid 62 million; telecom paid 105 million (deceptive-pattern enforcement actions). Boycott cost ride-hailing firm about 200,000 users.
- EU rules: withdrawing consent must take no more effort than giving it.

### 3 Mock headline
1. Draft negative press coverage the feature could generate.
2. Present it w/ question: what will team do to avoid it?
3. Follow w/ concrete dos + don'ts.
4. Cite companies later forced to retrofit fix.
- Why: mockups reach leadership faster than strategy decks.
- Hypothetical: mock headline → "Smart doorbell's neighbourhood feed showed burglars which homes stood empty."

### 4 Predatory twin
- Take ordinary, well-liked object from outside your product category; describe version measuring success by how much you consume, knowing enough about you to press at your weakest moment, paid for by whoever supplies refill.
- Set your feature beside its predatory twin; name shared properties.
- Why: reaches people fluent in engagement vocabulary; they would otherwise cheerfully defend same mechanic.
- Hypothetical: reading lamp counting success in hours lit, noticing when you read late + tired to push paid brighter mode, funded by seller of light credits. Other candidates: umbrella, garden hose.

### 5 Show positive results
- Precedents: visible guard on profile pictures cut copying of them by about three quarters; prompt, specific ban explanations dropped reoffending below 8%; location app's anonymous mode immediately eased users' fears.
- Build on internal initiatives already shown to work.

### 6 Name the pattern
- Use [deceptive-pattern taxonomy](../ethics/deceptive-patterns.md) names: roach motel, forced continuity, sneak into basket, hidden costs, misdirection, trick questions, disguised ads, bait and switch, friend spam, price-comparison prevention.
- Why: naming turns vague discomfort into objection stakeholders can hear.
- Always bring honest alternative.

### 7 Inclusion as reach
- Roughly half of people have some disability by around age 70.
- Solving design problem for one group extends to many. So-called 1% of users = millions of people.
- Three-part message leaders can repeat w/o notes:
  1. Inclusive work widens who can buy + use product.
  2. Inclusive work tends to produce features whole market ends up wanting.
  3. Inclusive work leaves company in defensible public position, not reactive one after complaint/lawsuit.

### 8 Bring the replacement
- Never decline growth mechanic empty-handed: bring replacement, not only objection. Declining w/o one = moment recommendation loses the room.
- Substitute retention paths: reason to return valued by person; reminders at hour they chose; resumable sessions; faster route to first benefit; periodic summary of what product did for them.
- With replacement:
  1. Name metric it should move.
  2. Propose time window for judging it.
  3. Offer staged rollout w/ holdout group (process-safeguards.md) → settled w/ data, not conviction.

### 9 Ask what the metric is tied to
- Before arguing ethics, ask what business result metric ties to.
- Symptom: teams inherit default analytics, then defend those numbers as goals.
- More pages per visit does not mean more sold. More app opens per week does not mean customer trusting you w/ their money.
- Hypothetical: tax-filing service meant to finish each return in one sitting → more sessions per return may count as evidence against product doing its job, not of engagement.
- Growth metric nobody can connect to revenue/retention = easiest to replace; replacing it removes pressure producing deceptive pattern.

### 10 Protective friction already accepted
- Every organization already slows people where it cares about outcome; nobody files such protective friction as usability failure.
- Hypothetical: hospital records system requires second clinician's sign-off before dose changes; smart thermostat asks confirmation before schedule leaving home unheated for days.
- Question = not whether deliberate effort belongs in product but which harms justify extra step.
- Harm to product's user deserves at least as much consideration as fraud + spam get.
- Hypothetical: nobody would hire electrician ranking wiring speed above safety; standard does not change for software work.

### 11 Change what the organization takes for granted
- One good argument wins one feature; what lasts = shift in what organization takes for granted.
- One account of deep innovation names two engines of deep change: capability reliable + cheap enough to build on; change in what something means to people.
- Change-of-meaning engine available to people w/o authority over business model. Steps:
  1. Ask why practice exists until someone says reason aloud.
  2. Ship one honest disclosure/opt-in as precedent next argument can point at.
  3. Name shift already under way outside company (e.g. being tracked has moved, for much of public, from unremarkable to unacceptable).
- Slower than mandate but much harder to reverse.

### 12 Reciprocity test
- Comfortable if used on us, our parents, our children?
- If done in person, w/o technology, ethical?
- What would future whistleblower say about it?

## Five objections to calm design
Five standard objections recur; each has concrete answer.

|Objection|Answer|
|---|---|
|Adding features always adds value|Features compete for one fixed attention pool; features nobody finds still cost support, testing + screen space → measure how many features get used before adding another.|
|No legacy feature can ever be removed|Find each feature's current users + how they use it → retire it, merge it, or move long tail behind secondary route.|
|Other stakeholders need things too|Name each stakeholder + what they need from this release → objection becomes specific conflict, not abstraction.|
|Schedule leaves no room to test|Handful of sessions w/ real people in real conditions costs days + catches what launch would surface expensively + in public.|
|Nothing can be shown to outsiders before launch|Test under confidentiality, w/ small group, or on stripped-back version hiding strategy but not interaction.|

## Caution: business case = reinforcement, not foundation
- Revenue, risk + reputation arguments hold only while numbers agree.
- Accepting "it pays" as reason also accepts case collapsing in quarter it stops paying; somebody will eventually produce model showing it has.
- Lead w/ reason humane choice = right; commercial arguments = reinforcement, not foundation.
- Name findings still standing if numbers ran other way; hold those.

## Related
- ../guides/defend-a-decision.md: rationale w/ law, origin year, mechanism, evidence + metric.
- ../evidence/stating-evidence.md: quoting studies, numbers + origins accurately in argument step 3.
- ../evidence/product-cases.md: comparable product cases for argument step 3 + precedent argument.
- ../evidence/business-cost-of-deception.md: fines, refunds, churn + trust loss behind business-health + legal-risk arguments.
- ../evidence/inclusion-and-exclusion-costs.md: who gets left out + cost, for reach argument.
- counter-metrics.md: pairing each growth metric w/ harm it could hide, for metric + replacement arguments.
- ../ethics/ethics-review-workflow.md: pre-launch ethics review steps + watch-list phrases pausing discussion.
- debiasing.md: countering bias in reviews + team judgment, incl. entrenched stakeholder.
