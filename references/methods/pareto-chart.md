# Pareto chart

## Use when
- Deciding where to act first: ranking pages, features, segments or problems by impact share.
- Pareto chart = value bars + cumulative line, items ranked by impact share. Step list below + two cases.

## Steps
1. **Start from goal + hypothesis.** Confirm data exist + clean; check you can export them.
2. **Choose category + metric.**
|Category|Metric|
|---|---|
|pages, features, segments, problems|views, clicks, cost, complaints|
3. **Sort high → low.** Compute each item's share of total + cumulative-percent column.
4. **Plot**: values as bars; cumulative percentage as line on second axis. Horizontal line at 80% + vertical line where it meets cumulative curve. Items left of vertical line = priority set. Check priority set covers ≥ 80% of total.
5. **Find root causes** of dominant items w/ fishbone diagram. Problems small now but growing → add failure mode and effects analysis.
6. **Keep some capacity for long tail.**

## Cases
|Case|Result|Decision|
|---|---|---|
|One app, negative feedback|3 features = 86% of negative feedback|Fixed those ahead of quicker wins.|
|Redesign cut trial sign-ups|77% of remaining sign-ups had visited pricing page|Research started there, though other pages had higher exit rates.|

## Hypothetical example
Hypothetical: city public-services portal charts support calls by topic; bars left of vertical line (e.g. parking permits, bin collection) = priority set, fishbone diagram for each, slice of team time stays on rarer topics.

## Output
- Ranked table w/ share + cumulative percent; chart w/ 80% line; priority set; root-cause diagrams; named long-tail reserve.

## Pitfalls
- Unclean/unexportable data → confirm in step 1 before charting.
- Assuming left-hand items reach 80% → check priority set covers ≥ 80%.
- Spending all capacity on priority set → keep some for long tail.
- Metric ignoring value to people → see humane bound in Related.

## Related
- ../laws/pareto-principle.md: law behind chart: definition, limits, evidence.
- [Top tasks and user-by-problem matrix](top-tasks-and-user-problem-matrix.md): finding the few tasks + problems mattering most; reading 80/20 loosely.
- thresholds-and-formulas.md: measurable form of each law, incl. Pareto row.
- ../patterns/dashboards-and-data-displays.md: chart color, comparison + prioritisation on dense data screens.
- ../guides/write-a-finding.md: severity ranking for problems chart puts first.
- measure-what-you-value.md: humane bound on step 2 metric: value to people.
- ../evidence/inclusion-and-exclusion-costs.md: who gets left out + cost; read alongside long-tail step.
