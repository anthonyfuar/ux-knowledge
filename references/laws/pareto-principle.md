# Pareto Principle

## In one line
Effects concentrate: 20% of causes → roughly 80% of effects (80/20 split). Matters when deciding where effort goes first: what benefits most users most, split read as approximate.
- Alias: 80/20 rule. Class: effect / principle. Theme: Decisions.
- Reaches furthest into: feature + bug prioritization, focus on highest-impact flows, where research effort goes.
- Status: analytical lens, not law of nature + not measured ratio for your particular product.

## Applies when / does not apply when
|Use it when|Hold back / take care when|
|---|---|
|inputs + outputs badly uneven (UX strategy = one such system)|precise ratio needed: split approximate + holds across many kinds of events, not all|
|ranking features, issues, flows / user segments by impact|small sample: handful of helpdesk calls proves nothing|
|choosing where research effort goes|you need to know when/why imbalance will appear: principle empirical + says neither|
|picking problems to fix first|problem small now but growing: Pareto analysis misses it|

## Decision rules
- Expect skew: inputs not equal, nor outputs. Most of wanted result comes from small share of big group.
- Rank candidate work by how many users it helps + how much → bulk of effort to top of ranking.
- Procedure: (1) rank features, issues + user segments by impact; (2) invest first in small set giving most value to most users; (3) remember split approximate.
- Fix high-frequency few problems first; real splits often more skewed than 80/20.
- Weight counts by value: less frequent complaint from high-value customers may deserve fixing first.
- Read imbalance size, not only whether one exists.
- Ratio varies by context; aim = find the few variables moving outcome.
- Do not force split's two numbers to sum to 100; they measure different things.
- Keep capacity for long tail: taken literally, 80/20 still leaves ~20% of value in less-used majority.
- If one top set held focus long → check for stagnation + a few metrics over-optimized at others' expense; pair growth metrics w/ counter-metrics.
- Track small-but-growing problems separately; Pareto ranking will not surface them.
- If data few → collect more before ranking.

## Why it works

### Mechanism
- Analysis tool: wherever inputs + outputs badly uneven (UX strategy = one such case), 80/20 reasoning carries over widely, though it sounds imprecise.
- Vital minority of inputs (features, users, issues, contributors) produces most outputs → focus there = outsized value.
- 80/20 split = one case of power-law (Pareto) distribution, Pareto index α = log4(5), ~1.16.
- Power laws scale-invariant; under them extreme values far more likely than bell-curve thinking predicts.
- Under power law largest cause usually dwarfs second, second dwarfs third → one factor tends to dominate observed variation.
- Top-task analysis ("long neck"): a few tasks win most of users' votes.

### Origin
- Began w/ economic observation in 1896–97 economics course: 20% of Italy's population held 80% of its land. Link to 80/20 split often dated to ~1906.
- Pea-pod origin story = anecdotal.
- 1941: carried into quality control, observing most defects come from minority of causes.
- Quality-control phrase vital few + trivial many later revised by its own proponent to vital few + useful many.

## Evidence
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|222 prospective users each picked 5 of 94 tasks; top 15 tasks (16%) drew 41% of votes|top-task survey; 222 prospective users|one survey|design around top few tasks first|
|Coded answers to "one thing to improve": 2 issues = 50% of comments, 5 issues = 75%|coded open-ended feedback|one dataset|fix dominant few issues first|
|33 unique problems occurred 181 times; 9 of them (27%) caused 72% of poor interactions; long tail of problems hit one user each|formative usability test, car-rental product; 50 users|one test|fix frequent few first; long tail still real|
|Fixing top 20% of most-reported bugs removed 80% of related errors + crashes|software vendor report, 2002|industry report|fix most-reported few first|

Caveat: UX evidence for Pareto = one survey, one usability test + one industry report.

### Stating evidence for neighbouring laws
- Parkinson's Law comes from humorous essay, not study → do not overstate it.
- 1982 figures behind Doherty Threshold vendor-authored.
- Goal-Gradient Effect rests on animal studies + 2006 human field study of real rewards: customers speeding up more toward first reward more likely to earn another + came back sooner. Never restate it as finding about why people drop out.
- Complexity bias well illustrated by 1989 study: most participants proposed rules more elaborate than hidden one (any three ascending numbers). Study's own conclusion concerns reasoning strategies shifting w/ task, not complexity bias as such. Three-number rule-discovery task itself dates from 1960.

