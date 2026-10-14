# Parkinson's Law

## In one line
Work expands to fill time allotted to it: task consumes all time granted, however much. UX lens: users judge task speed vs expected duration → beat it (autofill, entered-data reuse, short purchase + booking flows).

- Theme: Motor/time. Classed as effect / principle. No aliases.
- Most affected: autofill, flow length vs expected duration, time-saving shortcuts in checkout + booking.
- Evidence status: humorous observation, not controlled study.

## Applies when / does not apply when

|Situation|Parkinson's Law?|Cite instead / also|
|---|---|---|
|Flow longer than users expect (forms, checkout, booking)|Yes, expected-duration lens|Measure expected vs actual time|
|Removing steps via stored-data reuse|Lens only|teslers-law.md first (system carries stored data)|
|Setting time boxes, step budgets, caps, time estimates|Yes|Planning fallacy, time-saving bias (below)|
|Bloating collections (space) / portions getting finished (quantity)|Yes, beyond time|Caps + unit sizing|
|Committee / review time on trivial items|Companion law of triviality (same essay)|Time-boxed flows, small approval groups|
|Claim needs experimental support|No: began as line in humorous essay|Say so when citing|
|Universal time-to-value target (e.g. 'first result within 2 minutes')|No research figure supports one|Own cohort data, labelled hypothesis; ../methods/activation-moment.md|

## Decision rules

### Time inside the product
- Users' expected task time = run-time ceiling.
- Benchmark = user's expected duration, not abstract speed.
- If task ends sooner than expected → experience improves.
- Bookings, purchases + similar stay short, w/o swelling, when forms fill critical info for user (autofill + similar time-savers).
- Steps:
  1. Measure expected vs actual task time.
  2. Aim to finish under expectation (autofill, entered-data reuse).
- If speeding up → target system's slowest part; report absolute time saved (time-saving bias).
- Redesign may feel slower at first though objectively faster (well-travelled road effect).
- Pad user-facing time estimates for planning fallacy (tasks take longer than predicted; 2004 research).
- Never cut explicit confirmation before money moves / content shared (see Humane bound).

### Time boxes in interfaces + the design process
- Firm, reachable time boxes + step budgets.
- Keep limit realistic: far below real minimum (e.g. one day for full dissertation) → failure, not focus.
- Scheduling + planning tools → default to firm, realistic time boxes from past durations.
- Counter law of triviality: explicit time-boxed flows, small approval groups, reviews on consequential decisions.

### Space + quantity
- Countermeasures: caps + unit sizing (one-in-one-out, smaller portions, small countable units).
- Cap bloating collections: pinned items, saved drafts, open workspaces.
- Meter usage in small visible units, not one open-ended pool.

### Citing
- If used as evidence → state source: humorous essay, not experiment.

## Why it works

Mechanism:
- Work inflates into available time; constraining time + beating expected duration prevents it + feels efficient.
- Generous allowance removes pressure to choose well → effort drifts into deliberation + polishing.
- Firm limit forces choice: essential vs optional.
- Felt duration built from remembered events + familiarity, not clock time.
- Estimates fail both ways; in one, people allow too little time for concrete tasks (planning fallacy).
- People bargain w/ others + themselves for slack time; task then expands into it (practitioner essay, not study).
- People over-expect what they can do short-term + under-expect what they can do long-term.
- Extends beyond time: possessions fill available storage (space); people tend to finish whatever portion served (quantity).

Related terms:
|Term|Meaning|
|---|---|
|Law of triviality (bike-shedding)|Companion law, same essay: committee time on item inversely related to item's cost|
|Planning fallacy|Tasks tend to take longer than predicted (2004 research)|
|Time-saving bias|People underestimate time saved by speeding up from slow speed + overestimate it from already fast speed (2008 research)|
|Well-travelled road effect|Familiar routes feel shorter than unfamiliar ones of equal length|

Origin, dated:
|When|What|
|---|---|
|1955|Humorous essay from long British Civil Service experience; law's wording = its opening line; appeared in weekly magazine, now also online|
|1955|Essay holds 2 versions: work swells to fill time allowed (usual meaning) + administrative headcount grows regardless of workload|
|1955|Satirical explanation: officials want subordinates, not rivals; departments make work for each other → organization grows w/o producing more|
|1958|Collected w/ several other essays in book published in London|
|1990, 1994|Classic usability heuristics (revised 1994); Flexibility and efficiency of use links to law|

## Evidence

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Work swells to fill time allowed|1955 humorous essay, British Civil Service experience|Observation, not controlled study|Use as lens; never cite as experiment|
|5–7% yearly staff growth (headcount version), citing Admiralty + Colonial Office figures|1955 essay|Satirical essay|Illustrative only|
|Colonial Office added staff every year while empire it administered shrank|Observation behind headcount version, 1955 essay|In humorous essay, not study|Illustrative only|
|Mock 'coefficient of inefficiency': committee threshold of ~20 members|Same satire|Weakly sourced satire|Do not quote as threshold|
|Tasks take longer than predicted (planning fallacy)|2004 research|Kind + sample not stated here|Pad user-facing estimates|
|Time-saving bias: misjudged savings from slow vs fast starting speed|2008 research|Kind + sample not stated here|Speed up slowest part; report absolute time saved|

