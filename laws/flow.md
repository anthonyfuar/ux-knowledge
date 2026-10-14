# Flow

## In one line
Flow = complete absorption in ongoing activity; reached when challenge matches skill. Marks: engagement held back nowhere, high-energy concentration, pleasure in doing itself. Use for: sustained focused work/play, where absorption belongs in product, whether "flow" fits engagement claim.
- Class: construct (not law, not effect). Aliases: none.
- Theme: Attention. Most affects: difficulty scaled to skill, feedback on actions, friction removal + discoverability.
- Marks: feeling fully in command + deep concentration on here-and-now.
- Core design rule: features discoverable, friction removed, feedback for each action, challenge matched to skill.

## Applies when / does not apply when
|Situation|Flow?|Do instead / note|
|---|---|---|
|Sustained focused work/play toward own goal|yes: design for absorption|challenge matched to skill, feedback per action, low friction|
|Home page / hub|no: pass through quickly, not dwell|decide where flow belongs; send people on to work|
|Passive consumption|rarely produces flow|do not routinely expect flow from it|
|Endless scroll where absorption serves time-on-site, not user's goal|no: hyperfocus / capture|see Humane bound|
|"Flow" in UX writing (often merely = smooth task path)|much weaker claim than psychological state|do not read as psychological state|
|Challenge-skill balance in place|flow only in people w/ internal locus of control / action orientation|balance alone does not produce flow in everyone|

## Decision rules

### Challenge vs skill
- Flow requires task difficulty matched to person's skill.
- Task asks too little → boredom; too much → frustration.
- If anxious (challenge > skill) → build skill: onboarding, hints, coaching.
- If bored (skill > challenge) → raise challenge: shortcuts, advanced modes, stretch goals.
- Make task harder only when skill already exceeds challenge.
- Challenge must keep tracking growing skill.
- Reduce anxiety + build skill → absorption possible (design consequence of athlete studies; see Evidence).

### Feedback
- Feedback for each action.
- Feedback covers both: outcome reached + which actions went through.

### Friction + discoverability
- Two guards against disengagement: (1) remove purposeless friction → efficient, quick-responding system; (2) keep features + content where people can find them.
- Small breaks accumulate + outweigh smooth moments → polish micro-interactions (hover timing, feedback, affordances) as one chained system; term for them: "interesting moments".
- Aim for painless, not merely simple: complex tools can still produce flow.
- Speed cannot offset design blocking user's goal.

### Placement + edges
- Decide where flow belongs in product; home page: pass through quickly, not dwell.
- After one item done → let people move straight to next; avoid hub return after each action + interruptions during focused work (see Check questions).
- Give natural stopping points in absorbing experiences.

## Why it works

### Mechanism
- Engagement peaks where challenge = skill; feedback + responsive, low-friction system sustain sense of control + unbroken concentration.
- Classic preconditions: clear goals w/ visible progress; immediate, unambiguous feedback; perceived challenge-skill balance (central one).
- 2005 book chapter conditions: know what to do next; know how to do it; no distraction; immediate feedback; high challenge matched by high skill.
- Six features: intense focus on present; action + awareness merged; loss of reflective self-consciousness; sense of control; altered time sense; intrinsic reward (autotelic experience). Flow = their combination.
- 2021 reframing: intrinsically rewarding absorption where strong control feels unusually effortless.
- Self-forgetting = attention fully used: conscious processing estimated ~110 bits per second; understanding speech alone takes about 40–60 → none left for awareness of time, others or hunger.
- Flow most likely at moderate arousal.

### Eight-channel model
Also called Experience Fluctuation Model (1987): plots perceived challenge vs perceived skill, each relative to person's own average; maps combinations to flow, anxiety, boredom, apathy + related states.

|State|Definition in model|If → do|
|---|---|---|
|Flow|perceived challenge + perceived skill both above person's own average|keep challenge tracking growing skill|
|Anxiety|challenge > skill|build skill: onboarding, hints, coaching|
|Boredom|skill > challenge|raise challenge: shortcuts, advanced modes, stretch goals|
|Apathy|challenge + skill both low|no rule given|

### Origin
- Term "flow" coined by psychologist in 1975; original support = 1975 psychological construct, not UX experiment.
- By some accounts idea itself millennia old, under other names before term existed; some claim this, not established fact.
- Many fields cite term; occupational therapy one, notably familiar w/ it.

## Evidence
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Flow = state of total, enjoyed absorption|1975 psychological construct|construct, not UX experiment|discoverable features, low friction, feedback per action, challenge = skill|
|Pianists entering flow: lower heart rate + blood pressure, relaxed facial muscles, improved performance|research on flow as "effortless attention"|year + sample not stated|none stated|
|Higher skill went w/ less competitive anxiety, more confidence, more flow; anxiety correlated negatively w/ flow|questionnaire study, 328 youth football players (172 higher-league, mean age 14.72; 156 lower-league, mean age 17.11)|questionnaire; associations|reduce anxiety + build skill → absorption possible|
|94% described flow as action + awareness merging + as effortless|qualitative study, NCAA Division I athletes|qualitative|same: reduce anxiety, build skill|
|Flow had only small causal effect on performance; most correlation ran performance → flow (good performance produced flow more than reverse)|one longitudinal academic study|one study|do not sell flow as cause of better performance|
|Flow makes people 5x more productive|vendor claims|lack study details|do not cite them|

