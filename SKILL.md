---
name: ux-knowledge
description: Provides a consultable UX knowledge base (knowledge to apply, not a builder): 30 psychology-based UX laws, seven humane-design principles, interface patterns for 28 product surfaces, a deceptive-pattern taxonomy, review checklists, design, foresight and metrics methods, research evidence and a glossary, one small file per topic, written as decision rules. Use when designing, reviewing, auditing or explaining any UI, screen, flow, form, navigation, onboarding, search, dashboard, notification, feed, recommendation, AI feature, default, pricing or data-collection decision; diagnosing why an interface feels hard, slow or confusing; checking for dark patterns or manipulation; answering product-ethics questions; justifying a design decision; or checking the research finding, date or exact term behind a UX claim.
---

# UX knowledge

## Contents
- What this is
- How to consult
- Start from the situation
- Rules that hold everywhere
- Catalog
- Notation

## What this is
- Knowledge base, not builder: alone designs nothing, codes nothing, audits nothing.
- Equips any agent/skill designing, building, reviewing or explaining interface w/ knowledge to do it well → consult, then apply it inside task at hand.
- One small file per topic; each stands alone + ends w/ `## Related`. Open only needed files.
- Two complementary halves:

|Half|Asks about|Covered by|
|---|---|---|
|Usability|how people perceive, remember, attend, decide + move|30 laws, patterns by surface, usability review checklist|
|Humane design|what product does to people's time, attention, agency, safety + trust|seven principles, humane patterns, deceptive-pattern taxonomy, humane-design audit checklist|

- Design can pass one half + fail other → always check both. How halves interlock: [crosswalk](references/guides/laws-and-principles-crosswalk.md).

## How to consult
1. **Match situation.** Every fitting row of situation table below → open first file each names. Most tasks match 2–3 rows.
2. **Read little.**
   - Focused question → 2–4 files total.
   - Work on one surface → its pattern file + 1–2 laws/principles behind main point.
   - More files only for full review, or feature charging, collecting, ranking or acting on its own; then [how deep to go](references/guides/how-deep-to-go.md) sets how many.
   - Then column = pick-from menu, not to-do list.
3. **Make both passes**, even when question seems to fit one half only.
   - Usability pass: laws + usability patterns → what people see, remember, decide + do.
   - Humane pass: principles + humane patterns → what feature does to people.
