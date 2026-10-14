# Paradox of the Active User

## In one line
People use software at once, never open manuals. Rule: contextual help + progressive onboarding, not front-loaded tours. Matters most when choosing contextual tooltips vs tours, progressive onboarding + revisitable getting-started checklists.

- Class: effect or principle; no aliases. Theme: Complexity, within group Complexity and robustness.

## Applies when / does not apply when
|Applies when|Does not apply / limit|
|---|---|
|novices skip instructions, jump straight in|safety- or mission-critical domains (errors cost lives or revenue): pure exploration too risky; formal training still needed|
|experienced users plateau, keep known methods, rarely seek better|—|
|today manuals rare, yet both behaviors persist|—|
|any product: no course covers every use → some learning by doing unavoidable; support it in interface|—|

## Decision rules
Plan for skipping
- Skipping up-front learning = stable behavior; accommodate skippers, do not expect change.
- Documentation unread beforehand because task at hand drives users → plan for it.
- Replace front-loaded tours w/ contextual tooltips, progressive onboarding + revisitable get-started checklists.

Help in place
- Every route active newcomer might take needs help → spread tooltips + similar aids across whole product, each matched to its task + moment.
- Avoid guidance along one prescribed path: misses users on other paths.
- Never let front-loaded tours (overlay after overlay, each pointing at UI element) stand between person + product.

Progressive onboarding
- Start w/ one core action.
- Offer risk-free practice space; hide advanced features until each step mastered, then reveal them.
- Offer checklist or "get started" template: own pace, revisitable; real use teaches core features.

Learning by doing
- Safe experimentation: no lost work, no irreversible damage.
- Short feedback loops; never ask for long action sequences w/o showing results.
- Teach expert methods in context when useful, e.g. hover tip revealing faster accelerator.
- Design for discovering efficient methods over whole life of use, not only onboarding; paradox hits experienced users too → surface faster methods in context.

Against related biases
- Present bias → deliver learning when it pays off immediately (just-in-time help); offer reminders + self-set commitment devices.
- Planning fallacy → planning tools prompt for base rates from past tasks.
- Instant rewards can exploit present bias in engagement loops → design so users' longer-term goals win.

Choosing remedies
- Mix complementary remedies + test w/ real users; avoid relying on any single remedy.
- Organize help by user goals, w/ built-in error checkpoints.
- Stage features for beginners + test long-term effects.

## Why it works
1. Paradox: users skip up-front learning though, long-run, it would save them time.
2. Late payoff: learning pays off late, loses to pull of task at hand → people learn by doing, tolerate errors.
3. Incremental learning: each step rests on earlier ones → staged reveals work.
4. Two paradoxes (so named 1987):
   - (1) Production paradox: users care most about throughput → purpose + concrete rewards, little reason to stop and learn → keep known procedures even when better ones exist → long skill plateau.
   - (2) Assimilation paradox: new system read through prior knowledge; users may never imagine features their familiar metaphor does not suggest.
   - Production bias + assimilation bias reinforce each other.
   - Original 1987 account: both = basic properties of adult learning, not defects design can remove → every solution has trade-offs.
5. Plateau cost: skipped setup + learning → long mediocre-skill plateau → over years of daily use, large productivity gap. Same plateau explains why heavy personalization + setup-dependent features often go unused.
6. Newcomers = experts in own work, not blank slates; build quick theories from fragments + act on them → early confusions can spiral before improving.
7. Product tours = case of people made to adapt to technology.

Related terms
|Term|Meaning|Link to paradox|
|---|---|---|
|Satisficing|accepting first adequate option|production-paradox habit: keep slow but good-enough method, not search for better → why active users plateau at mediocre skill|
|Present bias|immediate rewards outweigh later ones|deliver learning when it pays off immediately (just-in-time help)|
|Hyperbolic discounting|preferences reverse as rewards near|—|
|Projection bias|assuming future self will want what one wants now|—|
|Planning fallacy|inside-view estimates ignore how long similar past tasks took|planning tools should prompt for base rates|
|Minimalist instruction|task-oriented, minimal documentation|collected in 1998 book|

