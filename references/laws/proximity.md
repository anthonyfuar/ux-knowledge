# Law of Proximity

## In one line
Spatial closeness usually makes separate objects read as one cluster: group sharing function. Matters for: spacing scale between vs within groups, label-to-field distance, list-item gaps.
- Type: effect/principle. Aliases: proximity principle; Gestalt principle of proximity. Theme: Perception (perception and grouping).
- Taught as 1 of 5 Gestalt grouping families (alphabetical: Closure, Connectedness, Continuity, Proximity, Similarity).
- Core rule: tight gaps within groups, larger between; spacing always means something.

## Applies when / does not apply when
|Applies when|Overridden / limited when|
|---|---|
|Any layout: spacing carries meaning, intended or not|Enclosure (Common Region) or connectors (Uniform Connectedness) present: override spacing|
|Gap between clusters > gaps within them → separate groups seen|Likeness (Similarity) differs: overrides equal spacing|
|Placing secondary actions relative to task focus|Cues of different magnitude compete: winner depends on each cue's magnitude → make cues agree + test|
||Continuity present: trades off against proximity (1936 demonstrations)|

## Decision rules
- Nearness signals relatedness → people read shared traits or purpose into adjacent items; place accordingly.
- Gap ratios, not borders, = first grouping tool.
- Inter-group whitespace pays twice (visible clusters, easier skimming); spacing in general → content organized + grasped faster.
- If removing borders/cards → add whitespace to keep grouping (widen gaps between groups).
- If spacing uniform → color/shade forms groups → audit for accidental shading patterns.
- If whitespace alone cannot show belonging → border or background fill.
- If proximity cannot bind elements → line, arrow or shared frame; border also raises perceived priority, on top of separating + grouping.
- If placing optional/escape actions (Skip, Details) → near task, not in far corners.
- If content sits among ads → never give it ad dimensions.
- If list uses indicators → make them distinct in shape.
- If layout must parse easily → mimic real-object cues (occlusion, shared motion, closed contours).
- If offering decline/skip → same size, contrast + position as accept.
- If layout changes per breakpoint → check groupings survive every one.

## Why it works
Mechanism:
- Proximity needs no added structure → acts early; cheapest grouping cue.
- Distance = grouping cue: small gaps mean "together", large gaps "separate" → spacing alone conveys relationships + shared function.
- Gap ratio: space between clusters > space within them → separate groups seen.
- Once spacing sets grouping (e.g. row spaced 1/23/45/6, 1923 demonstration), alternatives become very hard to see, even if geometrically simpler.
- Enclosure + spacing trade off: bordered widgets can sit closer yet still read as separate.
- Task-focused users develop tunnel vision → miss anything far from work area.
- Unrelated items placed together camouflage each other: users inspect one item of perceived group + infer rest of group.

Origin:
- Formalized 1923 among Gestalt grouping principles (from Gestalt psychologists); Similarity formalized same year.
- 1923 statement covered proximity, similarity, good continuation + others; English excerpts appeared 1938.
- 1923 method: vary one factor (e.g. spacing), hold another (e.g. likeness) constant, pit them against each other to compare strength.
- Extensions appeared 1929, 1935, 1936 (1936 work in English 2006).
- Other grouping laws, dated: Prägnanz 1910; Common Region 1992 (late-20th-century addition, proposed as grouping principle); Uniform Connectedness 1994.
- Corrected Gestalt slogan: whole not "more than" sum of its parts but different from it.
- 1999 textbook grouping template: all else equal, elements w/ shared property tend to read as one higher-order unit.

## Evidence
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Closeness → grouping + assumed shared function|1923 statement of grouping principles|Theoretical perception principle; no single specific study; no person/study beyond 1923 formalization → attribute to Gestalt psychologists collectively|Treat spacing as meaning|
|72 circles read as one block of 36 on left + three blocks of 12 on right, by spacing alone|Classic figure|Illustrative demonstration, not study; say so when citing|Gap ratios form groups|
|36 equally spaced circles forming square, 18 dark + 18 light, read as six horizontal rows|↑|Illustrative demonstration, not study|Likeness overrides equal spacing; audit shading|
|Row normally grouped 1/23/45/6 by spacing seen as 12/34/56 once closed contours surround pairs|1992 perceptual demonstration (Common Region)|Demonstration|Enclosure overrides spacing|
|Connectors between pairs in 1/23/45/6 spacing flip grouping to 12/34/56, overriding spacing + likeness; connector need not touch elements|1994 perceptual demonstration (Uniform Connectedness, first called element connectedness)|Demonstration. Connectors can include arrows, shapes, frames, lines, color|Bind what proximity cannot w/ connector|
|Continuity trades off against proximity|1936 demonstrations|Demonstrations|Make cues agree|
|Probabilistic account of how dot patterns group by spacing + likeness → grouping has measurable structure|2008 quantitative modeling|Model|—|
|Edge co-occurrence in natural scenes forecasts contour grouping|2001 modeling|Model|Real-object cues parse most easily|
|Several participants missed how-to video sized like surrounding display ads|Instructional-video usability study|Qualitative observation, no sample size|Never give content ad dimensions|
|Distinct-shape list indicators → faster, more accurate finding; near-identical ones slowed scanning|Earlier list-indicator research|—|Make list indicators distinct in shape|
|Optional "Skip" link in top corner far from main calls to action missed → participants concluded account creation (signing in) mandatory|Case: mobile usability sessions|Qualitative observation, no sample size|Place escape actions near task|
|"click and hold for details" hint in distant lower corner → viewer decided episode list unreachable|Case: TV streaming app|Qualitative observation, no sample size|Keep hints near focus|
|Google Search landing page changed little since 1998 launch; flow = single auto-focused field, autocomplete, filters only after query, query kept visible, retrieval time shown, spaced result chunks, borders around videos + featured snippets|Case: Google Search|Rests on longevity + adoption, not study|Hick's Law, working memory, Doherty Threshold, chunking, proximity + connectedness combined in one flow|

