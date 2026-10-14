# Usability review checklist

## Use when
- Reviewing screen, prototype / spec w/ yes/no usability questions.
- Questions grouped by theme: perception + grouping · memory + cognition · attention + salience · decisions + simplicity · motor, time + progress · expectations + emotion · systems + behavior.
- Each question names what to look for (failure signs) + law explaining it.

## Reading answers
|Mark / answer|Means|Do|
|---|---|---|
|Yes|design good on checked point|—|
|[A]|answerable from artifact itself (screen, prototype / spec)|—|
|[P]|needs process / research evidence|—|
|No on [A]|finding|cite law|
|[P] w/o evidence available|no defect|list once under 'Open questions for the team'|

## Steps
1. Quick pass (below) before full checklist.
2. Then answer only rows for surfaces on screen.
3. Merge findings sharing root cause → rank by severity.

## Quick pass
|Check|Passes when|
|---|---|
|Primary action|distinct + close to task|
|State|stays visible across steps|
|Response|system responds within 400 ms|
|Errors|keep person's input + next step together|
|Targets|sized + spaced|
|Ad styling|nothing styled like ad|
|Conventions|kept|
|Ending of flow|no upsells|

## Perception and grouping
|Check|Mark|Failure signs|Law|
|---|---|---|---|
|Related items closer together than to unrelated ones?|[A]|uniform spacing; labels equidistant from two fields; gaps contradicting meaning|../laws/proximity.md|
|Groupings survive every breakpoint?|[A]|stacked columns splitting related items or merging unrelated ones|../laws/proximity.md|
|Optional + escape actions near task?|[A]|Skip, Details / secondary actions in far corners|../laws/proximity.md, via tunnel vision|
|Bounded areas (border, fill) match real groupings?|[A]|cards / panels enclosing unrelated things, or splitting related ones across containers|../laws/common-region.md|
|No false floors?|[A]|full-width contrasting band above below-fold content|../laws/common-region.md|
|All grouping cues agree on one partition?|[A]|spacing says one group, colour / boxes another|../laws/proximity.md, ../laws/similarity.md, ../laws/common-region.md|
|Static text + interactive elements impossible to confuse?|[A]|links + navigation styled like body copy; non-clickable elements styled like links. Why: similarity creates false groups even between far-apart elements|../laws/similarity.md|
|Each visual treatment = exactly one behavior?|[A]|decorative icons in link / CTA colour; several different actions in one style; one icon for different categories|../laws/similarity.md|
|Connectors (lines, arrows, frames, shared colour) used only where relationship exists?|[A]|border giving element priority it does not deserve|../laws/uniform-connectedness.md|
|Figure vs ground unambiguous for every functional element?|[A]|low-contrast text; equal-weight regions flipping between figure + ground; floating layers w/o shadow / elevation|figure-ground, in ../laws/gestalt-principles-overview.md|
|Can person read screen as a few simple shapes?|[A]|busy, irregular compositions. Why: recall + visual handling both favour plain figures over intricate ones|[Prägnanz](../laws/pragnanz.md)|

## Memory and cognition
|Check|Mark|Failure signs|Law|
|---|---|---|---|
|Chunks easy to scan, w/ plain hierarchy?|[A]|text walls; unformatted numbers / codes; dense layouts w/o modules / dividers|../laws/chunking.md, ../laws/millers-law.md|
|UI shows state instead of asking people to remember it?|[A]|query / input lost on next screen; no visited-link styling; no breadcrumbs; comparisons needing details memorized|../laws/working-memory.md|
|Can person do each step w/o holding value (code, price, name) from another screen, or while scanning similar material?|[A]|retyping code shown elsewhere; remembering one name while scanning similar names|../laws/working-memory.md, ../laws/cognitive-load.md|
|Comparisons of more than 2-3 interacting variables pre-computed for person?|[A]|plan / pricing matrices w/o pre-computed comparisons|../laws/working-memory.md|
|Stressful states (error, payment) demand less memory than normal ones?|[A]|transient error toasts; hidden recovery steps; input lost after failure|../laws/working-memory.md|
|Each step shows only needed, relevant information?|[A]|unrequested motion; purely ornamental elements, imagery / colour (Hypothetical: tax-filing step w/ looping background video behind form). Why: decoration costs effort, adds no understanding|../laws/cognitive-load.md, extraneous load|
|Labels, explanations + data beside what they explain?|[A]|legends, help text / definitions needing cross-reference across screen or pages|../laws/cognitive-load.md, split attention|
|Key items at start + end of lists + navigation bars?|[A]|key actions buried mid-list|../laws/serial-position-effect.md|
|Information uninterrupted between where shown + where used?|[A]|interstitials, modals / detours before step using code / instruction|../laws/serial-position-effect.md, recency|
|Icons universal or labelled?|[A]|unlabelled custom icons; only the few glyphs nearly everyone reads alike may go wordless (Hypothetical: hospital ward-booking app pairs its custom bed-transfer glyph w/ text label)|../laws/cognitive-load.md|

