# Reading experiments honestly

## Use when
- Planning/reading product test, above all smoother flow vs more considered one.
- Covers: why short test favours frictionless variant · three habits keeping single test honest · two habits for what many tests accumulate into.

## Why a short test is not a fair referee
- Short test = not fair referee between smoother + more considered flow: frictionless variant wins almost by construction.
- Effort removed from flow felt at once + lands on watched number.
- Removed friction's cost arrives later, falls on people outside test, or shows up in something nobody instrumented.
- Hypothetical: one-tap "extend my overdraft" button in banking app saves effort on use (what test watches); any cost comes later as repayment worry, in support calls nobody links to test.

## Three habits for a single test
|Habit|Do|Because|
|---|---|---|
|1 Keep condition|Write down beforehand what result would keep slower version.|W/o it, whichever line ends higher decides test.|
|2 Window|Choose test window long enough for cost to surface.|Single-week read rewards whatever moves fastest.|
|3 Name what test cannot see|Where effect cannot appear inside test, say so plainly + argue from mechanism, not from number answering only easy half of question.|Skipping it = asking people how design makes them feel, then shipping whatever moved metric → teaches everyone qualitative work = decoration.|

## Two habits for what tests accumulate into
- Why: no team decides in one meeting to build compulsive product; each mechanic arrives as small test winning on own number. Experimentation tunes product toward compulsion faster than review inspects it.
1. **Scheduled review of accumulated experience**: put every change shipped since last review before team together. Judge product as one person meets it today, not each increment alone.
2. **Same rigour for well-being as for conversion**: if mechanic worth testing, its counter-metric worth testing too: same population, longer window than win.

## Check questions before reading a result
- Keep condition for slower version written before test?
- Window long enough for delayed costs to surface?
- Which effects could not appear inside this test? Stated?
- Counter-metric tested on same population, over longer window?
- Accumulated experience last reviewed as whole: when?

## Pitfalls
- No keep condition written beforehand → whichever line ends higher decides test.
- Single-week read → rewards whatever moves fastest; choose window long enough for cost to surface.
- Judging each increment alone → judge product as one person meets it today.
- Testing mechanic but not its counter-metric → test both, same population, counter-metric over longer window than win.

## Related
- counter-metrics.md: pairing each growth metric w/ harm it could hide + what to do when it trips.
- process-safeguards.md: incl. staged rollout w/ withdrawal condition written first.
- engagement-vs-empowerment-metrics.md: telling capture from benefit before choosing number to watch.
- measure-what-you-value.md: choosing metrics reflecting value to people.
- behavioral-insight-to-tested-change.md: usability-side method ending in controlled experiment, read by these rules.
- debiasing.md: countering bias in studies, reports + team judgment.
- ../patterns/friction-undo-and-confirmation.md: confirmation graded by consequence, undo windows, speed bumps; slower variants such tests weigh.
- ../evidence/convenience-and-friction.md: what removing/adding friction does.
