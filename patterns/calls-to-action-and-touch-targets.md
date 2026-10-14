# Calls to action and touch targets

## Scope
- Primary actions, button hierarchy, target size, spacing + placement on touch + pointer screens.
- Open when designing/reviewing buttons, tappable/clickable controls, action placement, disabled states, target size + spacing, main-action emphasis.

## Laws behind these patterns
|Law|Role here|
|---|---|
|../laws/fittss-law.md|target size, distance, travel|
|../laws/von-restorff-effect.md|primary action as isolate|
|../laws/selective-attention.md|banner blindness; actions near focus|
|../laws/hicks-law.md|highlight suggested choice among competing actions|
|../laws/serial-position-effect.md|one law behind call-to-action + placement patterns|

## Size and hit area

### How large, how far apart, how reachable?
- When: any tappable/clickable control, especially on touch screens.
- Do: targets in easy hand/pointer reach, generous gaps, size for reliable hits.
- Avoid: small, crowded targets.
- Why: speed-accuracy trade-off: errors climb when movement quick + target small (Fitts's Law). Size alone insufficient w/o spacing + reachable placement.
- Evidence: one tapping study: no participant hit exact centre of menu icon; some missed it entirely.
- Hypothetical: museum audio-guide touchscreen used while visitors stand + walk: big, well-spaced play/pause/next buttons along bottom edge → reliable taps mid-stride.

### Which size figure to design a touch target to?
- Do: size touch targets by screen position, in physical units: ~7 mm scrolling centre; ~12 mm corners. Target only as large as location needs. Short labels on touch targets. Standard minimums = floors, never aims → positional physical figures above floor.
- Avoid: one pixel size everywhere on screen; older ISO touch-target sizes (22 × 22 mm), made for infrared-grid screens sensing whole finger.
- Why: even density-independent pixels vary physically by screen + unrelated to human dimensions.
- Evidence: positional figures (~7 mm centre, ~12 mm corners) from observational research on how people touch phones; cover 95% of observed taps.
- Floors:

|Standard|Floor|
|---|---|
|WCAG 2.2 level AA, success criterion 2.5.8|24 × 24 CSS px, or spacing where 24 px circle per target touches no other target|
|WCAG success criterion 2.5.5 (enhanced level)|44 × 44 CSS px|
|iOS|44 × 44 pt|
|Android|48 × 48 dp|

- Hypothetical: parking-payment app: mid-screen zone-number keypad sized to centre physical figure, corner "help" + "back" to larger corner figure; never below platform floor.
- Measurable form of laws (target sizes, formulas): ../methods/thresholds-and-formulas.md. Testing under real grip + context: ../methods/testing-touch-layouts.md.

### Which part of the element is the target?
- When: cards, list rows, links, icon buttons.
- Do: whole visible boundary clickable, e.g. product tile's image, text + button area together. Icon + label = one hit area. Target looks as large as it acts.
- Avoid: only glyph/only text active; invisible padding as only enlargement (users still slow to hit visible shape); text links readable on touch screen yet too small to tap accurately (read-tap asymmetry).
- Hypothetical: bank account list: tap anywhere on row (name, balance, chevron) opens account, not only small chevron.

## Placement

### Where does each level of control go on a touch screen?
- When: arranging mobile touch-screen hierarchy (centre-first layout).
- Do: primary content + interaction (lists, grids) in scrolling centre; secondary controls (tabs, action buttons) at top + bottom edges; tertiary options in menus behind a few large corner targets.
- Avoid: touch layout built on one-thumb reach heat map, because people constantly shift grip on phone.
- Evidence: upper-corner back button = often most-used control on phone screen. Usability test of centre-first layout: every participant, incl. people w/ no mobile experience, found corner-menu options within a few seconds.
- Hypothetical: transit app: departures list in scrolling middle, route tabs along bottom, rarely used settings in menu behind one large top-corner button.

### How close to the user's focus should the action sit?
- When: placing task-completing button, optional/escape actions (Skip, Not now), detail links, task-specific buttons.
- Do: actions near user's task + focus → shorter travel (Fitts's Law, Selective Attention). Optional actions near content + calls to action user already watches. Keep paired navigation (Previous / Next) together. Task-specific action beside its content, apart from global form buttons.
- Avoid: primary button far from work area; optional actions in far corners task-focused users never see.
- Case: optional Skip link in top corner unseen → users thought sign-up mandatory. Add employer button among Next, Save as Draft + Cancel got lost, hard to find.
- Hypothetical: clinic check-in kiosk: "I don't have insurance" directly under insurance-card field, not in footer; "Add another medication" under medication list, away from Continue.

