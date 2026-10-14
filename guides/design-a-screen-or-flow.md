# Designing a screen, flow or feature

## Use when
- Designing new screen, component, flow / feature.
- One numbered 15-step sequence; each step belongs to usability / humane pass + names files to open.

## Before step 1
- Read core-stance.md: how to hold the laws, people over metrics + conflict ranking.
- Pick w/ how-deep-to-go.md humane-pass steps feature needs (quick pass, standard review / full treatment).

## Step overview
|Step|Pass|Name|
|---|---|---|
|1|usability|Goal + task core|
|2|usability|Identify surfaces|
|3|humane|Locate the surface|
|4|humane|Attention-hijack check|
|5|humane|Forecast before building|
|6|usability|Conventions by default|
|7|humane|Pick patterns|
|8|usability|Cut, then structure|
|9|usability|Time budget per level|
|10|usability|Peak + ending|
|11|usability|Cross-cutting: human factor, accessibility, personalization|
|12|usability|Check persuasive levers|
|13|humane|Defaults + metrics|
|14|usability|Deliver w/ rationale table|
|15|humane|Gate the launch|

Usability pass = steps 1, 2, 6, 8, 9, 10, 11, 12, 14. Humane pass = steps 3, 4, 5, 7, 13, 15.

## Step 1. Goal + task core (usability)
- Name user's goal + task's irreducible core (../laws/teslers-law.md).
- Decide what system carries rather than user; default = system carries it (../methods/who-absorbs-complexity.md).

## Step 2. Identify surfaces (usability)
- List surfaces design touches → open matching pattern file for each. Most screens touch three / four surfaces.

|Surface|Pattern file|
|---|---|
|Navigation|../patterns/navigation-and-menus.md|
|CTA|../patterns/calls-to-action-and-touch-targets.md|
|Form|../patterns/forms-and-data-entry.md|
|Onboarding|../patterns/onboarding-and-first-use.md|
|Search|../patterns/search-and-results.md|
|Lists|../patterns/lists-options-and-choice.md|
|Layout|../patterns/layout-grouping-and-hierarchy.md|
|Loading|../patterns/feedback-loading-and-performance.md|
|Progress|../patterns/progress-goals-and-completion.md|
|Errors|../patterns/errors-and-input-tolerance.md|
|Endings|../patterns/memorable-moments-and-endings.md|
|AI features|../patterns/ai-and-automated-features.md|

- Every surface in [pattern catalog index](../patterns/index.md); index explains catalog use.

## Step 3. Locate the surface (humane)
- Principles applying to surface → ../principles/surface-to-principle-map.md; names them + adds where-to-start practices.
- Read each implicated principle in own file: definition, practices, review questions under `Audit questions`.
- Seven principles: ../principles/respectful.md, ../principles/finite.md, ../principles/empowering.md, ../principles/intentional.md, ../principles/inclusive.md, ../principles/resilient.md, ../principles/transparent.md; side by side in [principles index](../principles/index.md).

## Step 4. Attention-hijack check (humane)
- Ten attention hijacks + paired counters: table in ../ethics/attention-hijacks.md.
- For each lever design pulls, ask: does it respect / exploit underlying human sensitivity?
- For each hijack design uses → adopt its named counter.
- Attention-hijack pass described in ../principles/cross-cutting-practices.md.

## Step 5. Forecast before building (humane)
- Use ../methods/second-order-thinking.md, ../methods/futures-wheel.md, ../methods/premortem.md + ../methods/misuse-case-brainstorming.md.
- Same method set also holds [four quadrants of design responsibility](../methods/four-quadrants-of-responsibility.md) + ../methods/three-gate-check.md; [methods overview](../methods/index.md) maps method to stage.
- Include indirect users (affected people never opening product) + intimate-partner attacker.
- Findings → explicit anti-goals → change plan.

## Step 6. Conventions by default (usability)
- Known conventions by default (../laws/jakobs-law.md, ../laws/mental-model.md).
- Deviate from convention only for differentiation, disruption / exploration → plan test for deviation (../methods/convention-or-new-pattern.md, ../patterns/departing-from-convention.md).

## Step 7. Pick patterns (humane)
- Choose from pattern files matching surface; each entry: when it applies, what to do + avoid, example.

|Concern|Pattern file|
|---|---|
|Notifications|../patterns/notifications-and-interruptions.md|
|Feeds|../patterns/feeds-scrolling-and-pacing.md|
|Defaults|../patterns/defaults-and-choice-architecture.md|
|Friction|../patterns/friction-undo-and-confirmation.md|
|Personalization + AI|../patterns/recommendations-and-personalization.md, ../patterns/ai-and-automated-features.md|
|Privacy|../patterns/privacy-data-and-security.md|
|Calm technology|../patterns/calm-technology-and-device-etiquette.md|
|Inclusion|../patterns/inclusive-and-accessible-design.md|
|Safety|../patterns/safety-and-abuse-resistance.md|
|Transparency|../patterns/transparency-and-honesty.md|
|Process|../methods/process-safeguards.md: process patterns keeping other patterns honest|
|Monetization + growth|../patterns/monetization-and-growth.md|
|Habit + progress|../patterns/habits-streaks-and-gamification.md|

