# Tesler's Law

## In one line
Every system has fixed complexity residue: it can change owner, never vanish. → Let system carry it: defaults, suggestions, data reuse, automation, progressive disclosure.

- Alias: Law of Conservation of Complexity. Theme: Complexity. Classed as effect / principle.
- Design areas most affected: complexity carrier (system / user), smart defaults + automation, progressive disclosure.
- Evidence status: mid-1980s industry engineering principle, not experiment.

## Applies when / does not apply when

|Situation|Tesler's Law?|Cite instead / also|
|---|---|---|
|Choosing 1 of 3 holders for part of process nobody can remove: code + hardware (system), support + operations staff (organization), head + hands (user)|Yes|../methods/who-absorbs-complexity.md|
|How far to simplify / automate|Yes, w/ paired check|hicks-law.md (too much)|
|Removing steps via stored-data reuse (forms take too long)|Yes, cite first|parkinsons-law.md only as expected-duration lens|
|Back loses filters, query or scroll position|Yes, system carries state|working-memory.md, user-control heuristic|
|Settings page w/ dozens of toggles hard to scan|Yes, for progressive disclosure|cognitive-load.md, chunking.md, common-region.md, pareto-principle.md to verify usage w/ analytics; not choice-overload.md|
|Many independent settings (e.g. sixty separate toggles)|Relocate complexity per Tesler's Law|Not Choice Overload (needs one choice among close substitutes): scanning + finding load → Cognitive Load, selective-attention.md, Chunking, progressive disclosure|
|Complex applications (five traits below)|Yes, but consumer simplification rules (fewer options, linear wizards) do not apply|Staged disclosure, nonlinear workflows|
|Simplicity for its own sake|No: simplicity not goal in itself|occams-razor.md, stopped by floor of simplification|

Five traits of complex applications (2020 practitioner guideline set) = when consumer simplification rules stop applying:
1. Users = highly trained domain specialists.
2. Large data sets + advanced analysis.
3. Open-ended goals w/ unknown / variable subtasks.
4. Handoffs among roles + tools.
5. High-stakes tasks: failure can cost revenue or lives.

## Decision rules

### 1. Find the core, then assign the carrier
- Once irreducible core found → decide explicitly: system or user carries it; default to system.
- Before assigning any piece to user → list irreducible core + check if system could hold each piece (defaults, reuse, automation).
- If complexity unavoidable → absorb it in design + engineering; target = smallest possible residue for users.
- Unless company holds sustainable monopoly → value customer time over engineer time.
- Accept extra build effort saving many users repeated effort.
- Complexity moved to engineers has real cost → moving it = cost-benefit case, not dogma.
- Cut functionality only where no significant penalty follows.
- Design for real people (often act irrationally); perfectly rational ideal user = wrong target.

Ways to relocate complexity to system:
|Lever|Form|
|---|---|
|Data|Entered-data reuse; prefilling known data; stored payment methods|
|Prediction|Suggestions from history|
|Layering|Progressive disclosure: hover menus, toggles, accordions, dropdowns|
|Delegation|Automation|
|Intent|Less up-front expertise needed when people describe end result in natural language, not step through command-based GUI actions (intent-based interaction); candidate where product carries many features|

### 2. Estimate the cost before deciding
1. Pick time window (week, year, customer lifetime) + currency (time, money, utility).
2. Estimate user cost: frequency of complexity × active users × cost per encounter = weekly frequency × weekly active users × cost per encounter (2017 practitioner formula).
3. Compare multiplied user cost w/ one-off build cost (often ≥ one week of team time) → user cost almost always wins.
- Measurable form (industry framing): 1 lost minute per user per day × 1,000,000 users vs single added engineer-week.
- Quote formula, not its accompanying worked example (3 encounters/week × 1,000,000 users × 0.5 minutes): its totals mix seconds + minutes.