## Attention and salience
|Check|Mark|Failure signs|Law|
|---|---|---|---|
|Primary action stands out from similar elements?|[A]|primary + secondary buttons look identical|../laws/von-restorff-effect.md|
|Emphasis rare enough to work?|[A]|several highlights competing; standout elements reading as ads|../laws/von-restorff-effect.md|
|Contrast still works w/o colour + w/o motion?|[A]|state / priority shown by colour alone; motion as only differentiator|../laws/von-restorff-effect.md, accessibility|
|Critical information inside region user reads / acts in?|[A]|key facts in corner label, sidebar / header away from reading path; new UI appearing far from triggering element|../laws/selective-attention.md: tunnel vision, change blindness|
|Real content avoids ad styling + ad zones at every screen size?|[A]|content beside ads, in banner slots / banner-shaped; boxed, coloured / animated sections; contrasting blocks on mobile|../laws/selective-attention.md: banner blindness, faux ads; ../laws/von-restorff-effect.md|
|Important changes noticed?|[A]|weak change cues; several updates competing at once|../laws/selective-attention.md: change blindness|
|Unfinished tasks + more content clearly signalled?|[A]|hidden continuation; no progress indicator on multi-step tasks|../laws/zeigarnik-effect.md|
|Can person finish, dismiss or resume every open loop?|[A]|permanent nags to complete something; cliffhanger teasers; no resume for interrupted work|../laws/zeigarnik-effect.md|
|Challenge matched to skill, w/ feedback on every action?|[A]|no confirmation of what happened; friction, lag / hidden features breaking absorption|../laws/flow.md|
|Can users move straight to next item after completing one?|[A]|return to hub after every action; interruptions during focused work|../laws/flow.md|

## Decisions and simplicity
|Check|Mark|Failure signs|Law|
|---|---|---|---|
|Options minimal where speed matters?|[A]|crowded entry screens; long menus; extra options before core action|../laws/hicks-law.md|
|Every stage keeps option count low, w/ any lengthy, many-part flow spread over several stages?|[A]|one huge form / settings page. Scope: splitting flows into steps = Chunking + Cognitive Load matter; Hick's Law applies only to choices within each step|../laws/chunking.md, ../laws/cognitive-load.md; ../laws/hicks-law.md per step|
|Recommended / featured option present?|[A]|equal weight on all choices|../laws/hicks-law.md, ../laws/choice-overload.md|
|Options side by side when person needs to compare them?|[A]|pricing tiers on separate pages; no filters / search for large set|../laws/choice-overload.md|
|Comparison views free of decoys + irrelevant anchors?|[A]|dominated tier placed to steer choice; struck-through reference prices; spec rows irrelevant to task|../laws/choice-overload.md: decoy effect, distinction bias|
|All options in set shown together?|[A]|shown options pass for whole set while rest sit apart in groups out of view|../laws/cognitive-load.md|
|Every element earns its place, so none could go w/o losing function?|[A]|elements carrying no meaning / value|../laws/occams-razor.md|
|Design effort spent on features most users rely on?|[A]|polish spread evenly over rarely used features|../laws/pareto-principle.md|
|Design counters known biases, not relies on them? (process question)|[P]|designer confirmation bias in research; complexity bias in solutions|../laws/cognitive-bias.md|
|Each default = choice informed user would make, + easy to change?|[A]|pre-checked add-ons; opt-outs serving business; buried settings|../laws/cognitive-bias.md: status quo bias, loss aversion|
|Leaving / cancelling as easy as joining?|[A]|multi-step cancel; retention copy framed around guilt / loss|../laws/cognitive-bias.md: loss aversion|
|Can person check AI output cheaply before accepting?|[A]|no confidence cue / source; one-click acceptance of high-stakes suggestions|../laws/cognitive-bias.md: automation bias|

