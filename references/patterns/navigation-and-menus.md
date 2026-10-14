# Navigation and menus

## Scope + laws behind these patterns
- Use for: usability patterns for navigation ordering, grouping, depth + visibility: nav + tab bars · menus · drop-downs · long lists · links + Back · voice menus.
- Applies when: designing/reviewing how people find + move between destinations.
- Laws underneath: ../laws/serial-position-effect.md, ../laws/hicks-law.md, ../laws/millers-law.md, ../laws/working-memory.md, ../laws/similarity.md, ../laws/jakobs-law.md, ../laws/teslers-law.md (via progressive disclosure), ../laws/occams-razor.md, ../laws/choice-overload.md.
- Also: ../laws/fittss-law.md = travel distance + target size behind menu ordering, prime pixel, edges + corners.
- Bounds:
  - Whoever composes option set steers decision → audit what option set leaves out (../principles/empowering.md).
  - No ads styled as navigation, no controls delivering something other than their label says (../ethics/deceptive-patterns.md).

### Ordering a nav bar or any sequence of destinations?
- When: ordering nav/tab bar or any destination sequence (anchor key items at ends).
- Do: key actions at both outer ends, leftmost + rightmost (primacy + recency). Recall weakest mid-sequence → lowest-priority destinations there.
- Avoid: burying key destination mid-list.
- Why: ../laws/serial-position-effect.md.
- Hypothetical: banking app tab bar: Accounts far left, Pay far right, rarely used Offers in middle.

### Someone proposes capping the menu at 7 items?
- When: someone proposes 7-item menu cap, citing Miller's Law.
- Do: size menus by content + task. Chunk longer menu into grouped sections → stays digestible.
- Avoid: menu-length caps set arbitrarily + justified by Miller's Law's seven-item figure = misreading of Miller's Law.
- Why: prior knowledge + setting shift working-memory capacity. Later work suggests working memory holds closer to 4 items. ../laws/millers-law.md, ../laws/working-memory.md.
- Hypothetical: hospital intranet menu sized to links staff tasks need, grouped under Clinical, Rosters, HR + IT headings.

### How many options per moment, and split a set or not?
- When: nav, drop-downs, menus (few choices per moment, one set shown together).
- Do: few options at once. All options of one set together.
- Why: one set split w/ part out of sight → choice quality drops because alternatives unknown; hidden remainder stays undiscovered; shown part passes for entire set. ../laws/hicks-law.md, ../laws/choice-overload.md.
- Hypothetical: airline seat-class picker lists every class in one short list, not tucking premium classes behind "more options".

### Long list: country picker, categories, directory?
- When: country pickers, long category lists, directories (order long lists so people can subdivide them).
- Do: sort by known key (alphabetical, numeric, chronological) → people halve list mentally instead of scanning all. Group large inventories into high-level categories expanding stepwise.
- Avoid: unordered long list → forces linear scan, not Hick's Law decision process. Over-correcting into deep binary menu chains needing 10+ clicks to reach content.
- Why: ../laws/hicks-law.md.
- Hypothetical: pharmacy formulary sorted alphabetically within drug classes expanding on tap.

### Spoken voice menu?
- When: voice menus.
- Do: short spoken lists. Key option last, where auditory recency strongest.
- Avoid: filler after key choice, e.g. "or say help".
- Term: suffix effect = one extra spoken item after key option erases its recency advantage.
- Why: ../laws/serial-position-effect.md.
- Hypothetical: gas utility's phone line ends short menu on "to report a leak, say leak" + then stops talking.

### Many categories or deep link sets?
- When: many categories or deep link sets (disclose depth on demand).
- Do: each category's links folded away until its label pointed at/tapped → scanning covers one group at a time.
- Avoid: whole link inventory at top level.
- Why: ../laws/teslers-law.md (progressive disclosure).
- Hypothetical: hardware-store app lists departments first; tapping "Plumbing" expands only its subcategories, other departments stay collapsed.

### Styling links and nav items?
- When: styling links + nav items (make navigation look navigable).
- Do: body text one style, links/nav another, clearly set apart.
- Why: plain-looking interactive text gets grouped w/ prose + missed. ../laws/similarity.md.
- Hypothetical: benefits agency page colors + underlines its "check eligibility" links so they do not read as ordinary sentences.

### Tempted to hide navigation off-screen?
- When: tempted to hide nav off-screen for cleaner look.
- Do: before hiding, confirm it creates no obstacle. Ask: smallest visible interface still letting people locate content?
- Avoid: assuming hidden nav = simpler; it can add complexity.
- Why: ../laws/occams-razor.md.
- Hypothetical: museum ticketing site keeps "Visit", "Tickets" + "Exhibitions" visible in header, having first asked whether lone menu icon would hide opening hours from visitors.

