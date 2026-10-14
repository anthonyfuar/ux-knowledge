# Law of Common Region

## In one line
Items inside one bounded area seen as one group; shared boundary = belonging together. Use when set must read as related + spacing alone cannot say so.
- Aliases: principle of common region; one of Gestalt grouping principles. Class: effect / principle. Theme: Perception (perception + grouping).
- Reaches furthest into: card + panel containers, section backgrounds, form-field grouping.

## Applies when / does not apply when
|Add enclosure when|Hold back when|
|---|---|
|whitespace alone cannot express grouping|spacing already works (check first)|
|group mixes element types|border added "just in case"|
|group must say: related to each other, not to neighbours|testing has not shown confusion w/o border|

Scope note: Common Region = enclosure by boundary or fill. Uniform Connectedness = connector or continuous link. Practitioners often merge both as "draw a box around it"; keep apart when choosing + citing.

## Decision rules
- To show elements related → border or background fill around them.
- Either cue alone builds common region, for single element or whole set: own fill behind area, or outline around it.
- Enclosure payoff: layout organization becomes visible → quick reading of what belongs w/ what, element to element + section to section.
- Background color can also split interface chrome from content: sticky headers, footers, sidebars.
- Before adding border → ask: spacing alone enough? testing shown confusion w/o it?
- If containers removed → widen gaps between groups; enclosure + whitespace trade off.
- Draw boundaries only around real groups: enclosure overrides proximity + similarity (two close dots in different boxes read as separate) → misplaced boundary actively breaks real groups.
- Avoid full-width contrasting bands above continuing content: act as false floor → users think page ended + stop scrolling.
- Avoid borders "just in case": each adds visual processing work.
- If several grouping cues in play → make all agree on one partition + test; never rely on fixed cue-strength ranking.

## Why it works

### Mechanism
- One sharply drawn enclosure around set → everything inside reads as belonging together.
- Bounded area = container; pattern-seeking perception treats its contents as one unit → relationships easy to read.
- Grouping comes from boundary/background, not distance; border or fill alone enough.
- General template for grouping principles (1999 textbook): all else equal, elements w/ shared property tend to read as one higher-order unit.

### Origin
- Perception + grouping laws from Gestalt psychologists; Proximity + Similarity formalized 1923; Prägnanz as named principle dates from 1910.
- Common Region proposed as separate grouping principle in 1992, inside Gestalt grouping tradition: late-20th-century addition.
- Uniform Connectedness proposed as grouping principle in 1994.

## Evidence
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Dots spaced 1/23/45/6 (spacing alone groups them so) seen as 12/34/56 once closed contours surround pairs|1992 perceptual demonstration|demonstration figure, not controlled UX experiment|enclosure beats spacing → boundaries must match real groups|
|Grouping cues in general|most evidence = demonstration figures, not controlled UX experiments|say so when citing, e.g. 72-circle example|treat as dependable tendencies; test real layouts|
|Grouping laws innate (Gestalt view) or learned from real-object statistics (1975 view)?|theoretical debate|contested|cite as reliable descriptive tendencies, not as model of how processing works|

Citation caveats:
- Proximity + Similarity: no specific origin beyond 1923 grouping formalization → attribute to Gestalt psychologists collectively.
- Do not credit Closure to 1994 paper proposing Uniform Connectedness; that paper concerns connectedness.
- Gestalt therapy = separate field, argued to have no substantive relation to Gestalt perception research → never cite as perceptual evidence.

## Misreadings and limits
- Wrong: rank Gestalt grouping cues by fixed strength (e.g. "connectedness always wins") → Right: such rankings come from demonstrations + winner depends on each cue's strength; make cues agree + test.
- Wrong: strip containers w/o adding space (Proximity, Common Region) → Right: enclosure + whitespace trade off; widen gaps between groups when containers go.
- Wrong: Common Region = reason to add borders/cards just in case → Right: check whether spacing already works; extra borders add visual processing.
- Wrong: Common Region + Uniform Connectedness = same "box" → Right: boundary/fill vs connector/continuous link.
- Limit: enclosure overrides proximity + similarity → misplaced boundary breaks real groups.
- Limit: full-width contrasting band can create false floor → people stop scrolling.

