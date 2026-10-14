# Jakob's Law

## In one line
Any one product = smaller share of person's total usage → other products they already use set expectations of how it behaves. Use when: following vs breaking convention; weighing novel vs familiar pattern; planning redesign rollout; checking if Jakob's Law = right law to cite.
- Alias: Jakob's Law of Internet User Experience. Class: effect/principle.
- Theme: Expectations. Matters most for: platform conventions; opt-in redesign rollouts; deliberate, tested novelty.
- Core rules: follow conventions by default; novelty only for stated purpose + only after research + testing; opt-in redesign rollouts.

## Applies when / does not apply when
|Situation|Jakob's Law?|Note / do instead|
|---|---|---|
|product resembles one people already know|yes: inherits expectations of known one|match known one|
|tempted to copy known dark pattern/failure because common|no license: convention transfers learning, not approval|keep familiar structure, drop dark pattern/failure|
|task analysis, content design, site-specific information architecture|standards do not solve these|put effort there|
|data shows pattern failing|no freeze|iterate + give users temporary way back|
|broad audience|yes|explicit labels + proven patterns, even at some clutter/novelty cost|
|expert niche (e.g. other designers)|familiarity audience-specific|label-free, gesture-only designs suit|
|captive users (enterprise tools, dominant platforms pushing updates) or very high-frequency use|innovation safer|—|
|big brand imposing novelty|can work: perceived value outweighs learning cost|can still fail if plateau too far|
|information design (infographics, illustration, art direction)|creativity earns its place|only when it aids comprehension|
|audience from different cultures|past experience individual + cultural: white/black can signal purity or mourning, by culture|verify conventions w/ people they might exclude|

## Decision rules

### Default to convention
- Follow conventions by default; never trade usability for novelty.
- Each model learned = attention not spent on task → build on models people bring; none of that attention lost.
- Support most-practiced convention.
- Build new features from existing components + styles.
- Borrow known real-world affordances.
- Everyone-is-a-novice fix = transfer of learning: advanced features work identically everywhere, or live in browser/platform (e.g. Back, bookmarks) → people can use them w/o being taught.
- Conventions (e.g. blue underline = link, red = stop) help only when spacing, likeness + enclosure agree w/ them.
- Pattern changes in one place → decide if it should change everywhere, weighing impact vs effort.
- Unavailable controls → disable w/ explanation; do not hide (hidden controls break learned positions).

### Break a convention only if all three hold
1. New pattern much better once learned.
2. Users plausibly stay long enough to learn it.
3. Frequent exposure or scaffolding (contextual tips, progressive disclosure) can speed learning.
- Plus clear purpose of one of 3 kinds: exploration + surprise; disruption (new technology unseating incumbents); differentiation.
- Strict testing + research = footing any novel pattern needs.
- Change/extend known pattern only when it gives clearly shorter route to goal.

### Roll out a redesign
- Roll out as opt-in; users migrate when ready.
- After redesign, keep known version available for set period → redesign meets less friction.
- Give temporary way back when iterating on failing pattern.
- Measure redesign after users habituate, not in launch week.
- Read preference surveys carefully: familiarity-based liking can pass for usability.

### Compare familiar vs novel
1. Measure both across repeated trials, not one first use.
2. Plot time per repetition; find each design's saturation point (where more practice barely helps) + plateau time.
3. Rare task → pick quick-to-learn design. Daily task → pick design fastest at plateau.
- Familiar patterns start at plateau, novel ones start slow → compare designs by learning curves.
- Tutorial shown once = not learning; how often + how recently people practise sets fluency.

## Why it works

### Mechanism
- Resemblance triggers it: lookalike product inherits familiar ones' expectations w/o effort; if it also matches them, existing knowledge carries load.
- Confusing unfamiliar patterns raise cognitive load.
- Few people use any single site long enough to become expert → nearly all visitors first-timers, leaving if site not usable within seconds.
- Power law of learning (1980) = cognitive basis of conventions winning: task time falls w/ practice along power curve. Familiar pattern already at performance plateau; novel one at slow start of its learning curve.
- Remembered solutions to one goal race each other (e.g. clicking logo vs Home to go home); most-practiced fires first; if it fails, next tried → annoyance + harsher site judgment.
- Category-wide conventions keep attention on person's goal, not interface → payoff shows in goal metrics (e.g. sign-ups, conversion, sales).
- Once novel pattern broadly adopted → becomes new convention.
- Three-line menu icon becoming standard for main menu, but some apps use it for lists; each inconsistent use weakens convention for everyone.
- Only a few icons near-universal: magnifying glass for search, print, home.
- Redesign backlash partly from inertia (status quo bias + mere exposure effect), not only real regressions.

