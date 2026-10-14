# Laws and principles crosswalk

## Use when

- Design leans on psychological lever.
- Fix on one side (usability / humane) may break other side.
- Need other half's file for product surface.

Gives: per usability law → its lever, its misuse against people, bounding humane principle, file w/ honest alternative. Per humane principle → psychological laws behind its practices. Per product surface → usability + humane files to read together.

## Two halves, one design

|Half|Contents|Answers|Index|
|---|---|---|---|
|Usability|30 psychology-based laws on how people perceive, remember, attend, decide + move|can people use it?|../laws/index.md|
|Humane|seven principles (Respectful, Finite, Empowering, Intentional, Inclusive, Resilient, Transparent) on what product does to people's attention, time, agency, safety + trust|good for them?|[principles index](../principles/index.md)|

- One design must answer both questions; passing one never answers the other.
- Effortless to use, not good for people:
  - Hypothetical: bank account opened fully in app, closable only at branch (roach motel).
  - Hypothetical: language-learning app rolls straight from lesson to lesson w/o pause → moment of choosing to stop never comes.
  - Hypothetical: fitness tracker's playful mascot onboarding glides past screen switching on location-history sharing.
- Well-meant, not usable: handsome interface fighting perception, memory, attention + decision-making still fails.
- Over-correcting fails too: confirmations on trivial actions train people to click through; confirmation added everywhere → nagging; safety alerts added as fix → alert fatigue.

## The line-drawing test

- Same lever, two directions: compulsive products can come about when knowledge making products intuitive gets turned to preying on minds.
- Defaults, emphasis, grouping, progress displays, speed + polish: each helps when serving person's goal; each harms when serving goal person would reject.
- Test: influence = serves goal user already holds; manipulation = serves goal user would reject if they saw it.
- Ask: whose goal served? Would person endorse influence if they understood it?
- Lever-by-lever table, legitimate influence vs manipulation → ../ethics/influence-vs-manipulation.md. Psychology guardrails, all surfaces → ../ethics/using-psychology-responsibly.md.
- Resilient states pairing directly: abusability = successor to usability; evaluate w/ same rigor usability gets.

## Combining the halves

1. Usability pass: laws + usability pattern files → can people see structure, hold what task needs, notice what matters, decide, act + recover?
2. Humane pass: principles, humane pattern files + ethics tests → for each lever pulled: its law-table row below → bounding principle → file w/ honest alternative.
3. Conflicts → ranking: human rights (privacy, security, accessibility) first → people's time + effort → delight last.
   - Shortcut, speed gain / polish never outranks privacy, security / accessibility.
   - Delight never outranks people's time + effort.
   - Findings + severities ordered same way.
4. Check neighbours: satisfying one principle often quietly breaks another → check each principle's "Also check" set.
5. Law = heuristic to weigh, never mandate. User research + project data outrank any law.

Full step sequences, every step tagged usability / humane pass: design-a-screen-or-flow.md (new design), review-an-interface.md (existing). Stance + ranking: core-stance.md.

## How to read the law rows

- One table per law theme; every one of 30 laws has own row.
- Lever = what lever does for people = legitimate use of law.
- Turned against people = misuse recorded for lever.
- Bounded by = principle(s) whose practices set limit.
- Read = file w/ honest alternative; "(… entry)" = entry holding it inside listed file.
- Deceptive-pattern names follow [deceptive-pattern taxonomy](../ethics/deceptive-patterns.md); attention-hijack names follow ../ethics/attention-hijacks.md; each name pairs w/ its honest alternative in those tables.
- "No abuse case recorded" = no deliberate misuse of lever written down; not claiming none exists → apply general line-drawing test (../ethics/influence-vs-manipulation.md) + still check named principle.
- "Law file records no abuse case" = misuse comes from humane side (ethics / pattern file named in row), not from law's own file.

## Law → principle: perception and grouping

Shared guardrail, all five laws: emphasis, grouping + defaults steer choice → steer toward user's goal (../ethics/using-psychology-responsibly.md). Shared background: ../laws/gestalt-principles-overview.md.

