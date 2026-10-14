# Law of Similarity

## In one line
Separation = no barrier to grouping by likeness: look-alikes spread far apart still read as one form, set or overall image. → Body text one look, links / navigation another, never confusable w/ it; audit accidental look-alikes (they create false groups).

- Theme: Perception. Classed as effect / principle.
- Aliases: similarity principle; Gestalt principle of similarity.
- Gestalt grouping usually taught as 5 families; this law = one, beside Closure, Connectedness, Continuity + Proximity.
- Most affected: link + button styling vs body text, consistent component styling, accidental look-alikes.

## Applies when / does not apply when

|Situation|Similarity?|Cite instead / also|
|---|---|---|
|Any look-alike elements, page-wide + across distance, incl accidental resemblance|Yes|—|
|Links / buttons styled as text, or non-clickables as links|Yes|von-restorff-effect.md for one standout primary|
|Consistent styling of conventions|Yes|jakobs-law.md|
|Grid of look-alike cards hard to compare|No: uniform cards correctly read as one content type|cognitive-load.md + working-memory.md (comparing across cards); not selective-attention.md|
|Recognizing object across rotation, position, scale|No: called 'invariance'|—|
|Spacing vs likeness conflict|Both: grouping turns ambiguous|proximity.md|
|Items proximity cannot group|Add connector / frame|uniform-connectedness.md, common-region.md|
|Gestalt therapy claims|No: separate field, argued to have no substantive relation to Gestalt perception research|Never cite as perceptual evidence|

## Decision rules

### Separate what behaves differently
- Plain text never mistakable for link / navigation: give those own look.
- One visual treatment → one behavior; look-alikes assumed to behave alike.
- Assume elements w/ shared looks read as linked: people infer one set, probably same job or same meaning. Triggering cues: size, color, movement, shape, orientation.
- Never give content ad dimensions.
- Indicators: distinct shapes.
- If controls sit in busy linework / matching styles → can vanish → make them unlike surround.
- Escape actions (e.g. optional skip) near task.

### Audit for false groups
- Audit layouts for accidental resemblance between elements.
- If spacing uniform → color / shade forms groups → audit accidental shading patterns.
- Icon sets: fine line between consistent set + falsely implying specific icons related. If icons share shape → users skip labels + small differences.

### Grids + tiles
- Identical grids hide clickability + destination → add affordance cues.
- If tile size varies by importance → can blur whether items still one type → add labels / affordances.

### Combine cues
- Gap ratios, not borders, = first grouping tool.
- If proximity cannot group items → bind w/ line, arrow or shared frame.
- Make all cues agree on one partition, then test; do not rely on fixed cue rankings.
- Stack shared attributes + let proximity point same way → stronger grouping.
- Layouts mimicking real-object cues (occlusion, shared motion, closed contours) parse most easily.

## Why it works

Mechanism:
- Shared visual attributes = evidence of group membership, override physical separation → users infer shared meaning / function.
- Attributes driving similarity grouping: lightness, color, size, orientation, shape, texture, font treatment, motion.
- Color tends to dominate shape as similarity cue.
- Works page-wide → one item can belong to spatial group + similarity group at once.
- Several shared attributes + same-direction proximity strengthen grouping.
- Uniform spacing → likeness decides. Similarity + spacing pointing to different groups → ambiguous grouping.
- Head-to-head, similarity loses to proximity or enclosure, but = most resilient cue bc it works page-wide.
- Grid of identical boxes reads as equal variants of one content type.
- Connectors: need not touch elements to group them; include arrows, shapes, frames, lines + color.
- Border raises perceived priority, separates + groups.

Origin, dated:
|When|What|
|---|---|
|1910|Prägnanz named|
|1923|Similarity formalized as one of Gestalt grouping principles; Proximity in same statement (w/ good continuation + others)|
|1923|Method: vary one factor (e.g. spacing), hold another (e.g. likeness) constant, pit them against each other → compare strength|
|1926|Perception experiment on hidden (embedded) figures|
|1938|English excerpts of 1923 statement|
|1975|View: grouping learned from real-object statistics|
|1990, 1994|Classic usability heuristics (revised 1994); Consistency and standards links to Jakob's Law + Similarity|
|1992|Common Region formalized|
|1994|Uniform Connectedness formalized (first named 'element connectedness')|
|2001, 2008|Quantitative grouping models (see Evidence)|