## Origins
|When|What appeared or was shown|
|---|---|
|early 1980s|several user studies: learning + routine use of word processors + text editors|
|1987|Paradox of the Active User published as chapter, pp. 80-111, of edited HCI collection on mental processes in computer use (concept's broader cognition-focused setting); evidence base = user studies of people learning computers|
|1998|report: many later studies confirmed pattern; minimalist instruction collected in book|

## Evidence
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Newcomers went straight to work on machines, bundled documentation unopened; errors + stuck points accepted as price of starting at once|original user studies (early 1980s, word processors + text editors; published 1987)|observational; 1998 report: many later studies confirmed it|treat skipping as stable; help in context|
|Most people take in little or nothing of front-loaded tour|—|"most"|no front-loaded tours|
|Word processor seen as "super typewriter" → easy start; when metaphor broke, users misled: surprised space bar, backspace + return keys changed document formatting|case in original 1987 account|case; (2) assimilation paradox|users may never imagine features familiar metaphor does not suggest|
|Office staff learning word processor knew office tasks better than its designers did|original-study case|case|treat newcomers as experts in own work|
|Learner worked out wastebasket function by deleting applications she then could not restore|observed case, 1985|case; cost of learning by doing|safe experimentation: no irreversible damage|
|After one hour of look-but-don't-touch training, learner said he could have typed thousands of words meanwhile|observed case|case; cost of non-active training|learn by doing, not passive training|
|Training wheels: word processor showed all menu choices but disabled advanced + error-prone ones in early learning; choosing one → message, no state change|1984 controlled experiment|one word-processor study; one application, one interface style (menus)|stage features for beginners|
|vs full commercial system, training-wheels learners started faster, produced better work, lost less time on errors (blocked + unblocked counted); advantage grew over session; higher later concepts-test scores|1984 training-wheels experiment|↑|stage features for beginners; test long-term effects|
|Some protective interfaces hurt later learning → blocking's presentation matters|early results, 1985|"suggested", "some"|test long-term effects of protection|
|Guided Exploration: help as task cards, one per real office goal: deliberately incomplete hints, error-spotting checkpoints, recovery steps + general what-went-wrong card|1985 experimental comparison w/ novices|—|organize help by user goals w/ error checkpoints|
|vs commercial self-study manual, Guided Exploration novices took less time + did better on transfer test; achievement per unit time almost 3 times more efficient|1985 Guided Exploration comparison w/ novices|"almost"|↑|
|Many text-editor users never adopted available public macros, even basic ones, though macro use went w/ faster editing; secretarial + administrative staff macro use ~zero|1984 field survey w/ usage logging, daily work|"many", "about"|surface faster methods in context|
|Larger function-key repertoires went w/ faster work, but size tracked experience w/ other screen editors, not time on this one|1984 text-editor field survey|field survey w/ usage logging|experienced users plateau; design for discovery over whole life of use|
|Slack's progressive onboarding: message field only feature shown until messaging learned; newcomers practice w/ bot (Slackbot), mistakes cost nothing|product case|qualitative case|reveal features as each step mastered|
|Notion's getting-started template: beginner checklist, revisitable any time; real use teaches core features; keeps product's limitless possibilities from swamping newcomers|product case|↑|offer risk-free practice space|

## Remedies and their costs
Every remedy costs something (original 1987 account).

|Remedy|Cost / caveat|
|---|---|
|Make learning intrinsically rewarding (game-like framing, points)|can make serious tool look toy-like|
|Make learning safe (undo, staged "training wheels" interfaces, error blocking)|can make it passive; early results (1985) suggested some protective interfaces hurt later learning|
|Organize help by goals|fails when users misjudge goal; may leave isolated knowledge pockets, hard to combine|
|Match familiar metaphor exactly|can leave system trivial, learning shallow|
|Progressive disclosure|in 1987 no empirical test of it known|

→ Mix complementary remedies + test w/ real users.

## Misreadings and limits
- Wrong: front-load tours + manuals. → Right: contextual, always-available guidance; up-front documentation + tours fail.
- Wrong: design for rational user (misapplication shared w/ Tesler's Law). → Right: design for real, irrational behavior; perfectly rational ideal user = wrong design target.
- Wrong: 1984 training-wheels study hid features or added tooltip support. → Right: every menu choice stayed visible; advanced error-prone ones disabled w/ message + changed nothing; learners lost less time on errors.
- Limit: training-wheels evidence = one word-processor study (controlled experiments, one application, one interface style: menus); early results (1985) suggested some protective interfaces hurt later learning.
- Limit: in safety-critical or mission-critical domains formal training still needed.

## Check questions
- [A] (Paradox of the Active User): can users start immediately, help available along any path? Look for mandatory front-loaded tours + help existing only in manual or one fixed flow. In usability review checklist: under theme Systems and behavior.
- Can people experiment w/o losing work or causing irreversible damage?
- Results shown after each action, not after long sequence?
- Faster methods surfaced in context to experienced users?

## Symptoms → fixes
|Symptom|Likely cause|Fix|
|---|---|---|
|New users ignore tour|Paradox of the Active User: task pull beats up-front learning|contextual tooltips, progressive reveal + revisitable get-started checklist|
|Experienced users stay on slow methods; macros, shortcuts + accelerators unused|production paradox → skill plateau; satisficing|teach faster method in context when useful|
|Personalization or setup-dependent features unused|skipped setup + learning → long plateau of mediocre skill|teach feature in context when useful, at moment it pays off (just-in-time help)|
|Early confusion spirals|quick theories built from fragments|short feedback loops; safe experimentation|

## Hypothetical examples
- Hypothetical: banking app's home-loan calculator recalculates monthly payment as each slider moves → wrong entry shows at once, not after full form.
- Hypothetical: expense-report tool sees employee typing same merchant + category line after line → tip beside field offers one-step copy of previous line.
- Hypothetical: public-transit ticket app shows one-line tip beside fare-zone selector first time rider opens it, not tour at launch.

## Humane bound
- Bounded by ../principles/intentional.md principle: weigh quick win vs later effects; favor habits people would endorse. Also bounded by ../principles/transparent.md + ../principles/respectful.md.
- Instant rewards can exploit present bias in engagement loops → design so users' longer-term goals win (../ethics/using-psychology-responsibly.md).

First-use abuse to avoid:
- forced sign-up before product shows value;
- work held hostage = coercive use of effort people invested;
- confirmshaming when people skip or decline;
- pre-checked marketing consent;
- asking for notification permission at first launch.

Further reading: ../ethics/using-psychology-responsibly.md; ../patterns/onboarding-and-first-use.md (its entry on keeping onboarding accessible + fair); [Habit, progress and gamification mechanics](../patterns/habits-streaks-and-gamification.md).

## Related
- teslers-law.md: same theme (Complexity); shares rational-user misapplication.
- hicks-law.md: related via progressive onboarding.
- cognitive-load.md: cited together on tour screens offering no choice (attention spent before product gives value).
- mental-model.md: related via assimilation (new systems read through prior knowledge).
- [Usability heuristics mapped to laws](../checklists/usability-heuristics-map.md): "User control and freedom" relates to Jakob's Law (opt-in redesigns, way back) + this law (safe experimentation); "Help and documentation" relates to this law; classic heuristics date from 1990, revised 1994.
- [Usability review checklist](../checklists/usability-review.md): holds this law's question under Systems and behavior.
- ../methods/teaching-inside-the-task.md: steps for building first use around learning by doing.
- ../ethics/using-psychology-responsibly.md: guardrails where instant rewards could exploit present bias in engagement loops.
- ../guides/laws-and-principles-crosswalk.md: humane principle bounding this law.
- ../patterns/onboarding-and-first-use.md: patterns applying this law.
- [Errors, input tolerance and edge cases](../patterns/errors-and-input-tolerance.md): patterns applying this law.
- ../patterns/complexity-management.md: patterns applying this law.
- [AI, assistants and automated features](../patterns/ai-and-automated-features.md): patterns applying this law.
- [Habit, progress and gamification mechanics](../patterns/habits-streaks-and-gamification.md): humane bound on reward mechanics.