### Convergence forces (a 2000 essay argued four forces drive sites toward standard visual design, terminology, interaction flow + information architecture)
|Force|Why it pushes toward standards|
|---|---|
|people use many sites|each site judged by habits formed on others|
|small mobile screens|no room for idiosyncratic navigation|
|one service on several devices|must feel like one service|
|syndicated/outsourced features (search, carts, registration)|blend into host site only if simple + standard|

### Terms
|Term|Meaning|
|---|---|
|Mental-model discordance|clash when product departs from expectations set by people's existing models|
|Mere exposure effect|liking something only because familiar; summarized in 2004 review|
|Change aversion|short-term satisfaction drop after change|
|Internal consistency|consistency across product's own pages + components|
|External consistency|consistency w/ wider conventions outside product|
|Discount usability engineering|movement for improving interfaces via quick, low-cost fixes|
|Past experience (Gestalt)|grouping principle listed by Gestalt psychologists: things often seen together perceived together (e.g. cursive strokes read as familiar letters); weakest grouping principle, easily overridden by stimulus cues like closure + continuity|

### Origin
- Stated in 2000: people's experience across other sites, summed over time, shapes expectations of each new site. Cite Jakob's Law as dating to this 2000 statement.
- Status quo bias behind redesign inertia linked to 1991 work.
- Measurable form (learnability): by power law of learning (1980), task time falls w/ repetitions as straight line on log-log axes.
- Classic usability heuristics published 1990, revised 1994.

## Evidence
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Users' web experience elsewhere teaches what design patterns to expect|2000 practitioner principle from usability consulting|practitioner principle|follow conventions by default|
|4 forces drive sites to converge on standard visual design, terminology, interaction flow + information architecture|2000 essay|argued|—|
|Task time falls w/ practice along power curve|power law of practice (1980), roots in 1885 work|—|compare learning curves|
|Menu selection time over 8 practice blocks w/ same 6 items fit power curve|2010 lab study|lab|measure across repeated trials|
|Fact-recognition time fell across days of practice + saturated at about day 12|1985 lab study|lab; about|find saturation point|
|Value of external consistency|1989 edited volume on coordinating user interfaces for consistency|edited volume|keep external consistency|
|Real-world cases of justified novelty (exploration, disruption, differentiation)|no studies/statistics behind them|lesson only: break convention for clear purpose + test it|—|
|Brand names offered w/o any data, for product redesigns or serial position effect (e.g. Electronic Arts, Nike, Apple)|—|illustrations only|do not cite as evidence|

## Product cases
|Case|What happened|Strength|Lesson|
|---|---|---|---|
|Windows 8|users never reached learning plateau of its novel interface; vendor redesigned it|—|plateau too far → novelty fails|
|Snapchat, early 2018|redesign moved everyday features out of easy reach; users protested in large numbers; part of user base switched to Instagram|public reaction, no metrics|sudden redesigns cause mental-model discordance|
|Google|rolled out Gmail, YouTube + Calendar redesigns as opt-in|—|opt-in rollout|
|YouTube, 2017|after years of nearly constant look, its Material Design version stayed optional on desktop, w/ way back to earlier look, comment channel + time to try + get used to it|described outcome: discordance avoided|opt-in + way back + feedback channel + time|

## Misreadings and limits
- Wrong: hiding unavailable controls (Fitts's Law, Jakob's Law) → Right: disable w/ explanation; hidden controls break learned positions.
- Wrong: copying widespread deceptive or slow pattern + citing Jakob's Law → Right: keep familiar structure but not known dark pattern/failure.
- Wrong: novelty w/o purpose or testing → Right: default to convention + test any novel pattern.
- Wrong: judging novel pattern by first-use performance → Right: compare learning curves + plateaus across repetitions.
- Wrong: forcing abrupt redesign → Right: temporary opt-in + way to revert.
- Wrong: familiar design's preference-test win = proof of quality (Mental Model, Jakob's Law) → Right: mere exposure inflates liking → separate preference from performance.
- Wrong: all sites looking alike = user problem → Right: mostly producer's complaint, not users' problem.
- Wrong: Jakob's Law freezes design → Right: when data shows pattern failing, iterate + give users temporary way back.
- Limit: sudden forced redesigns → backlash.
- Limit: novelty costs users learning.
- Limit: familiarity's payoff to users outweighs monotony shared conventions can bring.
- Limit: past experience = weakest grouping principle; stimulus cues like closure + continuity easily override it.
- Limit: following standards does not solve task analysis, content design or site-specific information architecture.

