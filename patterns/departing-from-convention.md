# Departing from convention

## Use when
- Covers: when to follow established conventions, when + how to deviate (differentiation, disruption, exploration), learning-curve choice, redesign rollout.
- Open when designing/reviewing: new pattern, unusual layout / interaction, big change to familiar product.
- Laws in play: Jakob's Law, Mental Model, Cognitive Load, Aesthetic-Usability Effect, Choice Overload.

## Decision flow
1. Users already met pattern for this elsewhere? Yes → follow by default.
2. Stated purpose for departing (differentiation, disruption, exploration / surprise)? No → keep convention.
3. Audience behaviour, preference + need known, backed by research + strict tests? No → research first.
4. Departing → functional core stays familiar; novelty at periphery + carries function.
5. Pick learning curve by how often people do task.
6. Substantial change to familiar product → opt-in rollout, old version one switch away.

### Should this follow the convention? (default to convention)
- When: wherever patterns exist users already met elsewhere.
- Do: follow established patterns by default. Research users' aims + models they already bring (personas, empathy + journey maps, user interviews) → designer's model + theirs converge.
- Avoid: novelty for its own sake. Never assume designer's model matches users'.
- Why: Jakob's Law, Mental Model, Cognitive Load.
  - Established patterns → people's existing mental models carry over to new product.
  - Payoff visible in signups, conversion + sales: known interface goes unnoticed, attention stays on goal → completion more likely.
  - Confusion from unfamiliar patterns raises cognitive load.
  - Origin: 1943 account of thinking = explaining + anticipating events by consulting miniature inner copy of world.
- Hypothetical: hotel-booking site keeps date picker, guest count + reserve button where travellers met them on every other booking site.

### Is there a purpose that justifies novelty?
- When: considering any departure from convention.
- Do: novelty only for stated purpose. Three purposes:

|Purpose|Looks like|Illustration|
|---|---|---|
|Differentiation|deep personalization; alternative layouts; product's own interactions + features; branding|Hypothetical: fitness-tracking app swaps usual tile dashboard for one running diary of day w/ member-chosen measures; carries own coaching feature + visual identity|
|Disruption|when new technology changes interaction model|Hypothetical: library catalogue: readers describe half-remembered book in plain sentences → language technology returns one shortlist; no separate title, author + subject fields|
|Exploration / surprise|unusual page structure, motion + interaction; e.g. narrative paced by reader's own swipes / scrolls|Hypothetical below|

- Avoid: novelty w/o one of these purposes (novelty for its own sake).
- Why exploration novelty works: departures from usual get noticed + remembered; tied to scrolling → content pulls people onward + experience turns immersive.
- Hypothetical (exploration): water utility's explainer follows one drop reservoir → tap; each scroll step advances drop one stage on animated map. Aim = open-ended browsing + discovery → scroll-led format fits. Plain article page would also work; team picks scroll version expecting better interest + recall.
- Caveat (differentiation): browser praised for reorganizing familiar browsing later moved effort to successor product + now gets only engine updates. Novelty praise not evidence of lasting usability.

### Is the audience known well enough to leave convention?
- When: before committing to any novel pattern.
- Do: known audience behaviour, preferences + needs = precondition for leaving convention. Back either route (convention / novelty) w/ strict tests + research.
- Avoid: leaving convention w/o this knowledge.
- Hypothetical: pension portal weighing swipe-based fund picker first interviews members + tests it vs standard list before deciding.

### Where may the novelty go? (familiar core, novel periphery)
- When: departure has purpose.
- Do: keep functional core familiar, innovate at periphery. Product's primary job sets its structure. Core conventional where expectations strongest. Novel elements carry function, not only decoration. Iterate them via many cheap prototypes.
- Avoid: novelty leaving product harder to use. Rethink any pattern people have not met before wherever it worsens experience.
- Case: concert hall (design won 1988 competition, four finalists): radical exterior + conventional "modified shoebox" interior; every facade pipe of its 6,134-pipe organ functional.
  - Caveat: support for familiar core + novel periphery here = single architectural case, not user study.
- Case: Perplexity (AI search product): single query box = familiar entry point (core); novel controls around it: source focusing, file attachment, optional more-thorough mode (periphery).
- Hypothetical: museum ticketing site keeps standard basket + payment step, adds illustrated floor-plan exhibition picker.

### Which learning curve to choose?
- When: two designs differ in learning speed vs speed once learned.
- Do: choose by how often people do task. Rare task → quick-to-learn design. Daily task → faster-plateau design, even if slower to learn.
- Avoid: judging novel pattern from single first-use trial.
- Hypothetical (rare): replacement-passport application → quick-to-learn form wins.
- Hypothetical (daily): pharmacist's stock-count screen used every shift → faster plateau wins.
- Hypothetical worked curve (two designs of ward nurse's daily medication-round screen): A: fewer repetitions to learn but plateaus at slower time per task; B: more repetitions to learn, plateaus at faster time per task + overtakes A after some days of use. Daily task → B. Compare both curves over many repetitions, not one first-use trial.

### How to roll out a substantial redesign? (opt-in rollout)
- When: substantially changing familiar product.
- Do: opt-in rollout: for set period, previous version one switch away while users try new one → they grow used to it + give feedback.
- Avoid: redesign putting everyday features out of reach (see bad case).
- Why: Mental Model. Process safeguards (staged rollout w/ withdrawal condition) = humane-side companion. Defaults patterns bound how products offer change: opt-in + symmetric exit.
- Good cases:
  - YouTube's 2017 desktop redesign to Material Design, after look largely unchanged for years, shipped opt-in + reversible.
  - Google did same opt-in, reversible rollout w/ Calendar + Gmail.
  - Users moved to new design when ready, w/o discordance.
- Bad case: Snapchat's early-2018 redesign put everyday features out of reach → mental-model discordance + heavy backlash: users protested en masse + some left for Instagram.
- Hypothetical: council's bin-collection app ships new layout behind "try the new look" switch; "back to classic" kept in menu for trial period + feedback link.

## Related
- ../methods/convention-or-new-pattern.md: when new pattern worth its learning cost.
- ../methods/object-oriented-ux.md: maps objects before screens; structures product around objects in user's model.
- navigation-and-menus.md: conventions: ordering, grouping, depth, visibility.
- onboarding-and-first-use.md: first-run experience when pattern unfamiliar.
- ai-and-automated-features.md: AI as reason for novelty, w/ new capability off by default.
- ../evidence/product-cases.md: real product examples of laws in use.
- ../methods/process-safeguards.md: staged rollout w/ withdrawal condition; humane companion to opt-in redesigns.
- defaults-and-choice-architecture.md: opt-in + symmetric exit; bounds on how products offer change.
- ../laws/jakobs-law.md: in play for following vs leaving convention.
- ../laws/mental-model.md: in play; existing models carry over via established patterns.
- ../laws/cognitive-load.md: in play; confusion from unfamiliar patterns raises it.
- ../laws/aesthetic-usability-effect.md: in play for conventions vs novelty.
- ../laws/choice-overload.md: in play for conventions vs novelty.
- calm-technology-and-device-etiquette.md: humane side; familiarity lets background product recede.