- If design notifies people → pick channel + moment from urgency-by-modality + timing tables in ../checklists/interruption-decision-rules.md.

## Step 8. Cut, then structure (usability)
- First cut choices + elements (../laws/hicks-law.md, ../laws/choice-overload.md, ../laws/occams-razor.md, ../laws/cognitive-load.md) → then structure what remains (../laws/chunking.md, ../laws/proximity.md, ../laws/common-region.md).
- Stop cutting before clarity / meaning lost.
- Step lists: ../methods/cutting-to-essentials.md (applying Occam's Razor), ../methods/lightening-mental-effort.md (reducing cognitive load), ../methods/gestalt-layout-pass.md (grouping-first layout).

## Step 9. Time budget per level (usability)
Timing budget for each response level:

|Level|Budget|
|---|---|
|Pressed state / input echo|appears in < 0.1 s|
|System response|< 400 ms (../laws/doherty-threshold.md)|
|Slow work|cover it (../patterns/feedback-loading-and-performance.md)|
|Whole task|beat its expected duration (../laws/parkinsons-law.md, ../laws/goal-gradient-effect.md)|

- Every timing limit → ../methods/thresholds-and-formulas.md; timing pattern entries → ../patterns/feedback-loading-and-performance.md.

## Step 10. Peak + ending (usability)
- Design experience's peak + ending, failure states included (../laws/peak-end-rule.md, ../methods/peaks-and-endings.md, ../patterns/memorable-moments-and-endings.md).

## Step 11. Cross-cutting: human factor, accessibility, personalization (usability)
- Human factor: design for tired, stressed, older / distracted user, not for team.
- Accessibility = specifications, not intentions → carry specs into deliverable, not only into testing.

|Accessibility spec|Value|
|---|---|
|Text contrast|4.5:1|
|Large text, UI components, focus indicators|contrast 3:1|
|Colour / motion|never convey meaning by colour / motion alone|
|Errors|announce to screen readers (aria-live region / focused error summary); tie each error to its field|
|Text size|layout survives 200% text size + platform scaling (Dynamic Type, font scale)|
|Target size|meet floors in ../laws/fittss-law.md file (same row in ../laws/index.md)|
|Keyboard|keyboard access + focus order|
|Motion setting|respect reduced-motion|

- Humane-design accessibility entries → ../patterns/inclusive-and-accessible-design.md.
- Personalization: infer / default settings rather than requiring setup; active users skip configuration (../laws/paradox-of-the-active-user.md).
- Personalization: system carries adaptation, not user (Tesler's Law).

## Step 12. Check persuasive levers (usability)
- Test each lever against ../ethics/influence-vs-manipulation.md; concrete examples in ../ethics/using-psychology-responsibly.md + each lever's law file (../laws/index.md).

## Step 13. Defaults + metrics (humane)
- Justify every default as recommendation you would defend aloud (../patterns/defaults-and-choice-architecture.md).
- Pair each growth metric w/ user-goal metric + counter-metric (../methods/counter-metrics.md, ../methods/measure-what-you-value.md, ../methods/goals-signals-metrics.md).
- Same metric-method set: ../methods/reading-experiments-honestly.md, ../methods/engagement-vs-empowerment-metrics.md.

## Step 14. Deliver w/ rationale table (usability)
- Deliver short rationale table: `decision | law + mechanism | what could prove it wrong | metric or test`.
- Mark each decision: convention (low risk) / deviation (needs testing).
- Common mobile patterns, e.g. collapsed order summary / sticky CTA, count as conventions.
- Hypothetical row, clinic booking app: decision = visit length auto-set from chosen visit type | law + mechanism = Tesler's Law, system carries choice it can derive | could prove it wrong = patients w/ several concerns get slot too short | metric = share of visits overrunning / rebooked.
- Row → argument: defend-a-decision.md.

## Step 15. Gate the launch (humane)
Launch gate defined in ../ethics/ethics-review-workflow.md. Gate conditions:
- Safety features ship on day one (../patterns/safety-and-abuse-resistance.md).
- Block, report + appeal specified before launch.
- Named owner watches feature after launch.
- Any Blocking-severity finding holds gate (write-a-finding.md).
- Rollout stages, holdout group + withdrawal condition written down before first cohort sees feature (../methods/process-safeguards.md).

## Related
- core-stance.md: how to hold the laws, people over metrics, conflict ranking.
- how-deep-to-go.md: humane-pass steps required by quick pass, standard review / full treatment.
- review-an-interface.md: same two passes on something already existing.
- defend-a-decision.md: rationale-table row → argument.
- common-mistakes.md: most damaging misuses, usability + humane sides.
- laws-and-principles-crosswalk.md: principle bounding each law + lever each principle guards.
- ../laws/index.md: index of all 30 UX laws, w/ decision matrix for choosing law fitting situation.
- [Pattern catalog index](../patterns/index.md): every surface + how to use catalog.
- ../ethics/ethics-review-workflow.md: step 15's launch gate.
