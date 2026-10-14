# Pattern catalog

## Use when
- Explains: structure of pattern entries (usability + humane patterns), rules for using them, picking surface / topic files to read.
- Open before individual pattern files when designing, fixing / reviewing surface / feature.

## How entries are built
|Kind|Organized by|Entry shape|Tag|
|---|---|---|---|
|Usability patterns|surface designed / reviewed, not law|file first names laws in play, then entries: When / Do / Avoid / example|laws in play|
|Humane patterns = reusable patterns for products respecting people's attention, time, agency + safety|topic|When (when it applies) / Do (what to do) / Avoid (anti-pattern) / example|principle entry chiefly serves|

- Cases in surface files = real; never add numbers missing from case.
- Every anti-pattern under Avoid ships daily; none hypothetical.
- Humane tag = principle owning pattern's practice in its principle file → reviewer working from one principle finds every pattern under it.
- Where overlap matters → second principle follows as "also …".
- Most humane patterns serve 2-3 principles.

## Rules for applying patterns
|Situation|Do|Avoid|
|---|---|---|
|Weighing UX law|treat as heuristic to weigh|treating as mandate|
|Project research / data disagree w/ principle|project's own research + data outrank any principle|—|
|Design forces people to adapt|bend design to people (core stance)|making people bend to product|
|Explaining to stakeholders|cite law + mechanism; "why" makes decision defensible|citing only rule|
|Predicting problems before testing|Fitts's Law, Hick's Law + Jakob's Law = predictive models → can predict slowdowns + errors before testing|—|
|Reading any entry|first as review question ("do we do this?"), second as design move|—|
|Stakeholder request resembles deceptive-pattern entry|name pattern, cite harm, propose humane alternative; naming trick defends against it = original motive for cataloguing deceptive patterns|—|
|Restoring choice|smallest restoring intervention: off by default, visible end, confirmation / label|—|
|About to add sensor, camera / persistent log|least invasive means: ask for plainest mechanism achieving same outcome; quieter mechanism gets most of effect → any extra data collection must justify itself|—|

- Hypothetical (least invasive means): office kitchen display of floor's shared energy use today nudges people to switch appliances off + identifies nobody; kitchen camera would also nudge but also record people present.

## Picking files: steps
1. Find surface, then scan its patterns. Most screens touch 3-4 surface files.
   - Hypothetical: passport-renewal flow touches forms-and-data-entry.md (applicant details), calls-to-action-and-touch-targets.md (pay + submit button), progress-goals-and-completion.md (multi-step indicator) + memorable-moments-and-endings.md (confirmation screen).
2. Humane side: one feature usually touches several topics → review neighbouring groups too.
3. Money mechanics (pricing, rewards, referrals) → monetization-and-growth.md + defaults-and-choice-architecture.md + [deceptive-pattern taxonomy](../ethics/deceptive-patterns.md) when reviewing how product earns / grows.
4. Habit mechanics (streaks, progress) → habits-streaks-and-gamification.md + notifications-and-interruptions.md + feeds-scrolling-and-pacing.md when product sets pace of someone's day.

## Usability surface files
|File|Covers|
|---|---|
|navigation-and-menus.md|ordering, grouping, depth + visibility of navigation|
|calls-to-action-and-touch-targets.md|primary actions, button hierarchy, target size, spacing, placement|
|forms-and-data-entry.md|fields, formats, validation timing, checkout, payment failure, accessible errors|
|onboarding-and-first-use.md|first-run experience, tours, empty states, activation, re-engagement nudges|
|search-and-results.md|query entry, suggestions, results layout, zero results, filters|
|lists-options-and-choice.md|option counts, ordering, comparison, pricing tiers|
|layout-grouping-and-hierarchy.md|grouping cues, spacing, containers, emphasis, reading order|
|dashboards-and-data-displays.md|dense data screens, chart colour, comparison, prioritisation|
|feedback-loading-and-performance.md|response-time budgets, indicators, skeletons, waits|
|progress-goals-and-completion.md|progress indicators, head starts, multi-step completion|
|errors-and-input-tolerance.md|error prevention + recovery, tolerant input, destructive actions, real content|
|complexity-management.md|who carries complexity, progressive disclosure, settings pages, expert tools|
|first-impressions-and-aesthetics.md|visual polish, what it buys, what it hides|
|departing-from-convention.md|when to follow conventions, when + how to deviate, redesign rollouts|
|memorable-moments-and-endings.md|peaks, endings + failure moments|
|ai-and-automated-features.md (in both lists)|generated answers, agents, automation hand-over, uncertainty, human review, fairness; usability + humane entries side by side|

## Humane topic files
|File|Covers|
|---|---|
|notifications-and-interruptions.md|what interrupts, when, on what channel, under whose control|
|feeds-scrolling-and-pacing.md|stopping points, infinite scroll, autoplay, variable rewards|
|defaults-and-choice-architecture.md|defaults, opt-in, equal-weight decline, symmetric exit|
|friction-undo-and-confirmation.md|confirmation graded by consequence, undo windows, speed bumps|
|recommendations-and-personalization.md|algorithmically ranked feeds, steering controls, rabbit holes, sensitive states|
|privacy-data-and-security.md|data minimisation, consent, access + deletion, tracking|
|calm-technology-and-device-etiquette.md|peripheral attention, quiet signalling, failing gracefully|
|inclusive-and-accessible-design.md|persona spectrum, accessibility floors, low-end devices, identity|
|safety-and-abuse-resistance.md|misuse cases, blocking + reporting, vulnerable people, children|
|transparency-and-honesty.md|transparency of data, algorithms + business model: honest controls, true cost, explaining algorithm, honesty tests|
|monetization-and-growth.md|revenue models, free tiers, virtual currency, referrals|
|habits-streaks-and-gamification.md|streaks, counters, rewards + their effect on vulnerable people|

## The seven principles
- Seven humane principles: ../principles/respectful.md, ../principles/finite.md, ../principles/empowering.md, ../principles/intentional.md, ../principles/inclusive.md, ../principles/resilient.md, ../principles/transparent.md.

## Related
- ../laws/index.md: 30 UX laws named in surface files, by theme, w/ decision matrix.
- [Principles index](../principles/index.md): seven humane-design principles named in entry tags, side by side.
- ../principles/surface-to-principle-map.md: principles each product surface touches first + where to start.
- ../guides/symptom-to-fix-index.md: observed usability problem → law + fix.
- ../guides/design-a-screen-or-flow.md: steps bringing laws, principles + patterns into new design.
- ../guides/review-an-interface.md: steps for usability + humane-design review.
- ../guides/defend-a-decision.md: builds law-and-mechanism rationale explaining design decision to stakeholders.
- ../guides/core-stance.md: working rules: laws as heuristics, people over metrics.
- ../ethics/deceptive-patterns.md: taxonomy to match stakeholder requests against.
