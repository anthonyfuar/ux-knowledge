# Top tasks and the user-by-problem matrix

## Use when
- Ranking tasks, usability problems or feedback by impact before polishing.
- Deciding what navigation, testing + fixes get built around.
- Techniques: top-task analysis · user-by-problem matrix · grouping quantitative data · reading 80/20 split.
- Why rank first: resources finite + problems effectively unlimited → rank by impact before polishing.

## Top-task analysis
1. Give prospective users full task list; each picks their top five.
2. Find long neck = small task set taking most votes.
3. Build navigation, testing + measurement around top tasks.
- Never degrade top tasks in any redesign.

## User-by-problem matrix
- Grid of test participants × usability problems they hit.
- Rank fixes by how many users each problem hit.
- Code open-ended feedback same way.

|Problem|P1|P2|P3|Users hit|
|---|---|---|---|---|

## Grouping quantitative data
1. Group tickets, bugs, requests, analytics.
2. Check audience share in each group.
3. Weight counts in each group by value.

## Reading the 80/20 split
- Read loosely: about 10 to 40% of inputs behind most results.
- Do not chase exact 80/20 split; look for any small set w/ large effect.
- Dominant small set helpful → amplify it (e.g. tailor heavily used area to user needs).
- Dominant small set harmful → suppress it (e.g. fix first the one defect behind most complaints).
- Target several dimensions at once, not single split. Hypothetical: hospital shift-rostering tool: cross three dimensions (task share, staff share, time share) → focus design attention on the few tasks nearly all staff do most often (e.g. swapping shift, checking next week's rota).
- Set real thresholds from product maturity, industry, user type, use context + business goals.

## Hypothetical example
Hypothetical: council waste-services site runs top-task vote; "check my collection day" + "report a missed bin" form long neck → home page, search tests + success measures centre on them; redesign not allowed to make either slower. User-by-problem matrix from usability sessions then shows form problem hitting most participants; its fix goes first.

## Pitfalls
- Exact 80/20 hunting → any small set w/ large effect counts.
- Raw counts only → weight by value.
- Single split → several dimensions at once.
- Focus on small set alone → check who gets left out (Related).

## Related
- ../laws/pareto-principle.md: law behind both techniques: definition, limits, evidence.
- pareto-chart.md: step list for charting impact share once data grouped.
- thresholds-and-formulas.md: measurable form of each law, incl. Pareto row.
- ../patterns/navigation-and-menus.md: ordering, grouping, depth + visibility of navigation built around top tasks.
- debiasing.md: countering bias in studies + reports when coding feedback.
- measure-what-you-value.md: humane bound on weighting counts by value: value to people.
- ../evidence/inclusion-and-exclusion-costs.md: who gets left out + cost; read alongside any small-set focus.