## Misreadings and limits
- Wrong: ranking grouping cues by fixed strength ("connectedness always wins") (Gestalt laws) → Right: rankings come from demonstrations; winner depends on cue magnitude → make cues agree + test.
- Wrong: removing containers w/o adding space (Proximity, Common Region) → Right: enclosure + whitespace trade off → widen gaps between groups.
- Wrong: citing grouping laws as processing model → Right: whether inborn (Gestalt position: pattern-finding organizing rules built into mind from birth) or acquired from real-object statistics (1975 view) remains contested → cite as dependable descriptive tendencies.
- Wrong: citing demonstration figures (e.g. 72-circle figure) as controlled UX experiments → Right: most grouping evidence comes from demonstrations; say so.
- Wrong: citing Gestalt therapy as perceptual evidence → Right: separate field; argued to have no substantive relation to Gestalt perception research.
- Wrong: crediting Closure to 1994 connectedness paper → Right: this paper concerns connectedness.
- Wrong: merging Common Region + Uniform Connectedness as "draw a box around it" (practitioners often do) → Right: enclosure by boundary/fill vs connector or continuous link.
- Limit: many tight clusters make layout busy even if each cluster coherent.
- Limit: stacked full-bleed enclosed rows (often mobile styles left unchanged on wide screens) make every block look equally important → users toggle between scanning + reading.
- Limit: evidence of distant/look-alike elements missed (Skip link, TV hint, how-to video) = qualitative usability observations w/o sample sizes.

## Check questions
|Question|Look for|Laws|
|---|---|---|
|Related items closer to each other than to unrelated items?|Uniform spacing; labels equidistant from two fields; gaps contradicting meaning|Proximity|
|Groupings survive every breakpoint?|Stacked columns splitting related items or merging unrelated ones|Proximity|
|Optional + escape actions near task?|Skip, Details or other secondary actions in far corners|Proximity (tunnel vision)|
|All grouping cues agree on one partition?|Spacing saying one group while color or boxes say another|Proximity, Similarity, Common Region|

## Symptoms → fixes
|Symptom|Likely cause|Fix|
|---|---|---|
|Labels seem to belong to wrong field|Proximity|Each label nearer its own field than its neighbors; enlarge gaps between groups|
|Optional Skip missed; account creation believed mandatory|Escape action far from task (tunnel vision)|Place escape actions near task|
|Content (e.g. how-to video) missed among display ads|Content sized like surrounding ads|Never give content ad dimensions|
|Grouping lost after cards/borders removed|Enclosure taken away w/o added space|Widen gaps between groups|
|Unintended groups appear in evenly spaced grid|Accidental color/shade pattern|Audit shading; make cues agree|
|List slow to scan|Near-identical list indicators|Indicators distinct in shape|

## Hypothetical examples
- Hypothetical (space makes units): train-booking results list leaves generous space around each itinerary → departure, changes + fare read as one unit + list skims easily.
- Hypothetical (action buried among unrelated buttons): workplace video-call screen tucks "Share agenda" into bottom bar beside Mute, Camera, Leave; reads as one more call control + gets missed.
- Hypothetical (grouping lost at a breakpoint): pharmacy product page shows "Dosage" + "Side effects" links side by side on desktop; on phone second drops far below long description + easy to miss.
- Hypothetical (heading owns its text): workplace-tool employee handbook sets each heading tight to its paragraph w/ wider gap above → heading never seems to close previous section.
- Hypothetical (indentation nests): smart-home app lists each room w/ its devices indented beneath.

## Humane bound
- No abuse case recorded; general influence-vs-manipulation test applies.
- Recorded failures accidental: unrelated items placed together camouflage each other; optional Skip far from main actions missed → account creation believed mandatory.
- Bounded by ../principles/empowering.md: decline + skip options get same size, contrast + position as accept.
- Bounded by ../principles/transparent.md: grouping must not mislead.
- Read: ../patterns/defaults-and-choice-architecture.md (equal-weight No); ../ethics/influence-vs-manipulation.md; ../patterns/layout-grouping-and-hierarchy.md.

## Related
- common-region.md: enclosure overrides spacing; enclosure + whitespace trade off.
- similarity.md: likeness overrides equal spacing.
- uniform-connectedness.md: connectors override spacing + likeness.
- fittss-law.md: distance from task also costs movement.
- [Gestalt grouping principles overview](gestalt-principles-overview.md): shared background of five perception laws; how cues combine + compete.
- ../patterns/layout-grouping-and-hierarchy.md: patterns for grouping cues, spacing, containers, emphasis, reading order; applies this law.
- ../patterns/forms-and-data-entry.md: applies label-to-field distance.
- ../patterns/search-and-results.md: pattern file applying this law.
- ../methods/gestalt-layout-pass.md: lay out screen by grouping cues before styling.
- ../guides/laws-and-principles-crosswalk.md: humane principle bounding this law.