## Motor, time and progress
|Check|Mark|Failure signs|Law|
|---|---|---|---|
|Touch targets large, spaced + within easy reach?|[A]|small tap targets; cramped adjacent buttons; actions far from where attention is|../laws/fittss-law.md|
|Targets sized by position, specified in physical units, w/ whole visible element clickable?|[A]|hit areas limited to glyph; tiny targets in corners; specs only in pixels|../laws/fittss-law.md|
|Every target meets its platform's minimum? Floors: web 24 × 24 CSS px or equivalent spacing; iOS 44 × 44 pt; Android 48 × 48 dp|[A]|icon buttons + inline links below floor; adjacent targets w/ no gap between them|../laws/fittss-law.md, accessibility floor|
|Direct-manipulation feedback (pressed state, typing echo, drag) within ~0.1 s?|[A]|no pressed state; lag while typing|0.1 s response-time limit in ../methods/thresholds-and-formulas.md; not ../laws/doherty-threshold.md|
|System responds in under 400 ms?|[A]|silent waits; no immediate input acknowledgement|../laws/doherty-threshold.md|
|Unavoidable waits covered by animation / progress indicator?|[A]|blank screens during processing|../laws/doherty-threshold.md|
|Waits > ~2 s placed after completion point, never mid-task?|[A]|spinners between sequence steps; validation interrupting typing|../laws/doherty-threshold.md, closure|
|Operations > ~15 s run in background w/ notification when done?|[A]|modal screens blocking person during long jobs|1968 response-time levels in ../methods/thresholds-and-formulas.md; ../laws/doherty-threshold.md|
|Every progress bar driven by real work?|[A]|timer-filled bars; spinners w/o estimate where one possible|../laws/doherty-threshold.md, ../laws/goal-gradient-effect.md|
|Task takes no longer than users expect? (process question)|[P]|re-typing data system already knows; no autofill in purchase / booking forms|../laws/parkinsons-law.md|
|Progress visible, + user starts w/ some progress already made?|[A]|multi-step flows w/o step count / progress bar|../laws/goal-gradient-effect.md|
|Next goal shown right after completion?|[A]|success screens leading nowhere, where users drop off|../laws/goal-gradient-effect.md, ../laws/zeigarnik-effect.md|

## Progress-bar rules
- Precision not needed. Why: progress-bar benefit = perceptual → rough estimate still helps.
- Bar must track real work: advances only while work advances; stops when work stalls.
- Never let progress bar hide hung process.

## Expectations and emotion
|Check|Mark|Failure signs|Law|
|---|---|---|---|
|Standard patterns behave as elsewhere?|[A]|carts, checkout / form controls reinvented w/o stated purpose; links opening new windows; Back jumping up hierarchy; overlays Back cannot close|../laws/jakobs-law.md, ../laws/mental-model.md|
|Design checked against users' mental models, not team's? (process question)|[P]|no research behind assumptions about how users think|../laws/mental-model.md|
|Assumptions tested w/ real novices, not w/ team itself? (process question)|[P]|designers standing in for users (→ curse of knowledge + false-consensus effect); trusting users' self-reports of understanding, inflated by illusion of explanatory depth. Fix: probe real understanding w/ tasks asking person to explain how thing works|../laws/mental-model.md|
|Paid extras off by default?|[A]|insurance / protection add-ons pre-checked|../laws/mental-model.md, preselection|
|Major redesigns come w/ temporary opt-in + way back?|[A]|sudden forced changes to features people use daily|../laws/jakobs-law.md, discordance|
|Peak + final moments deliberately designed?|[A]|bare confirmation modals at high-stakes steps; flows ending on flat / negative screen|../laws/peak-end-rule.md|
|Flows end w/o exit pop-up, upsell / hook?|[A]|exit-intent offers; 'please don't go' dialogs; upsells on confirmation screens|../laws/peak-end-rule.md|
|Negative peaks (waits, errors, 404s, outages) planned for?|[A]|default error pages; unexplained waits|../laws/peak-end-rule.md|
|Error + outage states explain cause, give realistic recovery time, assign no blame + avoid alarm styling when person can do nothing?|[A]|red, generic 'try later' errors w/o time estimate|../laws/peak-end-rule.md|
|Consecutive failures + hard steps avoided, esp. at end?|[A]|repeated validation errors; final rejection|../laws/peak-end-rule.md, streak-end|
|In testing, task-success measures agree w/ satisfaction ratings? (process question)|[P]|positive ratings contradicted by task failures|../laws/aesthetic-usability-effect.md|