## Misreadings and limits
- Wrong: optimize top set + ignore remaining 80% → Right: this = misapplication to avoid; less-used majority still carries value.
- Wrong: 80/20 exact or universal → Right: approximate lens for uneven systems; real splits often 90:10 or 70:30 rather than 80:20.
- Wrong: trivial many worthless → Right: phrase revised to useful many; keep capacity for long tail.
- Wrong: two numbers must sum to 100 → Right: they measure different things.
- Wrong: run Pareto analysis on handful of data points → Right: small samples cannot support it; also weight counts by value.
- Wrong: imbalance exists, so job done → Right: its size matters too.
- Limit: Pareto analysis misses problems small now but growing.
- Limit: fixating on top set too long → stagnation + a few metrics over-optimized at others' expense.

## Check questions
- Effort going to features most users rely on? Look for: polish spread evenly over rarely used features.
- Sample big enough to support ranking?
- Counts weighted by value, not only frequency?
- Anything small but growing tracked outside ranking?
- Capacity kept for long tail + less-used majority?
- Each optimized metric has counter-metric?

## Symptoms → fixes
|Symptom|Likely cause (laws)|Fix|
|---|---|---|
|Settings page w/ dozens of toggles hard to scan|Cognitive Load, Chunking, Common Region, Tesler's Law via progressive disclosure, Pareto Principle (check usage w/ analytics); not Choice Overload|task-based labelled groups; search across setting names, synonyms + descriptions; advanced settings behind disclosure|
|Polish spread evenly over rarely used features|effort not ranked by impact (Pareto Principle)|rank by impact; invest first in small set most users rely on|
|Less-used majority deprioritized w/o review|top set fixated on; useful many read as trivial (Pareto Principle, Inclusive)|keep capacity for long tail; read exclusion evidence before deprioritizing|

## Hypothetical examples
- Hypothetical (rules of thumb, not measurements): city services portal: a few request types may make up most visits; online learning platform: a few courses may draw most enrolments. Treat both as hunches until counted.
- Hypothetical (one dominant cause): clinic's online booking flow: most abandoned bookings stall at same insurance-details step → fix that step first.
- Hypothetical (one dominant use): workplace expense tool finds most claims one type, travel → streamline travel claim form first.

## Humane bound
- No manipulation case recorded. Recorded misuse = exclusion: remaining 80% ignored, trivial many read as worthless, a few metrics over-optimized at others' expense.
- Heavy barriers stay because people meeting them not counted as market.
- Bound by Inclusive.
- Before deprioritizing less-used majority → read evidence on inclusion + exclusion cost.
- Further reading for this bound: inclusion + exclusion costs; friction, undo + deliberate pauses (ask whose friction you remove); counter-metrics.

## Related
- occams-razor.md: same Decisions theme.
- hicks-law.md: both favour prioritizing frequent path.
- ../methods/pareto-chart.md: step list for ranking problems by impact share.
- ../methods/top-tasks-and-user-problem-matrix.md: finds the few tasks + problems mattering most.
- ../methods/counter-metrics.md: humane bound on over-optimizing a few metrics; pairs each growth metric w/ harm it could hide.
- ../evidence/inclusion-and-exclusion-costs.md: people left out + what it costs; read before deprioritizing less-used majority.
- ../patterns/friction-undo-and-confirmation.md: ask whose friction you remove.
- ../checklists/usability-heuristics-map.md: links Pareto Principle to Flexibility and efficiency of use (w/ Tesler's Law + Parkinson's Law); classic heuristics from 1990, revised 1994.
- parkinsons-law.md: evidence = humorous essay, not study.
- doherty-threshold.md: 1982 figures vendor-authored.
- goal-gradient-effect.md: 2006 field study; not a finding on why people drop out.
- cognitive-load.md: leading law for settings-page symptom.
- chunking.md: shares settings-page fix.
- common-region.md: shares settings-page fix.
- teslers-law.md: progressive disclosure in settings-page fix.
- ../principles/inclusive.md: principle bounding Pareto Principle.
- ../guides/laws-and-principles-crosswalk.md: names humane principle bounding Pareto Principle.
- ../patterns/lists-options-and-choice.md: applies Pareto Principle.
- ../patterns/dashboards-and-data-displays.md: applies Pareto Principle.
- ../patterns/complexity-management.md: applies Pareto Principle.