|Law|Lever|Turned against people|Bounded by|Read|
|---|---|---|---|---|
|../laws/common-region.md|border / background fill → enclosed items read as one group, related to each other, not neighbours|no abuse case recorded → general test. Recorded accidental failures: misplaced boundary splits real groups; full-width contrasting band = false floor → people think page ended, stop scrolling|../principles/transparent.md: grouping + styling must not mislead|../ethics/using-psychology-responsibly.md; ../patterns/layout-grouping-and-hierarchy.md|
|[Law of Prägnanz](../laws/pragnanz.md)|simple shapes + compositions read w/ least effort; one ordered form aids memory + prevents overload|no abuse case recorded → general test|../principles/inclusive.md: visual style must not undercut accessibility floors (contrast, text, icons)|../patterns/first-impressions-and-aesthetics.md; ../patterns/inclusive-and-accessible-design.md|
|../laws/proximity.md|tight gaps within groups + larger between → structure read from spacing; spacing = cheapest grouping cue|no abuse case recorded → general test. Recorded accidental failures: unrelated items together camouflage each other (people inspect one item of perceived group, infer rest); optional Skip far from main actions missed → people believe account creation mandatory|../principles/empowering.md: decline + skip get same size, contrast + position as accept; ../principles/transparent.md: grouping must not mislead|../patterns/defaults-and-choice-architecture.md (equal-weight No entry); ../patterns/layout-grouping-and-hierarchy.md|
|../laws/similarity.md|look-alike items read as one kind → consistent styling shows interactive items + what belongs together|law file records no abuse case, only accidental false groups: non-clickable elements styled like links; icon set falsely implying certain icons related; how-to video sized like surrounding display ads → missed. On purpose (humane side): disguised ads = ads styled as content, navigation / download buttons|../principles/transparent.md: ads unmistakably ads; ../principles/inclusive.md: color-signalled groups need accessibility floors, e.g. color-blind-safe palette|[deceptive-pattern taxonomy](../ethics/deceptive-patterns.md); ../patterns/transparency-and-honesty.md (ads-unmistakably-ads entry); ../patterns/inclusive-and-accessible-design.md|
|../laws/uniform-connectedness.md|lines, arrows, frames + shared color tie related elements; connecting border also raises enclosed content's perceived priority|no abuse case recorded → general test. Recorded caution: border = emphasis → reserve for content deserving it; check guardrails before raising priority w/ border|../principles/transparent.md: highlighting = claim, must hold true|../ethics/using-psychology-responsibly.md; emphasis misuse → Von Restorff Effect row (attention and salience)|

## Law → principle: memory and cognition

|Law|Lever|Turned against people|Bounded by|Read|
|---|---|---|---|---|
|../laws/millers-law.md|chunk content to fit immediate-memory span, about 7 ± 2 items (later research argues span nearer 4 items than 7 ± 2); chunked layouts = accessibility aid, not mere convenience|no abuse case recorded → general test. Recorded misuse = misapplication, not manipulation: treating "seven" as cap on menu / list length|../principles/inclusive.md: memory capacity differs by person, lower for children + older adults|../patterns/inclusive-and-accessible-design.md; law-misapplications.md|
|../laws/working-memory.md|inputs, visited states + comparisons kept visible → people recognize instead of recall; memory burden moves to system|no abuse case recorded → general test. Crowded working memory degrades choices, not only recall; flow judged by team's own ease overloads typical users' working memory|../principles/inclusive.md: capacity cut by stress + sleep loss, falls w/ age; memory demands = accessibility issue|../patterns/inclusive-and-accessible-design.md (account-for-anxiety-and-emotional-state entry)|
|../laws/chunking.md|content split + regrouped into meaningful units (modules, headings, formatted strings) → easier to scan; more held per chunk|no abuse case recorded → general test. People remember own summary / label + later fill in fitting details → UI label on item, state / chart shapes later memory → names + summaries must stay accurate|../principles/inclusive.md: what counts as chunk varies w/ language, culture + prior knowledge; ../principles/transparent.md: accurate labels + summaries|../ethics/using-psychology-responsibly.md; ../patterns/inclusive-and-accessible-design.md|
|../laws/cognitive-load.md|cut extraneous load: drop non-essentials, common patterns, editable defaults, data reuse, fewer choices, labelled icons → capacity left for task|decision removed by default = decision made for person; default never neutral. Misuse: self-serving defaults; long, complex choice up front → people give up + accept preselection; all friction removed for conversion, incl. load-bearing effort carrying deliberation, ownership / learning|../principles/intentional.md: defaults chosen for well-being + withheld where active choice matters; friction kept on purpose. ../principles/inclusive.md: headroom for stressed, anxious + low-income users|../patterns/defaults-and-choice-architecture.md; ../patterns/friction-undo-and-confirmation.md; ../evidence/convenience-and-friction.md evidence|
|../laws/serial-position-effect.md|key items first + last, where best recalled in lists met only once (spoken menus, onboarding steps). Option sets needing neutrality (survey answers, vendor lists) → rotate / randomize order|position alone creates preference: 1998 ballot-order study found first-listed candidates gained small but statistically significant vote bump. First items frame how later ones read. Misuse: order steering where option set should stay neutral; leading w/ outlier instead of representative, accurate information; interstitials / promotional modals between showing something + using it erase what person held in mind|../principles/transparent.md + ../principles/empowering.md: explain what orders what people see + let them steer it; ../principles/respectful.md: what interrupts + when|../ethics/influence-vs-manipulation.md; ../patterns/recommendations-and-personalization.md; ../patterns/notifications-and-interruptions.md|

