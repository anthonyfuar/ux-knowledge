# First impressions and aesthetics

## Scope + laws behind these patterns
- Use for: usability patterns on visual polish: what attractiveness buys + hides.
  - Buys: leniency toward small flaws · design judged easier to use · favourable reaction.
  - Hides: real usability problems · weak legibility.
- Applies when: designing/reviewing visual design, colour + contrast, typography or high-stress screens, or reading test sentiment on polished interface.
- Laws underneath:
  - ../laws/aesthetic-usability-effect.md.
  - [Prägnanz](../laws/pragnanz.md): simple forms eye resolves easily.
  - ../laws/cognitive-load.md.
  - ../laws/occams-razor.md.

### Shipping a user-facing surface: invest in visual quality?
- When: shipping any user-facing surface.
- Do: make it attractive; pleasing, unobtrusive typography (grouping + hierarchy → layout-grouping-and-hierarchy.md).
- Why: Aesthetic-Usability Effect: good looks → favourable reaction → small flaws excused + design seems easier to use. Prägnanz: if eye can boil composition down to plain wholes → sticks in memory more readily + less effort to perceive.
- Hypothetical: council bin-collection page: one clear calendar block + calm type, not dense date table.

### Reading a test of a polished interface: does good sentiment mean usable?
- When: usability test or review of polished design.
- Do: in reviews separate "looks good" from "works well"; observe task success, not only satisfaction ratings. Polish may inflate sentiment → ../methods/debiasing.md.
- Misreading: Wrong: good sentiment in usability test = proof of usability → Right: not proof.
- Why: in tests polish can hide real problems, since participants grow more forgiving.
- Evidence: 1995 ATM interface study: perceived ease of use tracked aesthetic ratings more closely than actual ease of use did.
- Hypothetical: polished insurance-claim prototype scores well on satisfaction; review still counts how many participants finished receipt upload before calling it usable.

### Choosing text + background colours: does the pair pass?
- When: any text/background colour pair.
- Do:
  - Check every pair against WCAG AA contrast for its size.
  - Accent colours that cannot reach required contrast → only large type/decoration.
  - Small text → neutral surface passing contrast.

|Element|AA contrast|
|---|---|
|Body text|4.5:1|
|Large text, icons, input borders, focus indicators, chart marks|3:1|

- Large text (for contrast) = ~24 px regular / 19 px bold.
- Caveat: colour passing as heading can fail as caption.
- Misreading: Wrong: aesthetic-usability effect excuses low contrast → Right: never excuses low contrast.
- Case: 2021 redesign: many card colours failed AA contrast w/ light text → brightness + saturation tweaks fixed heading contrast; small descriptions moved onto one shared dark background.
- Hypothetical: transit app's line colours stay on route badges + large line names; timetable small print on neutral panel passing contrast.

### High-stress screen: how should it look?
- When: stress high: urgent bookings, error recovery, emergencies.
- Do: calm, pleasant presentation.
- Why: positive affect keeps thinking broad enough for problem-solving; stress narrows it.
- Hypothetical: banking app's card-blocked screen: soft colour, plain heading + one next step, not red alarm styling.

### Wanting an engaging feel: which colour + type choices?
- When: aiming for engaging feel.
- Do: non-grayscale colour schemes; one consistent body typeface.
- Evidence: site colour scheme study: pure black-on-white/white-on-black sites rated less pleasing + less stimulating.
- Hypothetical: school-portal redesign: pure black-on-white → tinted palette w/ one body typeface across pages.

### Polish over a real problem: let it stand?
- When: attractive design over findability/task-blocking problem.
- Do: fix problem; count on goodwill only for minor issues.
- Avoid: polish covering findability/task-blocking problems.
- Limit: attractiveness goodwill only buffers minor issues.
- Hypothetical: elegant hotel site w/ booking button hidden below photo carousel still needs button moved, however good it looks.

## Related
- layout-grouping-and-hierarchy.md: grouping cues, spacing, emphasis + reading order behind simple compositions.
- inclusive-and-accessible-design.md: accessibility floors visual style must not undercut.
- dashboards-and-data-displays.md: chart colour on dense data screens.
- errors-and-input-tolerance.md: error recovery = high-stress moment needing calm presentation.
- memorable-moments-and-endings.md: peaks + endings, other emotional side of experience.
- ../methods/debiasing.md: countering bias in studies + reviews; open when polish may inflate test sentiment.
- ../ethics/using-psychology-responsibly.md: guardrails for every psychological lever, attractiveness included.
- transparency-and-honesty.md: honesty tests; humane bound on polish hiding what matters.
- ../laws/aesthetic-usability-effect.md: law behind leniency toward attractive designs.
- [Prägnanz](../laws/pragnanz.md): simple forms eye resolves easily.