- Gestalt position: rules sorting input into patterns = inborn, not acquired. Inborn vs learned from real-object statistics (1975 view) = contested.

## Evidence

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Look-alikes group even when far apart|Theoretical perception principle; no single specific study; traces to 1923 formalization|Attribute to Gestalt psychologists collectively|Style body text vs links distinctly; audit accidental resemblance|
|72 circles: spacing alone groups them into one block of 36 (left) + three blocks of 12 (right)|Classic figure|Illustrative demonstration, not study|Gap ratios first|
|36 equally spaced circles in square, 18 dark + 18 light, seen as six horizontal rows|↑|Illustrative demonstration, not study|Likeness overrides equal spacing → audit shading|
|Visible connector → items judged more closely related|1994 perceptual demonstration ('element connectedness')|Perceptual demonstration|Bind w/ line, arrow, frame|
|Connectors joining pairs in 1/23/45/6 spacing flip grouping to 12/34/56, overriding spacing + likeness|1994 perceptual demonstration|↑|Connectors can override other cues|
|Probabilistic model explains dot-pattern grouping by spacing + likeness|2008 model|Quantitative modeling|Grouping has measurable structure|
|Edge co-occurrence statistics in natural scenes forecast contour grouping|2001 modeling study|↑|Mimic real-object cues|
|Simple figure embedded among added lines → practically invisible however hard one attends, unless recolored to differ from surround (camouflage by regrouping)|1926 perception experiment on hidden figures|No caveat stated|Controls unlike busy surround|
|Several participants missed how-to video in right column, sized exactly like surrounding display ads|Instructional-video usability study|Qualitative, no sample size|Never give content ad dimensions|
|Optional Skip link far from main actions missed → users believed sign-in required|Mobile usability observation|Qualitative, no sample size|Escape actions near task|
|Detail hint in far corner missed → users thought episode list unreachable|TV app usability observation|Qualitative, no sample size|Hints + escape actions near task|
|Distinct indicator shapes → faster, more accurate finding; near-identical shapes slowed scanning|Earlier list-indicator research|Details not stated|Distinct indicator shapes|

Caveat for all: most grouping evidence = demonstration figures, not controlled UX experiments; say so when citing one, e.g. 72-circle example.

## Misreadings and limits
- Wrong: rank grouping cues by fixed strength (e.g. 'connectedness always wins'). → Right: rankings come from demonstrations; winner depends on each cue's magnitude; make cues agree + test.
- Wrong: vary tile size for importance w/ no other cues. → Right: blurs whether items still one type; add labels / affordances.
- Wrong: blame hard-to-compare card grid on Similarity. → Right: uniform cards correctly read as one type; cite Cognitive Load + Working Memory.
- Wrong: equate similarity w/ 'invariance'. → Right: invariance = recognizing object across rotation, position + scale.
- Wrong: credit Closure to 1994 work. → Right: 1994 work concerns connectedness.
- Wrong: merge Common Region (enclosure by boundary / fill) w/ Uniform Connectedness (connector / continuous link) as 'draw a box around it', as practitioners often do. → Right: keep distinct.
- Wrong: cite Proximity / Similarity to one specific study. → Right: none beyond 1923 formalization; attribute to Gestalt psychologists collectively.
- Wrong: present grouping laws as processing model. → Right: innate vs learned = contested; cite as reliable descriptive tendencies.
- Wrong: cite Gestalt therapy as perceptual evidence. → Right: separate field.

Limits:
- Interactive elements resembling plain text → grouped w/ text + missed.
- Works across distance → accidental resemblance creates unintended groups.

## Check questions
Tag [A] = answerable from artifact itself (see ../checklists/usability-review.md).