## Law → principle: attention and salience

|Law|Lever|Turned against people|Bounded by|Read|
|---|---|---|---|---|
|../laws/selective-attention.md|strong cue, one change at a time + content visually unlike ads → what matters noticed, rest filtered|attention taken against person's interest via instant interruption: everything buzzes on arrival because interrupting pays sender better than waiting; other ../ethics/attention-hijacks.md; disguised ads convert inattention into agreement. 2012 consumer-choice experiments: at fast decision speeds, visual salience swayed choice more than preference, most of all when brand preference weak → salience in fast choices acts as default|../principles/respectful.md; ../principles/transparent.md: ads unmistakably ads|../ethics/attention-hijacks.md + their counters; ../patterns/notifications-and-interruptions.md; ../evidence/attention-and-distraction.md evidence|
|../laws/von-restorff-effect.md|one distinct item per area stands out + gets remembered → primary action / key information found; distinctness helps people spot option fitting their goal|salience pushes business's option over user's, esp. in quick decisions w/ weak preference; misdirection: emphasis draws eye to pricier / more data-hungry option; hidden No: decline option shrunk, greyed / missing|../principles/transparent.md: highlighting = claim, must hold true; ../principles/empowering.md: equal-weight No; ../principles/inclusive.md: contrast beyond color + motion (contrast only by color / only by motion excludes people w/ low vision, color vision deficiency / motion sensitivity)|[deceptive-pattern taxonomy](../ethics/deceptive-patterns.md); ../patterns/defaults-and-choice-architecture.md (equal-weight No entry); ../patterns/inclusive-and-accessible-design.md; ../ethics/influence-vs-manipulation.md|
|../laws/zeigarnik-effect.md|unfinished tasks stay in mind → signal more content exists, show clear progress, make started-then-left tasks easy to resume / dismiss|manufactured incomplete tasks / endless loops pulling people back = engagement dark pattern; cliffhangers, autoplay + ellipsis teasers drive compulsive return; permanent nag meters; completion meters turned compulsion loops; inflated progress. Named hijacks: bottomless bowl + autoplay; bottomless feed|../principles/finite.md; ../principles/intentional.md|../patterns/feeds-scrolling-and-pacing.md; ../patterns/progress-goals-and-completion.md (let-users-close-open-loops entry); ../patterns/habits-streaks-and-gamification.md; ../evidence/addiction-and-variable-rewards.md evidence|
|../laws/flow.md|low friction, feedback on each action + challenge matched to skill → absorption in person's own goal, w/ natural stopping points|endless scroll + long sessions labelled flow while absorption serves time-on-site, not user's goal = capture, not flow. 2021 critique of flow: its mechanics turn play into unpaid work / trap people in hyperfocus|../principles/finite.md; ../principles/intentional.md|../patterns/feeds-scrolling-and-pacing.md; ../patterns/habits-streaks-and-gamification.md; ../ethics/influence-vs-manipulation.md|

## Law → principle: decisions and simplicity