## Misreadings and limits
- Wrong: calling endless scroll / long sessions "flow" → Right: flow serves user's goal; compulsive time-on-site = hyperfocus / capture. Endless scroll not flow when absorption serves time-on-site, not user's goal.
- Wrong: "flow" in UX writing = psychological state → Right: there often merely = smooth task path, much weaker claim.
- Wrong: passive consumption creates flow → Right: rarely does.
- Wrong: challenge-skill balance yields flow for everyone → Right: produced flow only in people w/ internal locus of control / action orientation.
- Wrong: simple = flow → Right: aim for painless, not merely simple; complex tools can still produce flow.
- Wrong: faster system restores flow on its own → Right: speed cannot offset design blocking user's goal.
- Wrong: flow drives productivity (e.g. vendor "5x" claims) → Right: such claims lack study details; one longitudinal study found mostly performance → flow, little flow → performance.
- Wrong: idea millennia old (as fact) → Right: some claim it, not established.
- Limit: hyperfocus resembles flow but can trap people, e.g. excessive gaming, fixating on one part of task.
- Limit: flow has dangers; warning came from within term's originating research line.

## Check questions
[A] = answerable from artifact itself (screen, prototype, spec).
- [A] Challenge matched to skill, feedback on every action? Look for: no confirmation of what happened; friction, lag / hidden features breaking absorption.
- [A] Users go straight to next item after completing one? Look for: hub return after each action; interruptions during focused work.
- Feedback names both outcome reached + which actions went through?
- Features + content findable, no purposeless friction left?
- More challenge (shortcuts, advanced modes, stretch goals) once skill grows + skill support (onboarding, hints, coaching) for those struggling?
- Natural stopping points in absorbing experience?
- Claimed "flow" serves user's goal, not time-on-site?

## Symptoms → fixes
|Symptom|Likely cause|Fix|
|---|---|---|
|Disengagement, loss of flow|hidden features, needless friction, sluggishness, missing feedback|features findable; purposeless friction removed; responsive system; feedback naming outcome + action|
|Boredom|skill > challenge|raise challenge: shortcuts, advanced modes, stretch goals|
|Frustration, anxiety|challenge > skill|build skill: onboarding, hints, coaching|
|Absorption keeps breaking|hub return after each action; interruptions during focused work|move people straight to next item; hold interruptions|
|Overall experience feels rough though each step "fine"|small breaks accumulating|polish micro-interactions (hover timing, feedback, affordances) as one chained system|
|Long sessions reported as "flow" success|absorption serving time-on-site = capture|natural stopping points; measure benefit to user's goal, not time-on-site|

## Hypothetical examples
- Hypothetical: supporting flow → radiology reading workstation confirms "Report signed, sent to referring clinic" after each signature, opens next study w/o trip back to worklist, loads images w/o lag, keeps every measuring tool on one visible toolbar.
- Hypothetical: anxious vs bored → household-budget app: first-time user gets guided setup w/ hints while categories feel overwhelming; long-time user breezing through gets keyboard shortcuts + custom rules.
- Hypothetical: stopping point → evening crossword app ends each puzzle on calm "done for today" screen, not auto-starting next one.
- Hypothetical: wrong word → news site growth deck calls rising minutes-per-visit "flow"; reviewer reclassifies as time-on-site until shown to serve reader's goal.

## Humane bound
- Bounded by Finite + Intentional.
- Turned against people: flow mechanics can turn play into unpaid work / trap people in hyperfocus (2021 critique argued gamification uses flow to turn play into unpaid work).
- Turned against people: endless scroll + long sessions labelled "flow" while absorption serves time-on-site, not user's goal = capture.
- Counter-moves: natural stopping points; tell capture (time-on-site) from benefit to user's goal.
- Further reading: feeds, scrolling + pacing patterns (stopping points, infinite scroll, autoplay); habits, streaks + gamification patterns (gamification built on flow); influence vs manipulation.

## Related
- ../principles/finite.md: humane principle bounding Flow; experiences need edges + stopping points.
- ../principles/intentional.md: humane principle bounding Flow; absorption must serve user's goal.
- ../patterns/feeds-scrolling-and-pacing.md: humane bounds on absorption (stopping points, infinite scroll, autoplay).
- ../patterns/habits-streaks-and-gamification.md: humane bounds on gamification built on flow.
- ../ethics/influence-vs-manipulation.md: further reading on humane bound.
- doherty-threshold.md: system responsiveness keeps focus.
- cognitive-load.md: related law.
- paradox-of-the-active-user.md: skill grows through use.
- ../methods/measuring-flow.md: method: checks whether challenge matches skill.
- ../methods/engagement-vs-empowerment-metrics.md: tells capture (time-on-site) from benefit to user's goal.
- ../guides/laws-and-principles-crosswalk.md: names humane principle bounding Flow.
- ../patterns/onboarding-and-first-use.md: applies Flow.
- ../patterns/feedback-loading-and-performance.md: applies Flow.
- ../patterns/progress-goals-and-completion.md: applies Flow.
