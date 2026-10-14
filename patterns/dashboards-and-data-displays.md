# Dashboards and data displays

## Use when
- Covers dense data screens: dashboard content + order, review checklist (hierarchy, density, navigation vs filters, freshness), chart colour, loading + refresh.
- Open when designing/reviewing: dashboard, report, monitoring / analysis screen, chart.
- Laws in play: Pareto Principle, Working Memory, Cognitive Load, Von Restorff Effect, Selective Attention, Cognitive Bias.

### What goes on the dashboard, and in what order? (build around decisions)
- When: monitoring + analysis screens.
- Do:
  - Order tiles by decision each supports, most-used first.
  - Pre-computed deltas + comparisons, not users relating > 2-3 variables themselves.
  - Labels, units + legends on chart itself; separating them → split-attention effect.
  - Sample size beside every rate / rating → counters base-rate neglect.
  - Out-of-range value stands out by quieting everything else.
  - Each alert points at tile needing action.
  - Active filters + time range visible in every view → users need not hold them in working memory.
  - Notes + action history for analysis spanning several days.
  - 2020 task-based taxonomy of judgment biases as checklist: what biases each view invites?
- Avoid: decorative icons + gauges. Status by colour alone. Several alerts animating at once → splits limited attention.
- Why: Pareto Principle (tile order), Von Restorff Effect (out-of-range value, alert pointing at tile), Working Memory (visible filters + range), Selective Attention (several alerts animating at once), Cognitive Bias (bias checklist, sample size).
- Hypothetical: hospital bed-management screen leads w/ "beds free now vs same hour yesterday", shows "n = patients" under each discharge rate + greys all ward tiles except over-capacity one.

### Does an existing dashboard pass review? (hierarchy, density, navigation vs filters, freshness)
- When: reviewing dashboard / report.

|Area|Check|Passes when|
|---|---|---|
|Hierarchy|Headline|a few headline KPIs at top|
|Hierarchy|Context per KPI|each headline KPI has comparison (target / prior period) + shows which direction = good|
|Hierarchy|Detail|detail + breakdowns below headline / one click away|
|Hierarchy|Focus|each view answers one dominant question|
|Density|Expert use|dense layout for daily experts = modular, w/ consistent alignment + number formats|
|Density|What to cut|decoration cut before data|
|Density|Occasional use|occasional users: fewer tiles + more explanation|
|Navigation vs filters|Distinction|navigation (changes what's viewed, e.g. another report / entity) + filters (change current view's scope, e.g. time, region, segment) look + sit apart|
|↑|Active filters|shown as removable chips|
|↑|Filter reach|says whether filter applies to one tile / whole page|
|Freshness|Provenance|each view shows last-updated time + data source|
|Freshness|Stale data|stale / partial data flagged; never shown silently|

- Hypothetical: school-district attendance report: removable chips for term, school phase + year group above tiles, apart from report tabs; one chip reads "this tile only".

### Which colours for charts?
- When: choosing chart colour + emphasis.
- Do:
  - Colour as data, not decoration.
  - One colour per metric / category, constant across all charts + views.
  - Categorical palette: a few distinct hues, distinguishable under common colour-vision deficiencies; check w/ simulator.
  - Sequential palette for ordered values. Diverging palette only around meaningful midpoint.
  - Label lines + bars directly, not via legend.
  - Context series grey + single accent colour on key series.
  - Chart marks: ≥ 3:1 contrast vs background.
- Avoid: rainbow scales for ordered data. Red + green as only good + bad signal. One colour for different metrics on same page. More categories than palette keeps distinct → group rest as "Other".
- Why: Law of Similarity (one constant colour per metric / category). Von Restorff Effect (grey context, one accent). Accessibility floors bound colour + contrast choices.
- Hypothetical: energy-utility usage chart: household's own line in one accent colour, neighbourhood average grey, each line labelled at its end.

### How should the dashboard load and refresh?
- When: first load, refresh, filter change, failed queries.
- Do: first load → skeleton tiles shaped like final charts. Refresh / filter change → previous data stays visible (dimmed / small inline indicator) until new data arrives. Tiles load independently → one slow query never blanks whole page. Per-tile errors, each w/ retry.
- Avoid: full-page spinner hiding all data on every refresh. Numbers changing w/o any cue they changed.
- Why: slow query / error stays local to its tile; data never vanishes on refresh. Indicator choice by expected wait → feedback + loading patterns.
- Hypothetical: logistics-fleet dashboard: after region filter change, old map stays dimmed while reloading; only fuel tile shows "could not load, retry".

## Related
- layout-grouping-and-hierarchy.md: grouping cues, spacing, containers + emphasis for tiles + views.
- feedback-loading-and-performance.md: indicator choice by expected wait, skeletons, refresh keeping stale data visible.
- ../laws/similarity.md: behind one constant colour per metric / category.
- ../methods/top-tasks-and-user-problem-matrix.md: finds the few tasks + problems mattering most → sets tile order.
- ../methods/debiasing.md: counters bias in reports + team judgment.
- inclusive-and-accessible-design.md: accessibility floors bounding colour + contrast choices.
- ../methods/measure-what-you-value.md: picking headline metrics reflecting value to people.
- ../methods/counter-metrics.md: pairs each growth metric w/ harm it could hide.
- ../laws/pareto-principle.md: most-used tiles first.
- ../laws/working-memory.md: why filters + time range stay visible.
- ../laws/cognitive-load.md: in play for dense data screens.
- ../laws/von-restorff-effect.md: quiet everything else → outlier stands out.
- ../laws/selective-attention.md: several animated alerts split limited attention.
- ../laws/cognitive-bias.md: biases each dashboard view can invite.