### 3. Decide how far to simplify
- Simplicity = means (speed, usability, saved time), not goal in itself.
- Test both directions: 'how simple can it be?' + 'how complex must it be?'.
- Check every simplification against both hicks-law.md + Tesler's Law.
- If interface turns into abstract marks → simplifying went past limit, should already have stopped; stop short of abstraction.
- Floor of simplification: minimal interface failing real edge cases = incomplete, not simpler.
- If next cut would drop genuine user case → move case's complexity into system, not delete it.
- Removing tool can shift complexity into user's memory, not eliminate it.
- Keep some meaningful participation for user vs removing all effort. Some effort valuable to person: before automating step away, ask whether it gave them something.
- Complex applications (five traits) → favor staged disclosure + nonlinear workflows over consumer simplification rules.

Automation vs control: position product on spectrum from full automation to full manual control by:
- device type;
- activity frequency + complexity;
- user expertise;
- market positioning (power tool / mass market);
- emotional tone (powerful / elegant).

|Delegate to machine|Leave to user|
|---|---|
|Calculation, multitasking, pattern detection, querying large data|Direct-manipulation decisions, personal-preference decisions|

### 4. Layer + stage what remains
- Move complexity into progressively disclosed layers.
- Reveal features as each step mastered.
- If first-time users dive straight in, by any route → in-context aids (e.g. tooltips) at each point of need, on every route.
- Stage features for beginners + test long-term effects.

### 5. Design automation's failure path
- Always design it: fast support, clear diagnosis, instructions.
- Communicate system state; hidden automation w/o state feedback quickly confuses.
- Limit automation run time before handing control back; keep users' skills current.
- Wherever abstraction leaks → document workaround.

### 6. Watch the wording
- Wording = another main place complexity leaks back to users.

## Why it works

Mechanism:
- Complexity conserved: whatever system skips → user effort, multiplied across whole user base. Absorbing it once on build side → minimal total cost.
- Core argument: given choice, one engineer's extra week = usually lesser harm vs extra minute billed to each of millions of users (sparing engineer = 1 lost minute per user per day × 1,000,000 users).
- Every function needs control: visible (e.g. physical button) or absorbed by automation (e.g. self-regulating thermostat).
- Adding control tells user 'you handle this'; removing it = system decides; works only w/ smart defaults.
- Handing control to someone sets their workload: eases giver's job, burdens receiver.
- Perceived complexity lives in user's conceptual model (2010 book): felt simplicity depends on user's model of it. Better conceptual model can make something feel simpler w/o changing it.
- Simpler use always adds complexity to mechanism; simple mechanism can yield very complex surface.
- Simplicity vs control = spectrum from full automation to full manual control.
- Simple look does not mean easy use: stripping controls can force longer action sequences for same functions. Surface simplicity wins first impressions; operational simplicity matters more.
- Experts see rich toolset as many individually simple tools.
- Over-simplification backfires: users sense complexity must go somewhere → suspicious or feel robbed of control. Beyond some point, simplification → diminishing, then negative returns.
- Automation judged by how it breaks: breakdown possibly most memorable interaction w/ automated product; bad one can erase years of good service.
- Hidden complexity returns at abstraction's edges (leaky abstractions).
- Design paradigm argument, both halves: AI intent-based interaction = person states wanted outcome in natural language → system's complexity stays hidden + anyone knowing outcome gets power-user capability; vs GUI command paradigm of recent decades: system feedback answers each user action.
- Once interface standards sit in libraries applications share → consistency pays off for developers + users.

Terms:
|Term|Meaning|
|---|---|
|Waterbed theory|Push complexity down in one spot → it bulges elsewhere; design only picks where, among its 3 possible places (system, organization, user), irreducible core lives|
|Interaction-design language|Sets out how interactive system behaves + gets built: best practices, standards, principles|
|Law against miserliness|Do not reduce entities to point of inadequacy; marks where simplification stops|
|Principle of sufficient reason (as check on parsimony)|Avoid simplifying until explanation no longer covers facts; marks where simplification stops|
|Automation complacency|Drivers of self-driving cars + pilots of highly automated aircraft may panic or forget procedures when suddenly having to take over|
|Leaky abstraction|Hidden complexity returning at abstraction's edges|