## Systems and behavior
|Check|Mark|Failure signs|Law|
|---|---|---|---|
|System, not user, carries irreducible complexity?|[A]|users entering data system already knows; no defaults; no suggestions|../laws/teslers-law.md|
|Simplification stops before becoming abstraction?|[A]|controls reduced until meaning lost|../laws/teslers-law.md, ../laws/hicks-law.md|
|Each automated feature has designed failure + handover paths?|[A]|no state feedback; no diagnosis / support route when automation breaks; sudden takeover by person w/o preparation|../laws/teslers-law.md|
|Clear feedback + limits in place, w/ varied input accepted + normalized?|[A]|rigid formats; rejecting unambiguous input; silent failures|../laws/postels-law.md|
|Consequential interpreted inputs read back to person before system acts on them?|[A]|lenient parser silently turns free text into amount / date triggering payment / booking|../laws/postels-law.md|
|Strict, validating system behind forgiving surface?|[A]|database structure leaking into form rules; unvalidated input passed downstream|../laws/postels-law.md|
|Output consistent, reliable + accessible?|[A]|input leniency leaking into unpredictable output|../laws/postels-law.md|
|Layout put through extreme-content testing, not only ideal placeholders? (process question)|[P]|short names + studio photos in mockups; longest + shortest real values, missing images, larger fonts, long translations + right-to-left scripts never checked|../laws/aesthetic-usability-effect.md, ../laws/postels-law.md|
|Dangerous / unavailable controls disabled w/ stated reason (not hidden) + placed apart from positive actions?|[A]|OK beside Delete; controls vanishing depending on state; soft keys changing meaning|../laws/fittss-law.md, ../laws/jakobs-law.md|
|Can users record their reasoning during long, interrupted tasks?|[A]|no notes on models, charts / data sets; no action history|../laws/working-memory.md|
|Can users start immediately, w/ help available along any path?|[A]|mandatory tours at start; help only in manual or along one fixed flow|../laws/paradox-of-the-active-user.md|
|Can keyboard users reach + operate every action, in logical order, w/ visible focus indicator?|[A]|menus opening only on hover; focus traps; invisible focus|../laws/postels-law.md (any access method), ../laws/fittss-law.md|
|Every control exposes its name + state to assistive technology?|[A]|icon-only buttons w/ no accessible name|../laws/postels-law.md, ../laws/cognitive-load.md|
|Layout holds at 200% text size, w/ platform text scaling (Dynamic Type, Android font scale) + w/ reduced motion on?|[A]|clipped labels; fixed-height buttons; motion person cannot turn off|../laws/postels-law.md, ../laws/von-restorff-effect.md|
|Text meets 4.5:1 contrast ratio? Large text, UI components, focus indicators + chart marks need at least 3:1|[A]|light grey placeholder / helper text; primary buttons looking disabled|figure-ground in ../laws/gestalt-principles-overview.md; ../laws/von-restorff-effect.md, accessibility|
|Errors tied to their fields + announced to screen readers (live region / focused error summary)?|[A]|red borders as only cue; vanishing toasts; errors far from their fields|error-prevention + error-recovery heuristics in usability-heuristics-map.md; ../laws/working-memory.md|
|Duplicate submissions + irreversible mistakes prevented (idempotent submit, pending state, undo / soft delete; confirmation only for irreversible acts)?|[A]|double charges on double tap; delete w/ no recovery; destructive dialogs whose button says OK|error-prevention heuristic in usability-heuristics-map.md; no law needed|

## Related
- usability-heuristics-map.md: ten classic usability heuristics + laws behind each; use when no law explains "no" answer.
- ../guides/review-an-interface.md: review step sequence walking these themes.
- ../guides/write-a-finding.md: fixed shape, confidence labels + severity ranking for each finding.
- ../guides/symptom-to-fix-index.md: observed usability problem → law explaining it → fix.
- ../guides/law-misapplications.md: wrong uses of each law + correction; check before citing law.
- ../methods/thresholds-and-formulas.md: measurable form of response-time + target-size rows.
- humane-design-audit.md: humane-design companion; yes/no questions per humane principle + AI and automation.
- ../ethics/deceptive-patterns.md: humane bound on default, cancellation + retention-copy rows; names deceptive patterns + honest alternative to each.