### How to arrange hero controls and ejector seats?
- Terms: hero controls = most used, most important or most drastic actions → prominence up front. Ejector seats = drastic, irreversible controls → kept apart from others.
- When: arranging actions on screen/device.
- Do: most used/important/drastic action gets spatial + visual prominence. Group related controls in zones. Irreversible actions physically apart from positive ones. Each control: affordance (shows it exists), label/icon (shows what it does), feedback (shows it acted). Before consequential actions → feedforward: outcome preview. One control = one function, unless it toggles its own action.
- Avoid: OK directly beside destructive Cancel/Delete; context-changing soft keys (weaken predictability).
- Hypothetical: electric-car charging app: "start charging" (most used) = large central button; "stop + unlock cable" (drastic) in own separate spot; price + timer details in own zone.

## Emphasis and availability

### Which action stands out, and how?
- When: one action/piece of info matters most on screen.
- Do: primary action visually apart from similar elements (Von Restorff Effect). When actions compete → highlight suggested choice → users skip weighing whole set (Hick's Law), w/o hiding needed options. Motion to set isolate apart → only once effect on motion-sensitive viewers weighed.
- Avoid: emphasizing many things (competing highlights cancel each other out); ad-like standout (banner blindness filters it out); isolate marked by hue alone (fails people w/ reduced sight/impaired colour perception).
- Hypothetical: tax-filing summary page: "Submit return" = filled button w/ icon + bold label, while "Save draft" + "Download copy" stay outlined but visible.

### Action unavailable right now: hide it or disable it?
- When: action temporarily unavailable or dangerous in current state.
- Do: keep control in place, disabled/locked; say why + how to re-enable. Disabling w/ reason = mistake-proofing (poka-yoke).
- Avoid: hiding unavailable controls (vanishing controls) → breaks learned positions (Fitts's Law, Jakob's Law) + leaves users unsure whether feature exists.
- Hypothetical: pharmacy app keeps "Request refill" in usual spot, greyed, w/ note "waiting for prescriber approval; you'll be able to request once approved".

## Humane bounds
- defaults-and-choice-architecture.md: equal-weight No on every prompt; defaults as honest suggestions → bound on button hierarchy.
- transparency-and-honesty.md: primary + dismiss actions visually honest; controls do what label says.
- ../ethics/deceptive-patterns.md: emphasis + placement never used for hidden No, bait and switch, disguised ads.

## Related
- ../methods/thresholds-and-formulas.md: measurable form of laws: target sizes + formulas.
- ../methods/testing-touch-layouts.md: touch targets under real grip + context.
- forms-and-data-entry.md: Submit after last field, enabled submit button, pending state while payment in flight.
- navigation-and-menus.md: menu ordering by travel distance, prime pixel, edges + corners.
- layout-grouping-and-hierarchy.md: grouping cues + emphasis around primary action.
- defaults-and-choice-architecture.md: humane bound on button hierarchy.
- transparency-and-honesty.md: visually honest primary + dismiss actions.
- ../ethics/deceptive-patterns.md: what emphasis + placement must never serve.
- ../laws/fittss-law.md: size, distance + travel behind every target rule here.
- ../laws/von-restorff-effect.md: isolate primary action.