Origin, dated:
|When|What|
|---|---|
|mid-1980s|Interaction-design language formed in industry research labs; desktop publishing + desktop computer both depended on it; in it, application + interaction w/ it carry equal weight|
|mid-1980s|Law developed through 1980s industry work: popularly placed in earlier research-lab period, but named argument grew out of later work on shared application framework|
|Later, in industry (no precise year)|Formulated so customers face less complexity, while pitching standardization to outside developers + company's own management; refined while building intermediate 'generic application' on MacApp (Apple's object-oriented framework for Mac applications) developers could adapt|
|1984|Training-wheels experiments (see Evidence)|
|1990, 1994|Classic usability heuristics (revised 1994); Flexibility and efficiency of use links to Pareto Principle, Tesler's Law + Parkinson's Law|
|2006|Best-known account of law: interview in interaction-design book|
|2010|Book placing perceived complexity in user's conceptual model|
|2017|Practitioner complexity-cost formula|
|2020|Practitioner guideline set w/ five traits of complex applications|

- Dating: say it developed through 1980s industry work; check dates before quoting precise year.

## Evidence

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Complexity conserved; system should carry it|Mid-1980s industry engineering principle|Not experiment|Cite as principle|
|Engineer-week vs users-minute reasoning|Engineering cost argument|Not study|Use as cost framing|
|Simpler app → users move on to tougher tasks; stated reason: people resist losing complexity|Practitioner counterpoint|Practitioner argument|Do not promise lower total effort|
|Word processor showing all menu choices but disabling advanced + error-prone ones in early learning; choosing one → message, no state change|1984 controlled 'training wheels' experiments|One application (word processing), one interface style (menus)|Stage features for beginners|
|vs full commercial system: faster start, better work, less time lost on errors (blocked + unblocked alike); advantage grew over session; higher later concepts-test scores|Same 1984 experiments|Same scope limit|Test long-term effects of staging|
|One team ranked 'use simple language' first design principle + credited most engagement gains to rewritten copy, not new features|Insurance-software team|One company's reflection, not study|Treat wording as complexity lever|
|Counting boards (Roman tabula, Japanese soroban) easy to use but not portable; Hindu-Arabic positional notation portable w/ no moving parts but moved complexity into memorized number facts + symbol manipulation every schoolchild must learn|Book on arithmetic|Historical illustration|Removing tool can move complexity into memory|

Complexity moved to builders, one illustration per lever:
|Illustration|Where complexity went|Status|
|---|---|---|
|Slack progressive onboarding: message field = only feature shown until messaging learned; newcomers practice w/ bot where mistakes cost nothing|Staged learning|Qualitative case|
|Hypothetical: pharmacy refill form fills patient's own details + suggests usual collection branch from past orders|Data entry → system|Hypothetical|
|Hypothetical: home-insurance claim form offers to finish damage description as person types + proposes short ready answers to adjuster's follow-ups|Writing effort → system|Hypothetical|
|Hypothetical: passport-renewal form carries over mailing address from previous application; applicant only confirms|Address entry → system|Hypothetical|
|Hypothetical: utility-bill portal keeps household's bank account on file → paying = pick account + confirm|Payment entry → system|Hypothetical|
|Hypothetical: hospital supply room's sensors record what staff take → nobody scans items at door; ward charged automatically|Checkout → system|Hypothetical|
|Hypothetical: school attendance dashboard answers typed plain-language questions; staff need not build filters|Query building → system|Hypothetical|
|Hypothetical: university course catalogue site lists only faculties in top bar; pointing at one opens its departments|Progressive disclosure|Hypothetical|
|Hypothetical: home heat-pump controller keeps only dial + one button on casing; schedules, modes + holiday settings in menus on its display|On-screen layers|Hypothetical|
|Hypothetical: team lead sets up shared timesheet: new temps see only columns they fill in, every other column hidden → people around user, not maker, hid columns|Hidden by people around user|Hypothetical|