## Check questions
[A] = answerable from artifact itself (screen, prototype, spec).
- [A] (Jakob's Law, Mental Model) Do standard patterns behave as elsewhere? Look for: carts, checkout + form controls reinvented w/o stated purpose; links opening new windows; Back jumping up hierarchy; overlays Back cannot close.
- [A] (Jakob's Law, discordance) Major redesigns get temporary opt-in + way back? Look for: sudden forced changes to daily-used features.
- [A] (Fitts's Law, Jakob's Law) Dangerous/unavailable controls disabled w/ reason, not hidden, + kept apart from positive actions? Look for: OK beside Delete; controls vanishing by state; soft keys changing meaning.
- Before shipping novel pattern: all 3 conditions hold, + stated purpose of one of 3 kinds?
- Before reading preference test: could familiarity explain liking?

## Symptoms → fixes
|Symptom|Likely cause (laws)|Fix|
|---|---|---|
|Redesign triggers backlash|Jakob's Law, Mental Model|temporary opt-in w/ preview; feedback channel; way back|
|Team wants novel pattern users find slow|↑|deviate only if much better once learned, users stay long enough to learn, + scaffolding can support learning; compare learning curves, not first use|

## Hypothetical examples
- Hypothetical: familiarity beats closure → home thermostat app shows two curved arrows chasing each other in ring; people read them as familiar sync symbol, not one broken circle.
- Hypothetical: novelty becoming convention → long-press gesture to duplicate entry, first seen in one calendar app, spreads across many scheduling tools until people try it everywhere; thereafter = convention, not novelty.
- Hypothetical: borrow known real-world affordances → car-sharing app draws unlock control as key fob w/ separate lock + unlock buttons → drivers know what to press w/o instruction.
- Hypothetical: shared conventions keep attention on goal → city parking-permit portal orders steps (address, vehicle, payment) like other permit sites residents used → applicants think about permit, not screens.
- Hypothetical: known patterns → pharmacy refill site puts basket, account + search where shoppers' other online stores put them → first-time visitors find each w/o hunting.
- Hypothetical: law as team policy → bank's design review rejects any new screen drawing custom control where existing component already serves.
- Hypothetical: novelty for differentiation → budgeting app shows spending as calendar heat view instead of usual transaction list, states purpose up front + tests it before launch.
- Hypothetical: novelty for disruption → utility app lets households photograph meter to submit reading, using image recognition instead of established typed-entry form.
- Hypothetical: novelty for exploration + surprise → travel site's city guide lets visitors drag sun slider to watch streets change from morning to night, inviting play over speed.

## Humane bound
- Bounded by Transparent: controls do what their label says.
- Bounded by Inclusive: convention = default to verify w/ people it might exclude.
- Convention transfers learning, not approval: no license to copy known dark pattern/failure.
- Turned against people: breaking convention to trick people = bait and switch (e.g. close button starting upgrade).
- Turned against people, reverse case: novelty can hide intent; format people never met reads as neutral → persuasion inside it arrives unexamined.
- Further reading: deceptive-pattern taxonomy; transparency patterns (controls do exactly what their label says); six advantages systems hold over human persuaders; inclusive + accessible design (convention = default to check).

## Related
- ../principles/transparent.md: humane principle bounding it; controls do what label says.
- ../principles/inclusive.md: humane principle bounding it; verify conventions w/ people they might exclude.
- ../ethics/deceptive-patterns.md: named deceptive patterns + honest alternatives to keep out of familiar designs; convention transfers learning, not approval.
- ../patterns/transparency-and-honesty.md: controls do exactly what label says.
- ../ethics/persuasion-advantages-of-systems.md: six advantages systems hold over human persuaders.
- ../patterns/inclusive-and-accessible-design.md: treat convention as default to check.
- mental-model.md: conventions build on people's existing mental models; departure → mental-model discordance; shares standard-patterns check + redesign-backlash and novel-pattern fixes.
- cognitive-load.md: conventions cut learning load.
- occams-razor.md: leaving new pattern uninvented keeps complexity out at lowest cost.
- gestalt-principles-overview.md: Gestalt background; stimulus cues (closure, continuity) overriding past experience; how grouping cues combine + compete.
- ../checklists/usability-heuristics-map.md: "Match between system and real world" → Mental Model + Jakob's Law; "User control and freedom" → Jakob's Law (opt-in redesigns, way back) + Paradox of the Active User (safe experimentation); "Consistency and standards" → Jakob's Law + Similarity; classic heuristics 1990, revised 1994.
- ../methods/convention-or-new-pattern.md: steps for judging when new pattern worth its learning cost + for rolling out redesign.
- ../guides/laws-and-principles-crosswalk.md: maps humane principle bounding it.
- ../patterns/navigation-and-menus.md: applies it.
- ../patterns/forms-and-data-entry.md: applies it.
- ../patterns/onboarding-and-first-use.md: applies it.
- ../patterns/departing-from-convention.md: applies it.
- ../patterns/ai-and-automated-features.md: applies it.
