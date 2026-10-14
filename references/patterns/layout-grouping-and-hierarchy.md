# Layout, grouping and hierarchy

## Use when
- Covers arranging on-screen content: modules, grouping cues, one treatment per behaviour, spacing scale, section boundaries, co-location, reading path, salience, readable text, ad-like regions, icon labels.
- Open when laying out / reviewing: page, dense screen, long-form copy, visual styles / icon set.
- Laws in play: Chunking, Law of Proximity, Law of Common Region, Law of Similarity, Law of Uniform Connectedness, Law of Prägnanz, Cognitive Load, Selective Attention, Von Restorff Effect.

### How to structure a dense screen? (modularize the page)
- When: data-packed screens, e.g. dashboards + data-heavy pages.
- Do: separate sections w/ rules / dividers, make importance order plain + let each module stand apart from neighbours; structure serves how people size up on-screen content.
- Avoid: grouping w/o hierarchy → weakens chunking.
- Why: Chunking.
- Hypothetical: airport operations screen splits gates, delays + staffing into ruled modules, each under clear heading, ranked by size.

### Which grouping cue fits the job?
- When: deciding how items show they belong together, apart or in order.
- Do: pick cue to fit job; each Gestalt cue has own use + technique:

|Cue|Use to|Technique|Avoid / limit|Law|
|---|---|---|---|---|
|Proximity|signal "together" vs "separate" through distance alone|tight gaps within group, larger between groups; whitespace does double duty|—|Law of Proximity|
|Common region|make obvious section container|border / background fill behind set|—|Law of Common Region|
|Similarity|tie separated items to one meaning|match motion or orientation, size, shape or colour|—|Law of Similarity|
|Uniform connectedness|stress relationship / add context|arrows, connectors, frames, lines, shared colour|—|Law of Uniform Connectedness|
|Prägnanz|easy-to-read shapes + compositions|plain forms; recall + perception both cope w/ them more easily|—|Law of Prägnanz|
|Continuity|show membership + order|shared axis aligns items into one group, broken alignment separates; sequence via visible / implied line (numbered steps, arrows); eye paths w/o abrupt turns|—|—|
|Common fate|bind items through motion|related items move same direction w/ same timing + easing; unrelated items stay still|synchronized motion of unrelated items implies relationship → motion only to carry meaning|—|
|Closure|imply shapes + containers|partial lines, whitespace, cropping, dashed borders; controls inside busy line work dissimilar in colour / weight so line work does not absorb them|implied shapes clashing w/ familiar symbols|—|
|Figure-ground|functional content on top layer|strong contrast, clear size difference, shadow / elevation for floating elements (menus, cards, modals); controls small, enclosed + convex|low-contrast pairs (red on blue, red on grey); equal-weight regions → figure + ground flip; ambiguous figure-ground only for logos + art|—|

- Origin: Gestalt school premise → people arrive in world already inclined to sort what they sense into patterns.
- Five families cover Gestalt grouping principles, sorted by cue relied on: placement (proximity = position; continuity = path eye follows) · look (similarity = shared appearance) · structure (connectedness = drawn link; closure = shape mind completes).
- Hypothetical (continuity): hospital discharge checklist aligns each section's items on one left edge under its heading; item shifted off shared edge reads as belonging elsewhere.
- Hypothetical (common fate): map app: place labels slide in step w/ map when panned while toolbar stays still.

### Do groupings hold, with no accidental ones, at every breakpoint?
- When: checking any layout, esp. across screen sizes.
- Do: related items closer to each other than to anything else. Re-check groupings at every breakpoint. Breakpoint cannot keep needed gap → move element elsewhere.
- Avoid: accidental resemblance / closeness → unintended groupings. Mobile row stacks unchanged on wide screens: stacked full-bleed enclosed rows flatten importance + slow scanning.
- Why: Law of Proximity.
- Hypothetical: train-booking form's "return journey" toggle loses gap separating it from "add railcard" link on narrow phone layout → moves down beside date fields.
- Hypothetical: clinic booking page: each doctor's photo + "book" button share one card on desktop; on mobile button drops below next doctor's photo + reads as next doctor's.

### How to style links, buttons, icons and badges? (one visual treatment, one behaviour)
- When: defining link, button, icon + badge styles.
- Do: interactive colour only on interactive elements, not keywords, headings / decorative icons. Primary call-to-action colour not shared w/ secondary buttons. Same-shape badge types differ by both colour + glyph. Distinct icon per category.
- Avoid: decorative elements styled like controls. Several different actions in one identical style. Near-identical icons for different things.
- Cases: red decorative icon above red upload button looked clickable. Identical green Submit, Cancel + Add Attachment buttons → users hunted for Submit.

### How should spacing carry structure? (spacing scale + text levels)
- When: setting typographic levels + spacing.
- Do: systematic gaps between typographic levels (heading → body, section → section) → spacing, not only size, carries structure. Heading nearer own text than section above. Indent nested list items. Each text level own treatment. Pull quote set deliberately outside text structure flags one line as special.
- Avoid: uniform spacing + styling → content becomes flat set of equals.
- Hypothetical: council's planning-application page: heading close above its paragraph, wide gap before next section, nested conditions indented.

### Will people see there is more below? (section boundaries on long pages)
- When: long pages.
- Do: visual continuity across section boundaries → evident more content lies below.
- Avoid: false floor = full-width, high-contrast horizontal band above important content → reads as page end → people stop scrolling.
- Hypothetical: insurance policy page lets next section's heading peek above fold, not dark full-width band.