## Misreadings and limits
- Wrong: simplify until controls become abstract (Hick's Law, Tesler's Law). → Right: keep meaning; complexity must live somewhere (Tesler's Law); clarity beats minimalism (cognitive-load.md).
- Wrong: cite Choice Overload for many independent settings. → Right: Choice Overload needs one choice among close substitutes; sixty separate toggles = scanning + finding load (Cognitive Load, Selective Attention, Chunking, progressive disclosure); per Tesler's Law, relocate complexity.
- Wrong: design for rational user (Tesler's Law, paradox-of-the-active-user.md). → Right: design for real, irrational behavior.
- Wrong: equate 'looks simple' w/ 'easy to use' by removing controls. → Right: fewer visible controls can mean longer hidden sequences + memorized gestures; judge operational simplicity + keep capability experts need.
- Wrong: remove all effort from high-stakes actions. → Right: instant, invisible completion can feel unsafe or broken; keep meaningful participation + visible work.
- Wrong: call burden irreducible so users keep carrying it. → Right: list irreducible core first; check if system could hold each piece (defaults, reuse, automation) before assigning it to user.
- Wrong: ship automation w/o failure path. → Right: design breakdown, diagnosis + handover; limit uninterrupted automation so users' skills stay current.
- Wrong: expect simplification to reduce users' total burden. → Right: users may take on harder tasks instead; simplification may raise ambitions, not lower total effort.
- Wrong: under lean shipping, read 'simple' as 'minimal'. → Right: simple is not minimal; this misreading yields thin, low-value features until later iteration.
- Wrong: treat no-visible-interface design as simplest. → Right: practitioner warning against it: smartwatches + gesture-heavy mobile systems force people to memorize hidden gestures.

Limits:
- Complexity never eliminated, only reassigned; automation moves it to builders.
- Removing genuinely needed functions → harder job.
- Instant high-stakes operations (e.g. money transfers) can feel unsafe or broken.
- Beyond some point, simplification → diminishing, then negative returns.

## Check questions
Tag [A] = answerable from artifact itself (see ../checklists/usability-review.md).

|Check|Look for|Law / principle|Tag|
|---|---|---|---|
|System, not user, carries irreducible complexity?|Users entering data system already knows; no defaults / suggestions|Tesler's Law|[A]|
|Simplification stops short of abstraction?|Controls reduced until their meaning lost|Tesler's Law, Hick's Law|[A]|
|Each automated feature has designed failure + handover path?|No state feedback; no diagnosis / support route when automation breaks; sudden unprepared takeover|Tesler's Law|[A]|

## Symptoms → fixes
General: where complexity stays in interface → frustration + confusion.

|Symptom|Likely cause|Fix|
|---|---|---|
|Forms take too long|Tesler's Law (system carries stored data); Parkinson's Law (expected-duration lens)|Autofill, data reuse, sensible editable defaults|
|Automated feature fails + users lost|Tesler's Law|Communicate system state; failure + handover path w/ diagnosis + support|
|Settings page w/ dozens of toggles hard to scan|Cognitive Load, Chunking, Common Region; Tesler's Law for progressive disclosure; Pareto Principle to verify usage w/ analytics; not Choice Overload|Task-based labeled groups; search over names, synonyms + descriptions; advanced settings behind disclosure|
|Filters, query or scroll position lost on Back|Working Memory; Tesler's Law (system carries state); user-control heuristic|Keep state in URL; restore scroll position + filters on return|

## Hypothetical examples
- Hypothetical: banking app shows savings 'envelopes' per goal while money sits in one account ledger → envelope model makes budgeting feel simpler; mechanism unchanged.
- Hypothetical: full automation = building's smoke vents opening on their own; full manual = sailing dinghy steered by tiller + sheets.
- Hypothetical: budget airline: passengers print boarding passes + tag own bags for lower fare (self-service shifts work to customer).
- Hypothetical: travel agent making traveller pick every connection, seat + transfer time eases agent's job + burdens traveller.
- Hypothetical: medication dispenser releases right dose on schedule: real goal = correct dose, not act of counting pills.
- Hypothetical: transit card tapped at gate makes paying feel like no ticket purchase at all, while fares still collected.
- Hypothetical: garden irrigation controller adapts watering to household's past schedule + weather.
- Hypothetical: patient notes appear on every exam-room tablet w/o staff exporting + importing files.
- Hypothetical: one car installs map updates overnight in garage; another makes owners download maps at home, copy to USB stick, plug it in + restart system.
- Hypothetical: museum ticket kiosk lets visitors continue w/ existing wallet account, not registration form w/ username-taken errors + password rules.
- Hypothetical: print shop's 'Reprint last job' button.
- Hypothetical (counter-example): coffee machine w/ only power + brew buttons must choose grind, strength + temperature itself; w/ weak defaults → bitter or weak coffee.
- Hypothetical: washing machine offers many programs while everyday need may come down to single normal cycle.
- Hypothetical: TV remote w/ only arrow keys + OK forces letter-by-letter search entry: fewer buttons → longer sequences.
- Hypothetical: dental hygienist's tray of instruments, or spreadsheet's many single-purpose functions, seen by experts as many simple tools.
- Hypothetical: savings app automates transfers but has person name + confirm each goal → keeps meaningful part of effort.
- Hypothetical: clinic manager reviewing no-show reports by hand learns appointment times patients struggle to keep; auto-archiving report would remove this insight.
- Hypothetical: photo-backup service auto-detects camera folders but silently skips messaging-app images saved in nonstandard folder unless user adds folder by hand → document workaround.

## Humane bound
Tesler's Law turned against people:
- Calling burden irreducible so users keep carrying it.
- Control removed so system decides silently: hidden automation w/o system-state feedback, no failure path, decisions no one can question or overturn. Agency diminished when systems decide silently.
- Defaults system carries, chosen for system's benefit.

|Principle|Bound on Tesler's Law|Read|
|---|---|---|
|../principles/empowering.md|Human in loop: can review, correct, approve + appeal|../patterns/ai-and-automated-features.md (hand-over, uncertainty, human review)|
|../principles/intentional.md|Defaults chosen for people's well-being|../patterns/defaults-and-choice-architecture.md (opt-in, equal-weight decline)|
|—|Further reading on bound|../patterns/complexity-management.md|

## Related
- hicks-law.md: paired check; Hick's Law warns against too much (options + decoration for design's sake), Tesler's Law against too little (controls simplified into abstraction).
- occams-razor.md: dropping non-functional elements, stopped by floor of simplification.
- postels-law.md: accepting + normalizing varied input.
- parkinsons-law.md: shares forms-take-too-long fix (expected-duration lens).
- paradox-of-the-active-user.md: design for real, irrational behavior.
- ../checklists/usability-heuristics-map.md: Flexibility and efficiency of use links to Pareto Principle, Tesler's Law + Parkinson's Law.
- ../checklists/usability-review.md: meaning of [A] tag.
- ../methods/who-absorbs-complexity.md: allocating irreducible complexity between system + user.
- ../guides/laws-and-principles-crosswalk.md: humane principle bounding law.
- ../patterns/navigation-and-menus.md, ../patterns/forms-and-data-entry.md, ../patterns/onboarding-and-first-use.md, ../patterns/errors-and-input-tolerance.md: apply law.
- ../patterns/ai-and-automated-features.md: humane bounds on automation; applies law.
- ../patterns/defaults-and-choice-architecture.md: humane bounds on system-carried defaults.
- ../patterns/complexity-management.md: further reading on humane bound; applies law.
- ../lookup/timeline.md: lists 2006 interaction-design book holding best-known account of law.
- ../principles/empowering.md, ../principles/intentional.md: principles bounding it.