## Check questions
- Bounded areas (borders, fills) match real groupings? Look for: cards/panels enclosing unrelated things, or related things split across containers.
- No false floors? Look for: full-width contrasting bands above content continuing below the fold.
- All grouping cues (Proximity, Similarity, Common Region) agree on one partition? Look for: spacing saying one grouping while color/boxes say another.
- For each new border: spacing alone enough? testing shown confusion w/o it?
- Where containers removed, gaps between groups widened?

## Symptoms → fixes
|Symptom|Likely cause (laws)|Fix|
|---|---|---|
|Layout reads as undifferentiated clutter|Chunking, Common Region, Prägnanz|evident hierarchy, dividers, modules w/ backgrounds/borders|
|Settings page w/ dozens of toggles hard to scan|Cognitive Load, Chunking, Common Region, Tesler's Law via progressive disclosure, Pareto Principle (check usage w/ analytics); not Choice Overload|task-based labelled groups; search across setting names, synonyms + descriptions; advanced settings behind disclosure|
|Users stop scrolling early|full-width contrasting band = false floor (Common Region)|no full-width contrasting band above continuing content|
|Related items read as separate|misplaced boundary overriding proximity + similarity (Common Region)|redraw containers around real groups|

## Hypothetical examples
- Hypothetical (container sets meaning): bank transfer screen: same figure reads as amount to send inside Payment box + as daily cap inside Limits box.
- Hypothetical (media + text as one unit): patient portal boxes each scan thumbnail w/ its clinician note → no note read as belonging to next scan.
- Hypothetical (rows vs columns): train timetable tints alternate rows so each departure reads across, while plain gaps keep columns apart.
- Hypothetical (cards resolve ambiguity): online course catalogue grid leaves tutor names + ratings floating between neighbouring courses until each course gets own card.
- Hypothetical (border + tint): smart-home app draws one rounded border around room's temperature, humidity + schedule readouts; staff timesheet tool gives approve + reject actions own shaded panel.
- Hypothetical (spacing suffices): travel booking app's passenger-details step separates each traveller's block w/ heading + generous gaps, no box around each block, + still reads clearly.

## Humane bound
- No recorded case of Common Region turned against people; general influence-vs-manipulation test applies.
- Recorded failures accidental: misplaced boundary breaks real groups; full-width contrasting band acts as false floor → people think page ended + stop scrolling.
- Bound by Transparent: grouping + styling must not mislead.
- Further reading for this bound: using psychology responsibly; content layout, grouping + visual hierarchy patterns.

## Related
- proximity.md: enclosure overrides spacing as well as likeness; enclosure + whitespace trade off.
- similarity.md: enclosure overrides likeness as well as spacing.
- uniform-connectedness.md: works via connector/continuous link; keep distinct from enclosure by boundary/fill.
- gestalt-principles-overview.md: shared background of five perception laws + how grouping cues combine + compete.
- chunking.md: shares undifferentiated-clutter + settings-page fixes.
- [Prägnanz](pragnanz.md): shares undifferentiated-clutter fix.
- cognitive-load.md: leading law for settings-page symptom.
- teslers-law.md: progressive disclosure in settings-page fix.
- pareto-principle.md: checking setting usage w/ analytics.
- ../patterns/layout-grouping-and-hierarchy.md: grouping cues, spacing, containers, emphasis + reading order; also further reading on humane bound.
- ../patterns/forms-and-data-entry.md: applies form-field grouping by common region.
- ../patterns/complexity-management.md: applies Common Region.
- ../methods/gestalt-layout-pass.md: lays out screen by grouping cues before styling.
- ../principles/transparent.md: principle bounding Common Region.
- ../ethics/using-psychology-responsibly.md: further reading on humane bound.
- ../ethics/influence-vs-manipulation.md: general test applying here.
- ../guides/laws-and-principles-crosswalk.md: names humane principle bounding Common Region.