### Carrying a mobile nav to larger screens?
- When: mobile nav carried to larger screens (re-check salience at every breakpoint).
- Do: large screens → global nav open, not behind icon. Re-check key controls' relative size at each breakpoint.
- Avoid: scaling layout up w/o scaling key controls → quietly demotes them.
- Why: control salience depends on its share of screen + how many elements compete w/ it.
- Case: one publisher's mobile menu icon took ~20% of nav bar width; same pixel size on desktop took ~3.5% of layout width, amid attractive content.
- Hypothetical: grocery-delivery site shows full category bar on desktop, not phone's single menu icon.

### People browse many pages or items?
- When: people browse many pages/items (show where user went).
- Do: distinct visited-link styling + breadcrumbs → recognition replaces recall.
- Avoid: expecting users to recall pages already checked; they routinely forget.
- Why: ../laws/working-memory.md.
- Hypothetical: rental-listings site greys visited listings + shows breadcrumb trail city > district > street.

### Site of related objects?
- When: sites of related objects, e.g. recipes, chefs + ingredients, or products, brands + reviews (content acts as navigation).
- Do: each object page pivots to related objects (recipe → all its chef's recipes or every dish w/ one of its ingredients) → no dead ends.
- Avoid: relying on global navigation alone.
- Why: small screens may hide global nav; large-screen users may ignore it. First-time users go for prominent content; menus + search = their fallbacks (search-and-results.md).
- Hypothetical: museum collection site: each artwork page links to same artist's other works, same-period works + works in same material.

### How should links and Back behave?
- When: wiring links, Back + full-screen overlays.
- Do: link replaces current page. Back returns to last-seen screen. Back closes full-screen overlay, because users read full-screen overlays as new pages.
- Avoid: opening links in new windows: break Back + confuse people on maximized small screens. Back jumping up hierarchy or going two pages back.
- Hypothetical: train-booking app's full-screen seat map closes on Back, returning to last-seen journey summary.

### Ordering a drop-down, context menu or option sheet?
- When: drop-downs, context menus, long menus, option sheets (order by travel distance).
- Do: most frequent items nearest trigger. Items w/ ~equal use → trigger at list middle, halving longest travel. Prefer grid (mega) menus over long single columns. Prime pixel = open follow-up UI at pointer/finger's current position, e.g. right-click menu at click point, login box beside login link, delete options beside delete icon. Cascading menus → widen or shorten path + add hover tolerance.
- Avoid: radial (pie) menus as default: equalize pointer distance but unfamiliar (../laws/jakobs-law.md); touch has no cursor origin → distance advantage gone. Narrow-path cascading menus: movement through narrow tunnel follows steering law. Option bottom sheet appearing far from its trigger.
- Why: ../laws/fittss-law.md: travel distance + target size.
- Hypothetical: spreadsheet tool's cell context menu opens at click point, copy + paste on top, rarer formatting items lower.

### Pointer-driven full-screen UI: use edges and corners?
- When: pointer-driven, full-screen UIs.
- Do: pin high-frequency desktop commands to true screen edges + corners, because mouse cannot overshoot them (top-edge global menu bar, corner start button, bottom dock).
- Never: edge targets on touch; slower there.
- Avoid: treating browser/window edge as screen edge: browser chrome + taskbars intervene.
- Caveat: corner cheap to hit precisely but may lie far from pointer → weigh both.
- Why: ../laws/fittss-law.md.
- Hypothetical: full-screen desktop video editor pins playback controls to bottom screen edge, where mouse stops by itself.

## Related
- ../laws/fittss-law.md: travel distance + target size behind menu ordering, prime pixel, edges + corners.
- calls-to-action-and-touch-targets.md: size, spacing + placement of controls making up navigation.
- lists-options-and-choice.md: option counts, ordering + comparison beyond menus.
- search-and-results.md: other fallback route to content beside menus.
- layout-grouping-and-hierarchy.md: grouping cues + emphasis for menu sections + nav salience.
- departing-from-convention.md: when to follow navigation conventions + how to deviate.
- ../principles/empowering.md: bound; whoever composes option set steers decision → audit what option set leaves out.
- ../ethics/deceptive-patterns.md: bound; ads styled as navigation, controls delivering something other than their label.
- ../methods/mapping-memory-demands.md: information architecture from users' own categories (card sorting, tree testing) when regrouping navigation.