### Where does the explanation go? (co-location)
- When: label, value, explanation / chart legend needed to understand another element.
- Do: place info needing integration together → merged before reader moves on. Spatial content as picture, not words.
- Avoid: cross-screen references, footnote-style legends, help text far from its field → split-attention effect → re-reading + shallow understanding.
- Hypothetical: tax form shows hint for "taxable allowance" directly under field, not in help panel at page foot.

### Where does the key fact go? (in the reading path)
- When: people must find key fact, date, price / instruction on page / pop-up.
- Do: key fact inside area currently read, next to text discussing it. Also helps screen-magnifier users seeing only small part of screen at a time.
- Avoid: relying on large type / corner label outside reading region to pull eye → readers have tunnel vision on area they read. Judging salience from designer's own view of screen.
- Case: test of timeline pop-up showing year in large type top left: participant missed year + found it only in last line of body text.

### How to make the critical item stand out? (salience by removing)
- When: dense tables, alert lists, dashboards.
- Do: first strip decorative generic icons + graphics → quieter surroundings let critical value / alert stand out. Alerts point at exact region needing action.
- Avoid: adding more colour + weight everywhere → when everything emphasized, emphasis fails.
- Why: Von Restorff Effect.
- Hypothetical: pharmacy stock table drops category icons; the one expired batch then shows in single accent colour, its alert pointing at batch's row.

### Which elements stay? (strip non-contributors)
- When: reviewing any screen.
- Do: test each element against user's goal; failing layouts, ornament, imagery + colour → go. Keep only necessary + relevant elements.
- Avoid: simplifying past point where clarity suffers.
- Why: Cognitive Load. Each element kept on screen claims working memory as extraneous load.

### How to keep long copy easy to read? (readable type)
- When: long-form + instructional copy.
- Do:
  - Each line + copy as whole at sensible length; split under true headings.
  - Readable, not merely legible: unobtrusive design, effortless type, suits content + pleases eye. Understanding rises as distraction falls.
  - Sentence case for running text; capitals only for short labels. Why: all-caps words form uniform rectangles + most letter-identifying features sit in upper halves.
  - Familiar vocabulary. Why: unfamiliar terms shorten eye's jumps + slow reading.
  - Sizes, spacing + contrast surviving unknown conditions (bright sun, reading from across room), not only designer's own screen.
- Avoid: treating passed contrast check as readability. Readability = people want to read + can read comfortably.

### Will real content be mistaken for an ad? (keep out of ad territory)
- When: placing real content, promotions + callouts.
- Do: important content consistent w/ surroundings; signal importance via position + hierarchy. Usability-test anything important placed in top banner / right rail.
- Avoid: styling real content ad-like (never). Placing real content in ad regions / conventional ad slots (never; banner blindness). Boxed, coloured, animated or image-with-embedded-text treatments for real content.
- Why: hot-potato pattern = one irrelevant item in region → people abandon whole region.
- Case: mobile product site: installation-information section w/ background standing out from white page → taken for ad, scrolled past.

### Does this icon need a label? (label icons)
- When: icons, esp. navigation icons.
- Do:
  - Only a few near-universal icons may go unlabelled + only in context: home, search (magnifying glass), print, close, play, pause.
  - All others → visible text label, incl. menu, share + reply: share + reply sometimes on lists of universal icons, but meaning varies by product.
  - Labels always shown, not on hover. Why: hover-only labels add interaction cost + fail on touch screens.
  - Label restyled standard icons too.
  - No fitting icon in mind within ~5 seconds → use word.
  - Draw icons as schematic glyphs.
  - Test recognition: ask people what each icon should do. Test memorability: ask same people again after a couple of weeks.
- Avoid: reusing well-known icon for different behaviour. Heart + star icons compete for favourite, save, feature + rate; meanings vary by product.
- Why: cognitive load rises w/ icons: people must work out meaning + it may stick poorly in memory. Obscure icon = unused feature.
- Evidence: 2014 usability study tested main-navigation clock icon opening recently visited pages: every participant recognized clock, but not one clicked it.

## Related
- ../methods/gestalt-layout-pass.md: step method laying out screen by grouping cues before styling.
- ../laws/gestalt-principles-overview.md: shared background of perception laws; how grouping cues combine + compete.
- dashboards-and-data-displays.md: dense data screens, chart colour, comparison + prioritisation.
- calls-to-action-and-touch-targets.md: button hierarchy, target size, spacing + placement for controls styled here.
- ../methods/lightening-mental-effort.md: steps cutting extraneous load once non-contributing elements found.
- inclusive-and-accessible-design.md: accessibility floors contrast, text + icon choices must meet.
- calm-technology-and-device-etiquette.md: humane bounds on emphasis: peripheral attention + quiet signalling.
- ../ethics/deceptive-patterns.md: named deceptive patterns + honest alternatives; check emphasis + styling do not mislead.
- ../laws/chunking.md · ../laws/proximity.md · ../laws/common-region.md · ../laws/similarity.md · ../laws/uniform-connectedness.md · [Law of Prägnanz](../laws/pragnanz.md): grouping laws behind cue table.
- ../laws/cognitive-load.md · ../laws/selective-attention.md · ../laws/von-restorff-effect.md: load, attention + salience laws in play.