Neighbouring claims often overstated beside this law:
|Claim|Caveat|Use|
|---|---|---|
|Pareto Principle 80/20 split|Approximate|Say 'approximate'|
|Doherty Threshold 1982 figures|Vendor-authored|Say so|
|Goal-Gradient Effect|Rests on animal studies + 2006 human field study of real rewards: customers accelerating more toward first reward = more likely to earn another + returned sooner|Never restate 2006 finding as one on why people drop out|
|Complexity bias|1989 study: most participants proposed rules more elaborate than hidden rule (any three ascending numbers); illustrates complexity bias well|Study's own conclusion: reasoning strategies shift w/ task, not complexity bias as such; three-number task from 1960 work|

## Misreadings and limits
- Wrong: present time-to-value target, e.g. 'first result within 2 minutes', as established (Parkinson's Law, goal-gradient-effect.md). → Right: no research figure supports universal target; derive from own cohort data + label as hypothesis.
- Wrong: cite Parkinson's Law as experimental finding. → Right: began as line in humorous 1955 essay from British Civil Service experience.
- Wrong: cite Parkinson's Law for step removal via stored data. → Right: cite Tesler's Law first; this law gives only expected-duration lens.
- Wrong: set tightest possible limit. → Right: limit far below real minimum → failure, not focus.
- Wrong: judge flow by raw speed. → Right: benchmark = what users expect.

## Check questions
Tag [P] = needs process / research evidence (see ../checklists/usability-review.md).

|Check|Look for|Law / principle|Tag|
|---|---|---|---|
|Task takes no longer than users expect?|Re-typing data system already knows; no autofill in purchase / booking forms|Parkinson's Law|[P]|
|Expected vs actual task time measured?|Only abstract speed tracked, no expected duration|↑||
|User-facing time estimates padded for planning fallacy?|Unpadded estimates|Planning fallacy||
|Bloating collections w/ caps + small visible units?|Uncapped pinned items, saved drafts, open workspaces; one open-ended pool|Parkinson's Law (space, quantity)||

## Symptoms → fixes

|Symptom|Likely cause|Fix|
|---|---|---|
|Forms take too long|Tesler's Law (system carries stored data); Parkinson's Law (expected-duration lens)|Autofill, data reuse, sensible editable defaults|
|Review meetings stall on trivial items|Law of triviality|Time-boxed flows, small approval groups, focus on consequential decisions|
|Saved items / workspaces sprawl|Parkinson's Law extended to space|Caps, one-in-one-out, small countable units|

## Hypothetical examples
- Hypothetical: clinic team w/ open-ended deadline to tidy patient-intake form keeps debating optional fields + rewording labels; w/ short, firm, reachable time box → ships essential fixes + parks optional ones, less polished but usable.
- Hypothetical: smart-thermostat app setup reuses home network + room names user's other devices already know → ends before user expects; library-card renewal finishes on one screen; facilities department's approval steps multiply while requests it handles shrink.

## Humane bound
- No abuse case recorded; general ../ethics/influence-vs-manipulation.md test applies.
- Recorded bound on cutting steps for speed: keep explicit confirmation before money moves / content shared; bounded by ../principles/intentional.md.
- Evidence on removing / adding friction + bound on cutting steps: ../evidence/convenience-and-friction.md; further reading: ../patterns/friction-undo-and-confirmation.md.

## Related
- teslers-law.md: cite first when removing steps via stored data; shares forms-take-too-long fix.
- goal-gradient-effect.md: shares time-to-value-target misapplication.
- doherty-threshold.md: same Motor/time theme.
- ../checklists/usability-heuristics-map.md: Flexibility and efficiency of use links to Pareto Principle, Tesler's Law + Parkinson's Law.
- ../checklists/usability-review.md: meaning of [P] tag.
- ../methods/thresholds-and-formulas.md: each law's measurable form, side by side.
- ../methods/activation-moment.md: find first real success + measure path to it, instead of assumed time-to-value target.
- ../guides/laws-and-principles-crosswalk.md: humane principle bounding law.
- ../patterns/forms-and-data-entry.md: applies law.
- ../patterns/progress-goals-and-completion.md: applies law.
- ../evidence/convenience-and-friction.md: bound on cutting steps for speed.
- ../patterns/friction-undo-and-confirmation.md: further reading on same bound.
- ../ethics/influence-vs-manipulation.md: general test for its humane bound.
- ../principles/intentional.md: confirmation before money moves / content shared.