|Law|Lever|Turned against people|Bounded by|Read|
|---|---|---|---|---|
|../laws/hicks-law.md|fewer options per step, long choice sequences split, one recommended option → faster decisions where speed matters|recommended option as license to hide essentials; menu control: whoever writes options frames question; choice feels free while alternatives never appear; recommendation / default picked for business, not what most people would choose if fully informed|../principles/empowering.md: audit omissions, full catalog one tap away; ../principles/intentional.md: default = recommendation you would defend aloud|../patterns/defaults-and-choice-architecture.md; ../ethics/attention-hijacks.md + their counters; ../evidence/decision-fatigue-and-choice.md evidence|
|../laws/choice-overload.md|one featured item, search + filters, side-by-side comparison → large sets stop overwhelming people|decoys + phantoms on comparison / pricing pages: deliberately weak middle / anchor tier pushing higher-margin plan = manipulation; spec tables making trivial differences look decisive; set narrowed so alternatives hidden. Named patterns for these pages: price comparison prevention, confusopoly|../principles/empowering.md: curate w/o hiding catalog; ../principles/transparent.md: plain, comparable plans, all tiers priced in same units at same moment|../patterns/lists-options-and-choice.md (compare-against-the-user's-criteria-not-a-decoy entry); [deceptive-pattern taxonomy](../ethics/deceptive-patterns.md); ../patterns/recommendations-and-personalization.md; ../evidence/decision-fatigue-and-choice.md evidence|
|../laws/cognitive-bias.md|knowing mental shortcuts (anchoring, framing, status quo + defaults, loss aversion) → design around them to protect people; also guards team's own decisions|status quo bias for conversion: pre-checked add-ons, self-serving opt-outs, buried settings; loss aversion for conversion: multi-step cancel flow w/ guilt-laden / loss-framed retention copy (can backfire, provoking reactance); anchoring: struck-through reference prices + first amounts shown only to inflate spending. Named patterns: sneak into basket, opt-out defaults + pre-ticked consent, roach motel, confirmshaming|../principles/transparent.md; ../principles/intentional.md (default effect); ../principles/empowering.md (leaving as easy as joining)|[deceptive-pattern taxonomy](../ethics/deceptive-patterns.md); ../patterns/defaults-and-choice-architecture.md; ../patterns/transparency-and-honesty.md (run-the-if-they-knew-test entry); ../ethics/influence-vs-manipulation.md|
|../laws/occams-razor.md|start w/ simplest design, drop non-functional elements → less to process; any element still cuttable → design not finished|law file records no abuse case; own pitfall = removing things at cost of function. Simplification misuse recorded on humane side: steps removed for conversion, incl. step where deliberation, learning / ownership happens; one-tap irreversible actions remove pause protecting against impulse, accident + regret|../principles/intentional.md: friction on purpose, confirmation effort scaled to severity|../patterns/friction-undo-and-confirmation.md (design-for-the-effort-that-builds-meaning entry); ../evidence/convenience-and-friction.md evidence|
|../laws/pareto-principle.md|invest first where most users gain most; split approximate|no manipulation case recorded; recorded misuse = exclusion: remaining 80% ignored; "trivial many" read as worthless; a few metrics over-optimized at expense of others; heavy barriers stay because people meeting them not counted as part of market|../principles/inclusive.md|../evidence/inclusion-and-exclusion-costs.md evidence; ../patterns/friction-undo-and-confirmation.md (ask-whose-friction-you-are-removing entry); ../methods/counter-metrics.md|

## Law → principle: motor control and time

|Law|Lever|Turned against people|Bounded by|Read|
|---|---|---|---|---|
|../laws/fittss-law.md|large, well-spaced targets near task focus → fast, accurate action|law file records no abuse case; own risk = irreversible action directly beside positive one. Size + position misused on purpose (humane side): hidden No, decline shrunk, greyed / missing, e.g. tiny grey "no" beside bright accept|../principles/empowering.md: decline + skip get same size, contrast + position as accept; ../principles/inclusive.md: size floors + keyboard access = accessibility floors; ../principles/intentional.md: confirmation graded by consequence for destructive + irreversible actions|../patterns/defaults-and-choice-architecture.md (equal-weight No entry); [deceptive-pattern taxonomy](../ethics/deceptive-patterns.md); ../patterns/inclusive-and-accessible-design.md; ../patterns/friction-undo-and-confirmation.md|
|../laws/doherty-threshold.md|response under 400 ms (popular threshold) + real progress cue for slower work → neither person nor machine kept waiting; focus kept|apps responding under 400 ms once characterized as addicting: reported characterization, not measured finding; deserves scrutiny. Misuse: speed tuned for compulsion; artificial delay inflating perceived value of trivial work; progress bar deliberately misrepresenting progress. Progress bars help even when inaccurate → honest progress = choice|../principles/transparent.md: no faked progress / faked effort; ../principles/intentional.md: zero + excessive friction both destroy value; ../principles/finite.md: compulsive use|../ethics/influence-vs-manipulation.md; ../ethics/using-psychology-responsibly.md; ../evidence/convenience-and-friction.md evidence|
|../laws/parkinsons-law.md|beat expected duration w/ autofill, data reuse + short purchase / booking flows; firm, realistic time boxes|no abuse case recorded → general test. Recorded bound on cutting steps for speed: explicit confirmation stays before money moves / content shared|../principles/intentional.md|../evidence/convenience-and-friction.md evidence; ../patterns/friction-undo-and-confirmation.md|
|../laws/goal-gradient-effect.md|remaining steps shown + small, truthful head start → effort rises as goal nears → tasks people want done get finished|illusory progress toward outcomes people did not choose (fake progress, inflated totals); threshold quietly raised by bonus size; finish lines moved for business goals over user's; targets ratcheting upward → nobody ever finished; near-goal window used to extract consent, raise prices / lock people in. Near goal, people less price-sensitive + more open to promotions: 2006 survey found 56% of people close to goal vs 38% of others accepted weekly marketing emails for bonus miles|../principles/intentional.md; ../principles/finite.md: no never-closing loops / moved finish lines; ../principles/transparent.md: progress shown = real completed steps / genuine gift|../patterns/habits-streaks-and-gamification.md; ../patterns/progress-goals-and-completion.md (grant-a-head-start-honestly entry); ../ethics/influence-vs-manipulation.md; ../ethics/using-psychology-responsibly.md|

## Law → principle: expectations and emotion

|Law|Lever|Turned against people|Bounded by|Read|
|---|---|---|---|---|
|../laws/jakobs-law.md|conventions by default → people reuse what they learned elsewhere; novelty only for stated, tested purpose; redesigns opt-in|copying widespread deceptive / slow pattern on grounds of convention = misuse: convention transfers learning, not approval. Breaking convention to trick people = bait and switch (Hypothetical: workplace tool's terms-update dialog; button in usual "Remind me later" spot accepts new terms). Reverse misuse: novelty hides intent; format people have not met before reads as neutral → persuasion inside arrives unexamined|../principles/transparent.md: controls do what their label says; ../principles/inclusive.md: convention = default to verify w/ people it might exclude|[deceptive-pattern taxonomy](../ethics/deceptive-patterns.md); ../patterns/transparency-and-honesty.md (controls-do-exactly-what-their-label-says entry); ../ethics/persuasion-advantages-of-systems.md (six advantages system holds over human persuader); ../patterns/inclusive-and-accessible-design.md (treat-a-convention-as-a-default-to-check entry)|
|../laws/mental-model.md|match users' model, not team's → system behaves as people predict|trust a model carries used against its holder: online cart inherits store rule of shopper alone deciding what goes in, then paid extra silently pre-added = sneak into basket. Case: luggage retailer pre-added $8.25 shipping-protection toggle to cart, on by default|../principles/transparent.md + ../principles/intentional.md: no preselection where money / consent decided|[deceptive-pattern taxonomy](../ethics/deceptive-patterns.md); ../patterns/defaults-and-choice-architecture.md; ../patterns/forms-and-data-entry.md (default-paid-add-ons-to-off entry)|
|../laws/aesthetic-usability-effect.md|polish → leniency toward small flaws, design judged easier to use, favorable reaction; earns goodwill|polish hides problems people pay for later; smoother-to-process content judged more correct regardless of accuracy → polish can make weak / false content credible; used as excuse for low contrast; charming animation over opaque data practices|../principles/transparent.md: polish must not hide what matters; ../principles/inclusive.md: accessibility floors visual style must not undercut|../ethics/influence-vs-manipulation.md; ../patterns/first-impressions-and-aesthetics.md (keep-beauty-from-costing-legibility entry); ../patterns/transparency-and-honesty.md; ../patterns/ai-and-automated-features.md (do-not-let-the-container-vouch-for-the-content entry)|
|../laws/peak-end-rule.md|peak + ending designed on purpose, negative peaks planned for (waits, errors, payment declines) → real value = what gets remembered|endings manufactured to cover bad experience; bad flow padded / lengthened to game recall (nicer memory does not justify extra real cost); hooks on way out: exit-intent please-don't-go pop-ups, discounts + upsells at cancellation, logout / leaving; artificial delight added to moments not already valuable|../principles/finite.md: experience has edges + clean ending; ../principles/empowering.md (leaving as easy as joining); ../principles/transparent.md|../patterns/memorable-moments-and-endings.md (end-well entry); ../patterns/defaults-and-choice-architecture.md (symmetric-exit entry); ../ethics/influence-vs-manipulation.md|

## Law → principle: complexity and robustness

|Law|Lever|Turned against people|Bounded by|Read|
|---|---|---|---|---|
|../laws/teslers-law.md|system carries irreducible complexity (defaults, suggestions, data reuse, automation, progressive disclosure) → less left for person's head + hands|calling burden irreducible so users keep carrying it; control removed → system decides silently: hidden automation w/ no system-state feedback, no failure path, decisions no one can question / overturn; carried defaults chosen for system, not person. People's agency diminished when systems decide silently|../principles/empowering.md: human in the loop: can review, correct, approve + appeal; ../principles/intentional.md: defaults chosen for well-being|../patterns/ai-and-automated-features.md; ../patterns/defaults-and-choice-architecture.md; ../patterns/complexity-management.md|
|../laws/postels-law.md|clear feedback + bounds; varied input accepted + normalized when meaning clear → fewer inputs rejected across formats, access methods + capability levels|leniency inside system (not only at human interface) hides defects + can get exploited: 2018 security research showed flexibility in onion-routing anonymity protocol exploitable to compromise both service + client anonymity. Misuse: ambiguous input accepted silently|../principles/resilient.md: abuse taken as given; ../principles/inclusive.md: any input, access method + capability level|../patterns/errors-and-input-tolerance.md; ../patterns/inclusive-and-accessible-design.md|
|../laws/paradox-of-the-active-user.md|contextual help + progressive onboarding instead of front-loaded tours → people learn by doing; value arrives early|instant rewards can exploit present bias in engagement loops. Misuse on first-use surface: forced sign-up before any value delivered; work held hostage (coercive use of effort already invested); confirmshaming on skip / decline; pre-checked marketing consent; notification permission asked at first launch|../principles/intentional.md: quick win weighed against later effects; habits people would endorse. ../principles/transparent.md; ../principles/respectful.md|../ethics/using-psychology-responsibly.md; ../patterns/onboarding-and-first-use.md (keep-onboarding-accessible-and-fair entry); ../patterns/habits-streaks-and-gamification.md|

## Principle → laws

- Each humane practice works because of how people perceive, remember, attend + decide.
- Law named behind principle = mechanism behind practice; not proof practice suffices.
- Practices + audit questions → each principle's own file.

### [Respectful](../principles/respectful.md)

- ../laws/selective-attention.md: attention = limited, goal-directed filter → every interruption competes w/ person's current task; peripheral signals work within this limit.
- ../laws/serial-position-effect.md: 15-30 seconds of unrelated activity erases what person just held in mind → let nothing interrupt between showing something + using it.
- Meets in: ../patterns/notifications-and-interruptions.md; ../patterns/calm-technology-and-device-etiquette.md; ../checklists/interruption-decision-rules.md; ../ethics/attention-hijacks.md + their counters.

### [Finite](../principles/finite.md)

- ../laws/zeigarnik-effect.md: unfinished goal consumes attention; unclosed loops → rumination + clutter → give stopping points + reachable finish.
- ../laws/flow.md: absorption belongs to person's own goal + has natural stopping points; endless scroll not flow.
- ../laws/goal-gradient-effect.md: pull rises near finish line → moved finish lines keep pulling people on.
- ../laws/peak-end-rule.md: ending weighs heavily in remembered judgment → give clean ending.
- ../laws/paradox-of-the-active-user.md (present bias): immediate rewards outweigh later ones.
- Meets in: ../patterns/feeds-scrolling-and-pacing.md; ../patterns/progress-goals-and-completion.md; ../patterns/habits-streaks-and-gamification.md; ../patterns/memorable-moments-and-endings.md.

### [Empowering](../principles/empowering.md)

- ../laws/choice-overload.md + ../laws/hicks-law.md: option count + option-set shape shape decision → curate w/o hiding catalog; audit omissions.
- ../laws/teslers-law.md: control removed → system decides → keep human in the loop w/ inspectable, correctable automation.
- ../laws/cognitive-bias.md: people over-trust automated output (automation bias).
- ../laws/von-restorff-effect.md + ../laws/fittss-law.md: salience, size + position set each answer's ease → give No equal weight.
- ../laws/jakobs-law.md: redesigns opt-in + w/ route back.
- Meets in: ../patterns/defaults-and-choice-architecture.md; ../patterns/recommendations-and-personalization.md; ../patterns/ai-and-automated-features.md; ../patterns/lists-options-and-choice.md; ../patterns/navigation-and-menus.md.

### [Intentional](../principles/intentional.md)

- ../laws/cognitive-bias.md: default effect = inertia + loss aversion + status quo bias → preselected option = likely outcome → default chosen for well-being / withheld.
- ../laws/teslers-law.md + ../laws/cognitive-load.md: step removal moves / removes work; some effort = load-bearing.
- Instant high-stakes operations can feel unsafe; together w/ load-bearing effort → friction-value curve Intentional relies on.
- ../laws/doherty-threshold.md: deliberate delay can raise perceived value + trust; stated principle, no study cited; honesty still applies.
- ../laws/fittss-law.md: keep irreversible actions apart from positive ones.
- ../laws/occams-razor.md: never remove something at cost of function.
- Meets in: ../patterns/friction-undo-and-confirmation.md; ../patterns/defaults-and-choice-architecture.md; ../patterns/errors-and-input-tolerance.md; ../evidence/convenience-and-friction.md evidence.

### [Inclusive](../principles/inclusive.md)

- ../laws/working-memory.md, ../laws/millers-law.md + ../laws/chunking.md: capacity + chunks vary w/ age, stress, language, culture + prior knowledge → memory demands = accessibility issue.
- ../laws/cognitive-load.md: people carry baseline load designers cannot see, e.g. worry, anxiety, financial scarcity.
- ../laws/fittss-law.md: target-size floors + keyboard reach.
- ../laws/postels-law.md: accept any input, access method + capability level.
- ../laws/von-restorff-effect.md + ../laws/similarity.md: meaning never carried by color / motion alone.
- ../laws/aesthetic-usability-effect.md: taste varies w/ culture.
- ../laws/jakobs-law.md: convention verified w/ people it might exclude.
- Meets in: ../patterns/inclusive-and-accessible-design.md; ../patterns/forms-and-data-entry.md (make-errors-perceivable-to-everyone entry); ../patterns/calls-to-action-and-touch-targets.md; ../methods/testing-touch-layouts.md realistically.

### [Resilient](../principles/resilient.md)

- ../laws/postels-law.md: liberal at human interface, strict + validating inside system; leniency can get exploited.
- ../laws/teslers-law.md: automation judged by how it breaks → give failure path + handover.
- ../laws/peak-end-rule.md: failures = negative peaks to plan for.
- ../laws/working-memory.md: stress cuts capacity → simplest flows, visible state, recoverable steps.
- Limit: laws explain only failure + recovery practices; abusability (how easily product lets one person harm another) sits on humane side alone.
- Meets in: ../patterns/errors-and-input-tolerance.md; ../patterns/safety-and-abuse-resistance.md; ../patterns/calm-technology-and-device-etiquette.md (work-even-when-failing entry); ../methods/misuse-case-brainstorming.md.

### [Transparent](../principles/transparent.md)

- ../laws/cognitive-bias.md: status quo bias + loss aversion behind pre-checked add-ons, self-serving opt-outs + subscription traps; anchoring + framing behind price + consent wording.
- ../laws/mental-model.md + ../laws/jakobs-law.md: people act on what controls conventionally do → controls must do what their label says.
- ../laws/aesthetic-usability-effect.md: polish raises credibility independent of accuracy.
- ../laws/goal-gradient-effect.md + ../laws/doherty-threshold.md: progress displays + delays work even when artificial → honesty = choice.
- ../laws/selective-attention.md + ../laws/von-restorff-effect.md: emphasis in quick decisions acts as default → highlighting = claim, must hold true; ads unmistakably ads.
- Meets in: ../patterns/transparency-and-honesty.md; [deceptive-pattern taxonomy](../ethics/deceptive-patterns.md); ../patterns/privacy-data-and-security.md; ../patterns/lists-options-and-choice.md.

## Shared surfaces

- Surface covered from both sides → read usability + humane file(s) together; humane side sets bounds (last column).
- Principles each surface touches first → ../principles/surface-to-principle-map.md.

|Surface|Usability side|Humane side|Humane side bounds|
|---|---|---|---|
|Onboarding + first use|../patterns/onboarding-and-first-use.md; ../methods/teaching-inside-the-task.md (for people skipping manuals); ../methods/activation-moment.md (time to value)|../patterns/notifications-and-interruptions.md; ../patterns/privacy-data-and-security.md; [deceptive-pattern taxonomy](../ethics/deceptive-patterns.md)|re-engagement nudges + permission asks; sign-up, skip / decline + consent steps|
|Defaults, options + choice|../patterns/lists-options-and-choice.md; ../laws/hicks-law.md; ../laws/choice-overload.md|../patterns/defaults-and-choice-architecture.md; ../evidence/decision-fatigue-and-choice.md evidence|recommended option + default: opt-in, equal-weight decline, catalog kept reachable|
|Notifications + attention|../laws/selective-attention.md; ../patterns/feedback-loading-and-performance.md|../patterns/notifications-and-interruptions.md; ../patterns/calm-technology-and-device-etiquette.md; ../checklists/interruption-decision-rules.md; ../ethics/attention-hijacks.md|what interrupts, when, on what channel, under whose control; how loudly changes announced|
|Progress, streaks + gamification|../patterns/progress-goals-and-completion.md; ../laws/goal-gradient-effect.md; ../laws/zeigarnik-effect.md|../patterns/habits-streaks-and-gamification.md; ../ethics/influence-vs-manipulation.md; ../evidence/addiction-and-variable-rewards.md evidence|streaks, counters + rewards + their effect on vulnerable people; illusory progress|
|Feeds, scrolling + stopping points|../patterns/search-and-results.md; ../laws/flow.md|../patterns/feeds-scrolling-and-pacing.md; ../patterns/recommendations-and-personalization.md|stopping points, infinite scroll + autoplay; where open loops turn into capture|
|Endings, cancellation + exit|../patterns/memorable-moments-and-endings.md; ../methods/peaks-and-endings.md method|../patterns/defaults-and-choice-architecture.md (symmetric-exit entry); [deceptive-pattern taxonomy](../ethics/deceptive-patterns.md); ../principles/finite.md|leaving as easy as joining; no hooks on way out|
|AI + automated features|../patterns/ai-and-automated-features.md (one file carrying both Laws line + Principles line); ../patterns/complexity-management.md; ../methods/who-absorbs-complexity.md|same AI pattern file; ../checklists/humane-design-audit.md (its AI + automation questions); ../ethics/persuasion-advantages-of-systems.md (six advantages system holds over human persuader)|hand-over, uncertainty, human review, appeal, disclosing system's nature|
|Forms, checkout + privacy|../patterns/forms-and-data-entry.md; ../patterns/errors-and-input-tolerance.md|../patterns/privacy-data-and-security.md; ../patterns/defaults-and-choice-architecture.md; ../patterns/friction-undo-and-confirmation.md|fields say why data needed; drop what no one can justify; no preselection on consent / money; explicit confirmation before purchase|
|Accessibility|cross-cutting accessibility step of design-a-screen-or-flow.md (accessibility as specs, not intentions); ../laws/fittss-law.md (size floors); ../laws/postels-law.md; ../methods/testing-touch-layouts.md|../patterns/inclusive-and-accessible-design.md; ../principles/inclusive.md; ../evidence/inclusion-and-exclusion-costs.md evidence|persona spectrum, accessibility floors, low-end devices; frames inclusion, not conformance manual|
|Errors, destructive actions + friction|../patterns/errors-and-input-tolerance.md; ../patterns/calls-to-action-and-touch-targets.md|../patterns/friction-undo-and-confirmation.md; ../patterns/safety-and-abuse-resistance.md; ../principles/resilient.md|confirmation graded by consequence; undo windows + speed bumps; recovery + failure states|
|Calls to action, emphasis + layout|../patterns/calls-to-action-and-touch-targets.md; ../patterns/layout-grouping-and-hierarchy.md|../patterns/defaults-and-choice-architecture.md (equal-weight No entry); ../patterns/transparency-and-honesty.md; [deceptive-pattern taxonomy](../ethics/deceptive-patterns.md)|what emphasis + placement must never serve: hidden No, bait and switch, disguised ads|
|Waiting + perceived speed|../patterns/feedback-loading-and-performance.md; ../methods/thresholds-and-formulas.md|../ethics/using-psychology-responsibly.md; ../evidence/convenience-and-friction.md evidence|deliberate delays + perceived-speed techniques; cases where speed alone = goal|
|Pricing, plans + monetization|../patterns/lists-options-and-choice.md|../patterns/monetization-and-growth.md; ../patterns/transparency-and-honesty.md; ../evidence/business-cost-of-deception.md evidence|true cost before click; decoys, anchors + tier steering|
|Search, ranking + recommendations|../patterns/search-and-results.md|../patterns/recommendations-and-personalization.md; ../patterns/transparency-and-honesty.md|algorithm-ranked results: steering controls + explaining what orders what people see|
|Complexity, settings + automation|../patterns/complexity-management.md|../patterns/defaults-and-choice-architecture.md; ../patterns/privacy-data-and-security.md|defaults system sets when absorbing decisions; personal settings over group + automated actions|
|First impressions + polish|../patterns/first-impressions-and-aesthetics.md|../patterns/transparency-and-honesty.md; ../patterns/inclusive-and-accessible-design.md|polish hiding what matters; accessibility floors visual style must not undercut|
|Conventions + redesigns|../patterns/departing-from-convention.md; ../methods/convention-or-new-pattern.md method|../methods/process-safeguards.md (process patterns keeping others honest); ../patterns/defaults-and-choice-architecture.md|how change gets offered: opt-in, symmetric exit, staged rollout w/ withdrawal condition|

## Related

- core-stance.md: laws as heuristics, people over metrics, conflict-settling ranking.
- design-a-screen-or-flow.md: runs both passes on new design.
- review-an-interface.md: runs both passes on something existing.
- ../laws/index.md: usability half; all 30 laws by theme, w/ core idea + design rule.
- [Principles index](../principles/index.md): humane half; seven principles side by side w/ neighbours to check.
- ../ethics/influence-vs-manipulation.md: general line-drawing test + lever-by-lever table, legitimate use vs crossing the line.
- [Deceptive-pattern taxonomy](../ethics/deceptive-patterns.md): pattern names used in tables above, each w/ its honest alternative.
- ../principles/surface-to-principle-map.md: principles each product surface touches first + pattern files to open.