4. **Check before quoting.** Before giving number, study, name, date or term → open file holding it + read [citation caveats](references/evidence/citation-caveats.md).
   - File does not state it → do not state it.
   - State evidence by year, study type, sample + caveat ([stating evidence](references/evidence/stating-evidence.md)); keep file's hedge.
   - No file names people: give origin as year + work type (law file's `Why it works`, [timeline](references/lookup/timeline.md), [misquoted claims](references/lookup/misquoted-claims.md)).
5. **Fit law to mechanism.** Before attaching law to problem → state mechanism in one sentence + confirm law's file says law explains it. Reading its `In one line` + `Applies when / does not apply when` suffices.
   - No law fits → cite matching usability heuristic instead, via [heuristics map](references/checklists/usability-heuristics-map.md).
6. **Name what stands behind each point.** In output, give law, principle or deceptive pattern behind every main point + its mechanism in one clause. Advice w/o them = opinion; supplying them = this knowledge base's purpose.
7. **Report in fixed shape** of [writing a finding](references/guides/write-a-finding.md).

## Start from the situation
|Situation|Open first|Then|
|---|---|---|
|New screen, flow or feature|[Design a screen or flow](references/guides/design-a-screen-or-flow.md)|pattern file of each surface touched ([pattern catalog](references/patterns/index.md)); [surface-to-principle map](references/principles/surface-to-principle-map.md)|
|Reviewing/auditing something existing|[Review an interface](references/guides/review-an-interface.md)|problems already listed → [symptom-to-fix index](references/guides/symptom-to-fix-index.md) has row for most; not yet listed → both [usability review](references/checklists/usability-review.md) + [humane-design audit](references/checklists/humane-design-audit.md); depth → [how deep to go](references/guides/how-deep-to-go.md)|
|Concrete problem: slow, cluttered, confusing, missed, mis-clicked, abandoned|[Symptom-to-fix index](references/guides/symptom-to-fix-index.md)|matching row's law file|
|One surface: form, navigation, onboarding, search, notifications, feed, AI feature, checkout, settings, dashboard|its file in `patterns/` (pick via [pattern catalog](references/patterns/index.md))|laws + principles linked atop that file|
|Applying/explaining one law|law's own file in `laws/`|[law misapplications](references/guides/law-misapplications.md)|
|Not sure what law fits|[UX laws index](references/laws/index.md)|[heuristics map](references/checklists/usability-heuristics-map.md)|
|Manipulative? Dark pattern? (hidden cost, scarcity/urgency cue, countdown, guilt copy, hard cancellation)|[Deceptive patterns](references/ethics/deceptive-patterns.md)|[influence vs manipulation](references/ethics/influence-vs-manipulation.md); [attention hijacks](references/ethics/attention-hijacks.md); [anti-patterns + humane alternatives](references/ethics/anti-patterns-and-humane-alternatives.md); countdowns + alarm copy → also [inclusive + accessible design](references/patterns/inclusive-and-accessible-design.md)|
|Feed, autoplay, notifications or anything built to hold attention|[Feeds, scrolling and pacing](references/patterns/feeds-scrolling-and-pacing.md) / [Notifications and interruptions](references/patterns/notifications-and-interruptions.md)|[attention hijacks](references/ethics/attention-hijacks.md); [deceptive patterns](references/ethics/deceptive-patterns.md) for named pattern; [Selective Attention](references/laws/selective-attention.md); [addiction + variable rewards evidence](references/evidence/addiction-and-variable-rewards.md)|
|Pricing, subscription, free trial, cancellation or any exit flow|[Defaults and choice architecture](references/patterns/defaults-and-choice-architecture.md)|[monetization + growth](references/patterns/monetization-and-growth.md); [deceptive patterns](references/ethics/deceptive-patterns.md); [Cognitive Bias](references/laws/cognitive-bias.md) for defaults + loss aversion; [business cost of deception](references/evidence/business-cost-of-deception.md)|
|Persuasive lever in play: progress, streak, default, emphasis, delay|[Using psychology responsibly](references/ethics/using-psychology-responsibly.md)|humane side: [habits, streaks + gamification](references/patterns/habits-streaks-and-gamification.md), [defaults + choice architecture](references/patterns/defaults-and-choice-architecture.md); usability side: [progress, goals + completion](references/patterns/progress-goals-and-completion.md), [Goal-Gradient Effect](references/laws/goal-gradient-effect.md); both sides: [crosswalk](references/guides/laws-and-principles-crosswalk.md)|
|Product-ethics question, e.g. should this ship?|[Answer an ethics question](references/guides/answer-an-ethics-question.md)|[ethics review workflow](references/ethics/ethics-review-workflow.md) / [Three-gate check](references/methods/three-gate-check.md)|
|Planning feature's consequences before building|[Methods index](references/methods/index.md)|[premortem](references/methods/premortem.md) / [second-order thinking](references/methods/second-order-thinking.md) / [misuse-case brainstorming](references/methods/misuse-case-brainstorming.md)|
|Choosing/questioning metrics|[Counter-metrics](references/methods/counter-metrics.md)|[measure what you value](references/methods/measure-what-you-value.md) / [engagement vs empowerment metrics](references/methods/engagement-vs-empowerment-metrics.md) / [reading experiments honestly](references/methods/reading-experiments-honestly.md)|
|Feature ranks, collects, charges or acts on its own; reaches children or vulnerable people; product about health, mood, sleep or well-being|[How deep to go](references/guides/how-deep-to-go.md)|[safety + abuse resistance](references/patterns/safety-and-abuse-resistance.md); [privacy, data + security](references/patterns/privacy-data-and-security.md); [children + adolescents evidence](references/evidence/children-and-adolescents.md)|
|Mobile/touch layout|[Calls to action and touch targets](references/patterns/calls-to-action-and-touch-targets.md)|[Fitts's Law](references/laws/fittss-law.md) / [testing touch layouts](references/methods/testing-touch-layouts.md) / [thresholds + formulas](references/methods/thresholds-and-formulas.md)|
|Accessibility + inclusion|[Inclusive and accessible design](references/patterns/inclusive-and-accessible-design.md)|[Inclusive](references/principles/inclusive.md) / [thresholds + formulas](references/methods/thresholds-and-formulas.md)|
|Defending decision to stakeholders|[Defend a decision](references/guides/defend-a-decision.md)|[stakeholder arguments](references/methods/stakeholder-arguments.md)|
|About to cite number, study or case|law file's `Evidence` section, or theme file in `evidence/`|[stating evidence](references/evidence/stating-evidence.md); [citation caveats](references/evidence/citation-caveats.md)|
|When was something shown/claimed; what term means|[Misquoted claims](references/lookup/misquoted-claims.md)|[timeline](references/lookup/timeline.md) / [glossary](references/lookup/glossary.md)|
|Response-time limit, target size or formula|[Thresholds and formulas](references/methods/thresholds-and-formulas.md)|[Doherty Threshold](references/laws/doherty-threshold.md) / [Fitts's Law](references/laws/fittss-law.md)|
|Writing up findings|[Write a finding](references/guides/write-a-finding.md)|[common mistakes](references/guides/common-mistakes.md)|

## Rules that hold everywhere
Full version + when this knowledge does not apply: [core stance](references/guides/core-stance.md).
- UX law = heuristic + hypothesis, never mandate. User research + project data outrank any law.
- Design bends to fit people; people never asked to bend to fit product.
- Mechanism first, then law. Law cited for behavior it does not explain = worse than no law at all.
- Evidence strength = part of claim → keep hedges (may, about, one study, vendor-authored, contested) verbatim.
- Whoever ships product owns its effects; misuse nobody imagined = design failure, not excuse.
- Values conflict → human rights (privacy, security, accessibility) rank above people's time + effort; those rank above delight.
- Retire word "user" from team talk; say "people" instead + state success by their goals, not DAUs or conversions. Count people, not percentages.
- Knowledge making product intuitive can also make it compulsive → test every persuasive lever against person's own goals.
- Prefer smallest change handing choice back: off by default, visible end, confirmation, label.
- Name deceptive pattern + pair it w/ its honest alternative.

## Catalog
Paths relative to this file; grouped by folder.

### references/laws/ (30 laws)
- Every law file has same core sections (a few add origins, product cases, terms or which-number table): `In one line` (claim, type, theme, core rule) · `Applies when / does not apply when` · `Decision rules` · `Why it works` (mechanism, then dated origin) · `Evidence` (Finding | Study | Strength + caveat | Design consequence) · `Misreadings and limits` (Wrong → Right) · `Check questions` · `Symptoms → fixes` · `Hypothetical examples` · `Humane bound` (principle limiting law + how it gets turned against people) · `Related`.
- [UX laws index](references/laws/index.md): all 30 side by side by theme, w/ dated origin, design rule + scope + decisions each law moves.
- [Gestalt grouping principles overview](references/laws/gestalt-principles-overview.md): shared background of five grouping laws: origin, common mechanism, how cues combine + compete, shared limits.

#### Perception and grouping
|Law|In one line|Not for|
|---|---|---|
|[Law of Common Region](references/laws/common-region.md)|Elements inside one shared boundary (border, fill, card) read as group|adding boxes where spacing already groups; treating it as same cue as connectedness|
|[Law of Prägnanz](references/laws/pragnanz.md)|Least-effort reading wins: complex/ambiguous image seen in plainest form; umbrella of grouping laws|proof simpler = better; model of how perception works|
|[Law of Proximity](references/laws/proximity.md)|Close-placed objects read as one group w/ shared function; every gap carries meaning|removing containers w/o widening gaps between groups|
|[Law of Similarity](references/laws/similarity.md)|Distance between items does not stop shared look binding them into one set → links + controls need own look|card grid hard to compare (belongs to Cognitive Load + Working Memory)|
|[Law of Uniform Connectedness](references/laws/uniform-connectedness.md)|Visible link (line, arrow, frame, shared color) makes elements seem more strongly related|merging it w/ Common Region into one draw-a-box rule; fixed rankings of cue strength|

#### Memory and cognition
|Law|In one line|Not for|
|---|---|---|
|[Miller's Law](references/laws/millers-law.md)|Working memory holds ~7 ± 2 chunks on average; later research argues nearer 4 → reason to chunk|capping menus, tabs or lists at seven: visible options scanned, not memorized|
|[Working Memory](references/laws/working-memory.md)|Small, fast-decaying workspace: few chunks (4–7), each fading after ~20–30 s → system remembers, person recognizes|treating 7 ± 2, 4–7 + ~4 as one rule; assuming fully visible dashboard costs no memory|
|[Chunking](references/laws/chunking.md)|Meaningful units assembled from separate bits of information; pays off most on dense screens + long strings|cutting material people search, scan or compare into memory-sized batches|
|[Cognitive Load](references/laws/cognitive-load.md)|Operating + making sense of interface both draw on person's thinking capacity; total drawn = load; intrinsic vs extraneous → cut extraneous|fixed click budget; aiming for zero load|
|[Serial Position Effect](references/laws/serial-position-effect.md)|First (primacy) + last (recency) items recalled best → two ends anchor 1–2 key items; rest follows frequency or key familiar to people|ordering whole visible menu: it = recall effect|

#### Attention and salience
|Law|In one line|Not for|
|---|---|---|
|[Selective Attention](references/laws/selective-attention.md)|Goal-relevant stimuli get attention, all else filtered out → place what matters in reading path|grids of look-alike cards (belongs to Cognitive Load)|
|[Von Restorff Effect (Isolation Effect)](references/laws/von-restorff-effect.md)|Item unlike its similar neighbours = one remembered; emphasis works only while rare|presenting one primary action as research rule: original study measured recall|
|[Zeigarnik Effect](references/laws/zeigarnik-effect.md)|Memory favors tasks interrupted or left unfinished → signal more content, show progress|head starts or pre-credited progress (endowed progress = Goal-Gradient Effect)|
|[Flow](references/laws/flow.md)|Full absorption (enjoyment, total engagement, energized concentration) when challenge matches person's skill|calling endless scroll or long sessions flow|

#### Decisions and simplicity
|Law|In one line|Not for|
|---|---|---|
|[Hick's Law (Hick-Hyman Law)](references/laws/hicks-law.md)|More choices + more complex choices → longer decisions; RT = a + b log2(n)|unordered menus, data-entry steps, screens w/ nothing to choose|
|[Choice Overload](references/laws/choice-overload.md)|Large option set overwhelms + sours whole experience → feature one, offer filters, allow side-by-side comparison|many independent settings or multi-select filters: effect needs one pick among alternatives|
|[Cognitive Bias](references/laws/cognitive-bias.md)|Systematic, often unconscious judgment errors from mental shortcuts → design to shield people from them; watch team's own|steering people against their own goals|
|[Occam's Razor](references/laws/occams-razor.md)|Assumption count = tie-breaker when options tie on predictive power: leanest wins → start simple, drop parts w/o function|choosing simpler option performing worse; cutting until function breaks|
|[Pareto Principle](references/laws/pareto-principle.md)|Small share of causes (~20%) accounts for most effects (~80%) → effort first where most people gain most|exact 80/20 split: check actual usage in analytics|

#### Motor control and time
|Law|In one line|Not for|
|---|---|---|
|[Fitts's Law](references/laws/fittss-law.md)|Movement time to target rises w/ distance + falls w/ size → near focus, within reach, large, well spaced|control people never find; thumb-zone maps; minimum target sizes (those floors = standards, not law predictions)|
|[Doherty Threshold](references/laws/doherty-threshold.md)|Responses under 400 ms (older standard 2,000 ms) → no idle time on human or machine side, steep productivity gain; 400 ms = popular attribution, originating 1982 paper argued for sub-second response|0.1 s pressed state of control; preventing double submits|
|[Parkinson's Law](references/laws/parkinsons-law.md)|Work expands to fill time allotted → beat duration people expect (autofill, data reuse, short flows)|evidence of anything: began as humorous essay|
|[Goal-Gradient Effect](references/laws/goal-gradient-effect.md)|Motivation + effort rise as goal nears → show steps left, small truthful head start; human evidence covers real, reachable rewards|explaining why people drop out|

#### Expectations and emotion
|Law|In one line|Not for|
|---|---|---|
|[Jakob's Law](references/laws/jakobs-law.md)|One product = smaller share of person's total use → products they already use set expectations; convention by default|banning novelty: depart when gain survives learning cost; test departure|
|[Mental Model](references/laws/mental-model.md)|People act on compressed internal model predicting system behavior → design to people's model, not team's|reading familiar design's preference win as proof of quality|
|[Aesthetic-Usability Effect](references/laws/aesthetic-usability-effect.md)|Good-looking design judged easier to use + earns leniency for minor flaws|proof of usability: in tests, polish keeps problems out of sight|
|[Peak-End Rule](references/laws/peak-end-rule.md)|Experience judged by most intense moment (peak) + end, not average → cite both halves|mid-experience abandonment; ending alone|

#### Complexity and robustness
|Law|In one line|Not for|
|---|---|---|
|[Tesler's Law](references/laws/teslers-law.md)|Every system holds irreducible complexity: can get moved, never removed → let system carry it|simplifying until controls turn abstract: complexity only moves|
|[Postel's Law (Robustness Principle)](references/laws/postels-law.md)|Strictness for what goes out (sent/emitted), leniency for what comes in → normalize clear input, keep own output standard|silently accepting ambiguous input; leniency inside system|
|[Paradox of the Active User](references/laws/paradox-of-the-active-user.md)|People start using software at once + leave manuals unopened → contextual help, progressive onboarding|hiding features: training-wheels study disabled features visibly|

### references/principles/ (7 principles + 3 support files)
- Every principle file: `In one line` · `Core practices` · `Commitments w/ a pattern (or method) entry` · `Guidance held here` · `Why it matters` · `Key concepts` · `Audit questions` (yes/no) · `Neighbours to check` · `Related`; Intentional + Resilient add one extra section each.
- [Principles index](references/principles/index.md): seven side by side; which to read in full.
- [Cross-cutting practices](references/principles/cross-cutting-practices.md): team + process habits serving all seven (reviews, kickoffs, research, metrics, norms).
- [Surface-to-principle map](references/principles/surface-to-principle-map.md): per product surface → principles hit first, where to start, pattern files to open.

|Principle|In one line|
|---|---|
|[Respectful](references/principles/respectful.md)|Well-being, attention + time = borrowed → return them w/ value; governed mainly by how + when product interrupts|
|[Finite](references/principles/finite.md)|Experience has edges: quality of time above endless quantity → stopping points instead of auto-refill|
|[Empowering](references/principles/empowering.md)|What people gain outranks what product earns from them; yardstick = agency, not utility|
|[Intentional](references/principles/intentional.md)|Quick win weighed against later + second-hand effects; friction placed on purpose where it protects|
|[Inclusive](references/principles/inclusive.md)|Every variation in ability, context, culture, language + mental state in scope; inclusion = way of working, not compliance state|
|[Resilient](references/principles/resilient.md)|Abuse assumed as given; design first for whoever stands to get hurt most; abusability = successor to usability|
|[Transparent](references/principles/transparent.md)|No deceptive patterns, honest conduct, aims stated openly|

### references/patterns/ (28 surfaces)
- Each file opens w/ its scope + laws/principles behind it; each entry = `### <decision to make>` w/ `When` / `Do` / `Avoid` / `Why` / `Case` (where documented) / `Hypothetical`.
- [Pattern catalog](references/patterns/index.md): how entries get built, rules for applying them, how to pick files touched by screen.

Usability surfaces:
- [Navigation and menus](references/patterns/navigation-and-menus.md): order, grouping, depth + visibility of nav bars, menus, long lists, links + Back, voice menus.
- [Calls to action and touch targets](references/patterns/calls-to-action-and-touch-targets.md): main action + button hierarchy; target size, spacing, reach + placement; hide vs disable.
- [Forms and data entry](references/patterns/forms-and-data-entry.md): fields, formats, defaults, validation timing, checkout, payment failure, accessible errors.
- [Onboarding and first use](references/patterns/onboarding-and-first-use.md): first session + first week: no-tour start, in-context guidance, empty states, first success, re-engagement nudges.
- [Search and results](references/patterns/search-and-results.md): query entry, suggestions, filter placement, result speed + layout, facets, zero results.
- [Lists, options and choice](references/patterns/lists-options-and-choice.md): how many options, what order, side-by-side comparison, pricing tiers, first number + frame.
- [Layout, grouping and hierarchy](references/patterns/layout-grouping-and-hierarchy.md): grouping cues, spacing scale, containers, emphasis, reading path, icon labels.
- [Dashboards and data displays](references/patterns/dashboards-and-data-displays.md): dense data screens: what to show + priority order, comparison, review checks, chart color, loading + refresh.
- [Feedback, loading and performance](references/patterns/feedback-loading-and-performance.md): indicator per expected wait (spinner, skeleton, progress bar), response-time budgets, stable layout, announcing changes.
- [Progress, goals and completion](references/patterns/progress-goals-and-completion.md): multi-step completion: progress display, honest head starts, near sub-goals, carrying information between steps.
- [Errors and input tolerance](references/patterns/errors-and-input-tolerance.md): prevention + recovery, tolerant input, real + extreme content, destructive actions, failure messages.
- [Complexity management](references/patterns/complexity-management.md): complexity's carrier, progressive disclosure, settings pages, expert tools.
- [First impressions and aesthetics](references/patterns/first-impressions-and-aesthetics.md): what visual polish buys, what it hides, contrast + high-stress screens.
- [Departing from convention](references/patterns/departing-from-convention.md): when to follow convention, when + where to break it, learning curves, redesign rollout.
- [Memorable moments and endings](references/patterns/memorable-moments-and-endings.md): mapping peaks, designing flow endings + exits, neutralizing failure moments.
- [AI and automated features](references/patterns/ai-and-automated-features.md) (usability + humane): generated answers, agents, automation hand-over, sources + uncertainty, human review, fairness.

Humane topics:
- [Notifications and interruptions](references/patterns/notifications-and-interruptions.md): what may interrupt, when, on what channel + controlled by whom.
- [Feeds, scrolling and pacing](references/patterns/feeds-scrolling-and-pacing.md): stopping points, infinite scroll vs load more, autoplay, variable rewards, session length.
- [Defaults and choice architecture](references/patterns/defaults-and-choice-architecture.md): preselection, opt-in, decline as visible as accept, leaving as easy as joining.
- [Friction, undo and confirmation](references/patterns/friction-undo-and-confirmation.md): confirmation scaled to consequence, undo windows, step-up checks, speed bumps.
- [Recommendations and personalization](references/patterns/recommendations-and-personalization.md): ranked feeds, steering levers, explanations, rabbit holes, sensitive states.
- [Privacy, data and security](references/patterns/privacy-data-and-security.md): data minimisation, consent, access + deletion, purpose limits, tracking, ads.
- [Calm technology and device etiquette](references/patterns/calm-technology-and-device-etiquette.md): peripheral attention, quiet signals, staying unobtrusive, failing gracefully.
- [Inclusive and accessible design](references/patterns/inclusive-and-accessible-design.md): persona spectrum, accessibility floors, low-end devices + slow links, identity fields.
- [Safety and abuse resistance](references/patterns/safety-and-abuse-resistance.md): misuse cases, tracking safeguards, blocking + reporting, moderation, children + vulnerable people.
- [Transparency and honesty](references/patterns/transparency-and-honesty.md): disclosing data use + revenue, explaining ranking algorithm, controls doing what they say, true cost up front, honesty tests.
- [Monetization and growth](references/patterns/monetization-and-growth.md): revenue model, free tiers + paywalls, virtual currency, paid random rewards, referrals.
- [Habits, streaks and gamification](references/patterns/habits-streaks-and-gamification.md): streaks, counters, ladders, rewards, usage reports + their effect on vulnerable people.

### references/ethics/
- [Deceptive patterns](references/ethics/deceptive-patterns.md): named dark patterns grouped by area (exit + billing, price + basket, wording + controls, data + consent, pressure) + grey zone; how each works, its harm + honest alternative.
- [Attention hijacks](references/ethics/attention-hijacks.md): ten levers taking attention against person's interest + counter to each.
- [Persuasion asymmetries](references/ethics/persuasion-advantages-of-systems.md): six advantages held by system over face-to-face persuader + counterweight to each; second audit after deceptive-pattern names.
- [Influence vs manipulation](references/ethics/influence-vs-manipulation.md): line-drawing tests: does lever serve person or exploit them.
- [Using psychology responsibly](references/ethics/using-psychology-responsibly.md): guardrails for any psychological lever used to raise engagement, w/ well-being cases.
- [Anti-patterns and humane alternatives](references/ethics/anti-patterns-and-humane-alternatives.md): fast lookup of common harmful patterns + what to ship instead.
- [Ethics review workflow](references/ethics/ethics-review-workflow.md): checkpoints + steps of pre-launch ethics review, objections, watch-list phrases.

### references/checklists/
- [Usability review](references/checklists/usability-review.md): yes/no questions by theme, each tied to law; "no" on question answerable from artifact itself = finding.
- [Usability heuristics map](references/checklists/usability-heuristics-map.md): ten classic usability heuristics → laws behind each; fallback when no law explains problem.
- [Humane-design audit](references/checklists/humane-design-audit.md): yes/no questions per humane principle + block on AI + automation.
- [Calm-technology scorecard](references/checklists/calm-technology-scorecard.md): scores attention, notifications, privacy, well-being + failure states.
- [Interruption decision rules](references/checklists/interruption-decision-rules.md): send test, urgency → modality, timing + etiquette for any interruption.

### references/methods/
- [Methods index](references/methods/index.md): every method by group + its stage of work.

Measurement:
- [Thresholds and formulas](references/methods/thresholds-and-formulas.md): measurable form of each law (response-time limits, target sizes, formulas), each w/ its origin.
- [Pareto chart](references/methods/pareto-chart.md): ranking pages, features or problems by impact share to set priorities.
- [Top tasks and user-by-problem matrix](references/methods/top-tasks-and-user-problem-matrix.md): finding the few tasks + problems mattering most.
- [Measuring flow](references/methods/measuring-flow.md): observation, validated scales + experience sampling to check challenge against skill.

Design process:
- [Lightening mental effort](references/methods/lightening-mental-effort.md): steps to cut extraneous load from screen or flow.
- [Mapping memory demands](references/methods/mapping-memory-demands.md): find each point where flow makes people remember → move it into interface.
- [Gestalt layout pass](references/methods/gestalt-layout-pass.md): settle grouping cues before styling.
- [Object-oriented UX](references/methods/object-oriented-ux.md): map objects in people's model before drawing screens.
- [Cutting to essentials](references/methods/cutting-to-essentials.md): Occam's Razor applied to screen: simplify w/o losing function.
- [Design critique](references/methods/design-critique.md): recurring critique session keeping goals apart from solutions.
- [Team design principles](references/methods/team-design-principles.md): turning laws into principles a team can use, w/o overstating law.
- [Convention or new pattern](references/methods/convention-or-new-pattern.md): whether new pattern earns its learning cost.
- [Teaching inside the task](references/methods/teaching-inside-the-task.md): onboarding for people skipping manuals: learning by doing.
- [Activation moment](references/methods/activation-moment.md): locating first real success + measuring time to value.
- [Peaks and endings](references/methods/peaks-and-endings.md): journey map → shaping peaks, waits, failures + end.
- [Behavioral insight to tested change](references/methods/behavioral-insight-to-tested-change.md): observed behavior → hypothesis → experiment before rollout.
- [Who absorbs complexity](references/methods/who-absorbs-complexity.md): Tesler's Law applied: allocating irreducible complexity between system + person.
- [Testing touch layouts](references/methods/testing-touch-layouts.md): testing targets under real grip, devices + context.

Foresight:
- [Second-order thinking](references/methods/second-order-thinking.md): what happens at full adoption + on whom cost falls.
- [Futures wheel](references/methods/futures-wheel.md): consequences of change, mapped in rings → mitigation + early-warning signal.
- [Premortem](references/methods/premortem.md): imagine launch already failed → reason back to causes.
- [Misuse-case brainstorming](references/methods/misuse-case-brainstorming.md): misuse case per use case, vulnerable-group prompts, tests on real build.
- [Four quadrants of design responsibility](references/methods/four-quadrants-of-responsibility.md): what gets built vs whom it affects, beyond single user.
- [Three-gate check](references/methods/three-gate-check.md): three gates in fixed order before building or releasing.

Metrics:
- [Counter-metrics](references/methods/counter-metrics.md): pair each growth metric w/ harm it could hide + what to do when it trips.
- [Measure what you value](references/methods/measure-what-you-value.md): metrics reflecting value to people, not activity alone.
- [Goals, signals, metrics](references/methods/goals-signals-metrics.md): goal in people's words → observable signal → number.
- [Reading experiments honestly](references/methods/reading-experiments-honestly.md): why short tests favor frictionless variant + habits keeping tests honest.
- [Engagement vs empowerment metrics](references/methods/engagement-vs-empowerment-metrics.md): telling capture metrics from benefit metrics.

Arguing and team practice:
- [Stakeholder arguments](references/methods/stakeholder-arguments.md): argument structures for usability + humane choices, common objections.
- [Debiasing](references/methods/debiasing.md): countering bias in research, reviews, reports + team's own judgment.
- [Process safeguards](references/methods/process-safeguards.md): three safeguards: fix flow behind refunds, change floor when competition causes harm, stage risky rollouts w/ withdrawal condition written first.
- [Team and personal practices](references/methods/team-and-personal-practices.md): habits keeping team + each practitioner able to choose humanely.

### references/evidence/
- Each law's evidence lives in its own file's `Evidence` section; humane-design evidence lives here, one file per theme.
- [Stating evidence](references/evidence/stating-evidence.md): how to state study, figure, case or origin accurately.
- [Citation caveats](references/evidence/citation-caveats.md): known traps: contested numbers, misattributions, misdatings, limits of each body of evidence.
- [Product cases](references/evidence/product-cases.md): real product cases of laws in use + each story's strength.
- [Attention and distraction](references/evidence/attention-and-distraction.md): interruption cost, phone checking, notification load.
- [Addiction and variable rewards](references/evidence/addiction-and-variable-rewards.md): compulsion loops, variable rewards, engineered engagement, time lost.
- [Children and adolescents](references/evidence/children-and-adolescents.md): effects on minors, sleep, data, age-appropriate defaults.
- [Decision fatigue and choice](references/evidence/decision-fatigue-and-choice.md): decision fatigue, option-set size, defaults, loss aversion, framing.
- [Personalization and surveillance](references/evidence/personalization-and-surveillance.md): tracking, inference, data markets, breaches, repurposed data.
- [Filter bubbles and polarization](references/evidence/filter-bubbles-and-polarization.md): what ranking + personalization do to exposure, belief + discourse.
- [Unintended consequences](references/evidence/unintended-consequences.md): second-order effects of products at scale on cities, non-users + fragile contexts.
- [Safety and abuse](references/evidence/safety-and-abuse.md): harassment, stalking + intimate-partner abuse carried out via products.
- [Convenience and friction](references/evidence/convenience-and-friction.md): effect of removing or adding step, pause or delay.
- [Inclusion and exclusion costs](references/evidence/inclusion-and-exclusion-costs.md): people left out + what exclusion costs or inclusion returns.
- [Business cost of deception](references/evidence/business-cost-of-deception.md): fines, refunds, churn + lost trust from deceptive patterns.

### references/guides/
- [Core stance](references/guides/core-stance.md): how to hold all this: laws as heuristics, people over metrics, rights over effort over delight, when knowledge does not apply.
- [Design a screen or flow](references/guides/design-a-screen-or-flow.md): numbered steps bringing laws + principles into new design, each tagged usability or humane pass.
- [Review an interface](references/guides/review-an-interface.md): numbered steps for usability + humane review of something existing.
- [How deep to go](references/guides/how-deep-to-go.md): quick pass vs standard review vs full treatment, + what each must deliver.
- [Defend a decision](references/guides/defend-a-decision.md): rationale built from problem, law w/ origin year + mechanism, evidence, change + its metric.
- [Answer an ethics question](references/guides/answer-an-ethics-question.md): reasoning steps when asked if product decision acceptable.
- [Write a finding](references/guides/write-a-finding.md): fixed shape, confidence labels + severity ranking of finding, law-based + principle-based, w/ hypothetical worked findings.
- [Symptom-to-fix index](references/guides/symptom-to-fix-index.md): observed problem → candidate law → fix.
- [Common mistakes](references/guides/common-mistakes.md): most damaging misuses of this knowledge, usability + humane side.
- [Law misapplications](references/guides/law-misapplications.md): every wrong use of each law w/ its correction.
- [Laws and principles crosswalk](references/guides/laws-and-principles-crosswalk.md): lever each law offers, how it gets turned against people, principle bounding it.

### references/lookup/
- [Misquoted claims](references/lookup/misquoted-claims.md): what each law or finding often gets misquoted, misdated or misread as vs what got shown + when.
- [Timeline](references/lookup/timeline.md): date order of research behind laws + foundational works of humane design, by year + kind of work.
- [Humane-design ideas](references/lookup/humane-design-ideas.md): key concepts, claims + dates of humane design by theme (calm technology, persuasion, surveillance, augmentation, inclusion, ethics).
- [Organizations and toolkits](references/lookup/organizations-and-toolkits.md): groups, toolkits, frameworks + movements working on humane technology, picked by need.
- [Glossary](references/lookup/glossary.md): usability + humane-design terms, A to Z.

## Notation
One shared notation across every file.

|Sign|Means|
|---|---|
|`→`|leads to, so, then|
|`=`|is, means|
|`+`|and|
|`/`|or|
|`~`|about|
|`≥` / `≤`|at least / at most|
|`<` / `>`|less than / more than|
|`↑`|same as table cell directly above|
|`vs`|versus|
|`w/` / `w/o`|with / without|
|`e.g.`|marks example|
|`Case:`|documented real event, decision or result|
|`Hypothetical:`|invented illustration; claims no real result|

- Negation always written as word (not, never, no, avoid, without), never as symbol.
- Short forms (e.g. RT, WM) spelled out at first use in each file.
- Bare file paths ending in `.md` = references to other files of this base, relative to file holding them; open them like links.
- Hedges (may, about, tends to, one study, contested) = part of claim; carry over unchanged.