|Check|Look for|Law / principle|Tag|
|---|---|---|---|
|All grouping cues agree on one partition?|Spacing saying one group while color / boxes say another|Proximity, Similarity, Common Region|[A]|
|Static text + interactive elements impossible to confuse?|Links / navigation styled as body copy; non-clickables styled as links (false groups even at distance)|Similarity|[A]|
|Each visual treatment maps to one behavior?|Decorative icons in link / CTA color; several different actions in one style; one icon for different categories|Similarity|[A]|

## Symptoms → fixes

|Symptom|Likely cause|Fix|
|---|---|---|
|Links or buttons missed|Similarity, Von Restorff Effect|Interactive elements unlike text; one standout primary action|
|Charts misread / series confused|↑|One color per metric across all charts; color-blind-safe categorical palette; direct labels, not legends; one accent color for key series|
|Grid of look-alike cards hard to compare|Cognitive Load + Working Memory (comparing across cards), not Similarity, not Selective Attention|Show deciding attributes (price, rating, key spec) consistently; add sort + filters|

## Hypothetical examples
- Hypothetical: tax-authority help page: body copy plain dark text, links underlined in distinct color, side navigation in tinted panel → no text mistaken for link.
- Hypothetical: home-energy dashboard's decorative lightning-bolt graphic in same accent color as its tappable tiles → residents tap graphic expecting it to open something.
- Hypothetical: flight seat-selection screen styles Confirm seat, Change flight + Add bag in one identical outline → travellers hunt for primary action; Confirm also far from seat map → added Fitts's Law cost.
- Hypothetical: patient portal reuses calendar icon for both Appointments + Bill due dates → patients assume bills live in appointments area.
- Hypothetical: banking app shows Pending + Completed transfers as same grey rounded tag, differing only in one small word → shared shape implies one status family; customers may skip distinguishing word.
- Hypothetical: city transit app: route lines = colored round badges, service alerts = triangular tags → riders never mistake alert for route.

## Humane bound
- No abuse case recorded; only accidental false groups: non-clickables styled as links, icon set falsely implying specific icons related, how-to video sized like display ads + missed.
- Same cue used deliberately against people = disguised ads: ads styled as content, navigation or download buttons → see ../ethics/deceptive-patterns.md.

|Principle|Bound on Similarity|Read|
|---|---|---|
|../principles/transparent.md|Ads must read unmistakably as ads|../patterns/transparency-and-honesty.md (make ads unmistakably ads)|
|../principles/inclusive.md|Color-signalled groups need accessibility floors, e.g. color-blind-safe palette|../patterns/inclusive-and-accessible-design.md (chart fix: color-blind-safe palette)|

## Related
- proximity.md: same-direction proximity strengthens similarity; proximity wins head-to-head; under uniform spacing likeness decides.
- von-restorff-effect.md: deliberately breaking similarity; shares missed-links + misread-charts fixes.
- jakobs-law.md: consistent styling of conventions.
- gestalt-principles-overview.md: shared background of 5 perception laws + how cues combine + compete.
- common-region.md, uniform-connectedness.md, [Prägnanz](pragnanz.md): sibling grouping laws.
- cognitive-load.md, working-memory.md: cite for hard-to-compare card grids.
- fittss-law.md: distance cost when primary action far from its field.
- ../checklists/usability-heuristics-map.md: Consistency and standards links to Jakob's Law + Similarity.
- ../checklists/usability-review.md: meaning of [A] tag.
- ../methods/gestalt-layout-pass.md: lay out screen by grouping cues before styling.
- ../guides/laws-and-principles-crosswalk.md: humane principle bounding law.
- ../patterns/navigation-and-menus.md, ../patterns/layout-grouping-and-hierarchy.md, ../patterns/dashboards-and-data-displays.md: apply law.
- ../patterns/transparency-and-honesty.md, ../patterns/inclusive-and-accessible-design.md, ../ethics/deceptive-patterns.md: humane bound + misuse side.
- ../principles/transparent.md, ../principles/inclusive.md: principles bounding it.
