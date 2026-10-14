# Inclusive and accessible design

## Scope + principles behind these patterns
- Use for: people design would otherwise exclude: persona spectrum · accessibility floors (zoom, motion, contrast, readable text, semantics) · common devices + slow connections · emotional state · fallback channels · identity fields · co-design · indirect users · marketplaces where one person accepts/refuses another.
- Applies when: designing/reviewing any feature for whom it excludes; acting on accessibility audit; form/profile/verification step encodes identity.
- Principles underneath:
  - ../principles/inclusive.md: most entries serve it.
  - ../principles/resilient.md: fallback channels, slow connections, accept-or-refuse marketplaces.
  - ../principles/empowering.md: co-design w/ excluded people.

## Frame
- Inclusive design frames disability = person-design mismatch.
- Mismatch can come from permanent/temporary/situational limits.
- Rule: solve for strongest constraint first → extend to everyone.

### Whom does each assumed ability leave out?
- When: product assumes ability: sight, hearing, one-handed use, attention, language or calm mood (mapping persona spectrum).
- Do: per assumed ability, name 3 people lacking it: one permanently, one temporarily, one situationally → design for all 3.
- Avoid: one average persona: able-bodied, fluent, on fast connection.
- Why: ../principles/inclusive.md; mismatches can come from permanent/temporary/situational limits.
- Hypothetical: voice-only pharmacy refill flow serves blind customer (permanent), someone w/ dilated pupils after eye exam (temporary), cook w/ flour-covered hands (situational).

### Start a new feature from disability, or audit it later?
- When: starting feature, not auditing it later.
- Do: accessibility = leading constraint → generalize to everyone. Coded accessible pattern library + automated accessibility checks on every commit. Verify w/ screen readers, keyboard-only use + contrast checks.
- Avoid: ship first → bolt on accessibility fixes after complaints. Degraded accessible version off to side of main product. Auto-captions meeting letter of accessibility rule but unreadable at speed = failure, not real access.
- Why: ../principles/inclusive.md; strongest constraint first → solution extends to everyone.
- Hypothetical: transit trip planner built first for blind riders (spoken step-by-step directions), later offered to every rider as hands-free mode.

### Audit came back clean: is inclusion done?
- When: conformance audit clean + team treats inclusion as done (access = floor, not finish line).
- Do: judge accessible result by whether experience worth reaching: plain language, sane structure, tasks people can complete unaided.
- Avoid: claiming inclusion from checklist total. Usability + access problems in separate queues, different owners.
- Why: clearing access barriers to confusing product only lets more people meet confusion. Reverse too: interface nobody can operate = not accessible either, whatever audit score. ../principles/inclusive.md.
- Hypothetical: pension-estimate tool passes every automated check; steps use actuarial terms, result page has no plain summary → people reach it w/o understanding it.

### Follow the standard pattern because everyone does?
- When: reaching for established pattern because everyone uses it (convention = default to check).
- Do: convention = starting point. Verify w/ people it might exclude. Invent only in content + where convention shown to fail somebody.
- Avoid: novel interface mechanics for own sake. Defending pattern solely because standard after someone showed it blocks them.
- Why: conventions' predictable placement + behavior lower everyone's learning cost. Many settled by interface builders, matching how they themselves work. ../principles/inclusive.md.
- Hypothetical: travel site keeps familiar month-grid date picker as default, tests it w/ screen-magnifier users: grid runs off their view → adds typed-date field only for this failure.

### Writing layout or viewport code?
- When: writing any layout/viewport code (preserve platform accessibility controls).
- Do: keep reduced-motion, font scaling, contrast settings + pinch-zoom working.
- Avoid: magic-number dimensions → layouts must reflow at 200% zoom. Locking viewport scale. Fixed pixel type sizes ignoring device text-size setting.
- Why: ../principles/inclusive.md.
- Hypothetical: hotel-booking site at 200% browser zoom stacks room cards in one column, not clipping price off-screen.

### Motion, autoplay or an endless feed on the page?
- When: infinite scroll, autoplay, animations or parallax present.
- Do: reduced-motion toggle + paginated alternative to endless feed.
- Never: autoplay media.
- Avoid: flicker, elements appearing suddenly, scroll-jacking. Decorative motion w/ no off switch.
- Case: major operating-system release shipped motion effects causing nausea for people w/ vestibular disorders.
- Why: ../principles/inclusive.md.
- Hypothetical: banking app drops animated confetti + counting-up balance when phone's reduced-motion setting on; promo videos wait for tap.

### Choosing type, contrast and state colors?
- When: any text/state indicator.
- Do: normal text contrast ≥4.5:1. Large text ≥3:1. Pair color w/ text/texture cue for every state.
- Never: color alone to convey state.
- Avoid: grey-on-white text aesthetics. Error shown only as red outline.
- Why: ../principles/inclusive.md (legible type, generous contrast, cues beyond color).
- Hypothetical: hospital bed-availability board marks full ward w/ striped fill + word "Full", not only red tile.

### Writing interface copy and instructions?
- When: writing interface copy + instructions (readable text = default).
- Do: write as you speak: short sentences, common words. General content: ~eighth-grade reading level. Check copy w/ readability score. Anxious users → guidance: write as if addressing ten-year-old.
- Avoid: jargon assuming domain expertise.
- Why: ../principles/inclusive.md.
- Hypothetical: tax-office letter replaces "remittance is due upon assessment" w/ "Pay by the date at the top of this letter."

### Building an interactive element or page structure?
- When: building any interactive element (native semantics + keyboard-first structure).
- Do: right native elements, headings + landmarks. Visible keyboard focus. Skip link. Label links + form fields by purpose. Proper feed role on feeds. Cut + order page content before decorating. Page purpose at top of document order. Shed features surviving only out of habit.
- Never: keyboard traps. Hiding element from assistive technology instead of removing it.
- Avoid: custom controls removing focus outlines. Structures making screen-reader users walk through every element.
- Why: screen-reader listeners + keyboard tabbers meet everything in sequence → each extra control, banner or decorative block = toll on them. Restrained page content = cheaper to build + better for everyone. ../principles/inclusive.md.
- Hypothetical: clinic appointment page puts booking form first in document order, drops decorative staff-photo slider kept only out of habit → keyboard user reaches booking in a few tab presses.

### Reviewing only on fast screens and fast links?
- When: reviews only on designer monitors over office fiber (design for commonest device + slowest connection).
- Do: test on mid-range phones + small laptops. Throttle test connection to target region's typical speed. Trim scripts + media for slow connections + common devices.
- Avoid: assuming 4K screens + gigabit links.
- Evidence: 2016, typical connection speed in some markets ~3 Mbps. 2017 survey: most common phone screen resolution 360x640.
- Why: ../principles/inclusive.md + ../principles/resilient.md.
- Hypothetical: regional bus-ticket site reviewed on mid-range phone, throttled connection → team drops home-page background video, defers chat-widget script.

### Task is high-stakes or unfamiliar?
- When: high-stakes/unfamiliar tasks (account for anxiety + emotional state).
- Do: distinguish system failures from user errors + name fault's source, e.g. "this was our fault". State next step. Feedback at every stage. Action effects clear + undoable. Lighten account + password burdens for anxious/occasional users. Reduce countdowns + alarmist copy.
- Avoid: generic "something went wrong" leaving person convinced they broke rules. 5 password rules + many-step reset for site used once/year.
- Why: ../principles/inclusive.md.
- Hypothetical: first-time visa applicant's payment fails because gateway down; page says fault on consulate's side, application saved + next steps, not bare error leaving them sure they filled something wrong.

### Essential task is digital-only?
- When: critical task digital-only (two channels for every essential task).
- Do: ≥1 alternative channel per essential task: phone, paper, chat or in person. All channels for same task consistent w/ each other.
- Avoid: declaring online forms required, no fallback when site fails.
- Why: ../principles/resilient.md.
- Hypothetical: people can file utility company's outage-compensation claim at service counter too, same fields + deadline as online form.

### Form or profile encodes who somebody is?
- When: form/profile/verification step encodes identity: names, gender, family, address, age, language (let people describe themselves accurately).
- Do: accept names people go by: single, non-Latin-script, very long, chosen. Allow name change w/o document. Allow household of one adult, three, or none of familiar shapes. Anything consequential in language audience genuinely reads. Let people correct wrong inference about them w/o proving something else in process.
- Avoid: consent flow assuming two parents. Important notice in one language only. Validation declaring real name invalid.
- Why: ../principles/inclusive.md.
- Hypothetical: school enrollment form lets family list whichever caregivers it has under any relationship label + takes child's name in any script.

### How to involve excluded people?
- When: across research, ideation, testing + iteration (co-design w/ excluded people).
- Do: bring disabled people + misrepresented communities in as compensated co-designers + decision makers. Monthly, sit w/ one excluded person + watch how they work in practice. Run each "all people can..." statement about product → find for whom it's false.
- Steps (opening move): 1. Say plainly what you ask of them. 2. Ask what would make taking part worth their while. 3. Honor answer in money, credit, advisory seat or decision power.
- Avoid: recruiting excluded people at end only to confirm team right. Disability simulations replacing work w/ disabled people; supplement only. Two-hour screen-reader simulation → sympathy, not insight.
- Attitudes sinking co-design: assuming you're room's expert; so afraid of wrong word you never begin; keeping every decision in your own hands; avoiding communities you don't already know; rescuer posture treating people as unable to name own needs.
- Case: one co-design effort w/ deaf community revealed many bilingual, English as second language → reshaped caption + reading-level decisions.
- Why: honoring what participants say would make it worthwhile turns transaction into partnership; also practical answer to fear of tokenizing. ../principles/empowering.md.
- Hypothetical: city parks department pays wheelchair users as voting advisors on playground layout, after asking each what would make sessions worth their time.

### Accessible route works but is joyless?
- When: accessible route correct but joyless, built only to satisfy rule (design past merely functional).
- Do: aim accessible experience at same pleasure, humor + craft everyone else gets. Partner w/ one excluded person + build something exactly for them. Allow ideas sounding ridiculous at outset. Harvest whatever works back into main product.
- Avoid: stripped-down variant parked aside as "the accessible version". Treating disabled people as subjects to study, not designers to work with.
- Why: unexplored design territory rewards play. One tailor-made experience flips assumption (disabled people owed function while everyone else owed delight) + yields ideas compliance pass never reaches. ../principles/inclusive.md.
- Hypothetical: cooking-class platform co-built w/ deaf home cook adds playful visual sizzle cues + witty captions; what works then offered in main product, e.g. to cooks in loud kitchens.

### Product affects people who never open it?
- When: product affects people never opening it, or amplification mechanics ship into regions w/ existing tensions (indirect users + fragile contexts).
- Do: include residents, renters, pedestrians, bystanders + stalking victims in product success criteria. Evaluate product mechanics beyond home market.
- Avoid: defining user only as account holder. Testing social mechanics only in stable markets.
- Case: routing app turned quiet residential streets into cut-throughs; residents had no channel to object.
- Why: ../principles/inclusive.md; continued in [safety patterns](safety-and-abuse-resistance.md).
- Hypothetical: smart-doorbell maker counts passers-by filmed on sidewalk as affected people when choosing default recording zone.

### One person can accept or refuse another?
- When: product lets one person accept/refuse another: host approving guest, driver taking ride, landlord, lender, hiring screening step.
- Do: decide deliberately what identity signals show before decision. Withhold bias-inviting signals until after it. Offer ≥1 route removing discretion under stated rule. Publish standard both sides held to. Measure acceptance + rating gaps between groups. Treat group acceptance/rating gap like outage.
- Avoid: calling refusal private choice between two adults, none of product's business. Learning of group disparity from press or lawsuit.
- Case: lodging marketplace answered documented refusals of guests of color w/ non-discrimination commitment every host had to accept before listing.
- Why: ../principles/inclusive.md + ../principles/resilient.md.
- Hypothetical: tutoring marketplace shows tutors student's subject + level; name + photo only after acceptance; instant-book route skips tutor approval for students meeting posted rules.

## Related
- ../principles/inclusive.md: principle most entries serve; definition, practices, audit questions.
- ../principles/resilient.md: fallback channels, slow connections, marketplace safeguards.
- ../principles/empowering.md: co-design w/ excluded people.
- ../evidence/inclusion-and-exclusion-costs.md: evidence on people left out + cost.
- ../checklists/humane-design-audit.md: yes/no questions per humane principle, Inclusive included.
- forms-and-data-entry.md: field usability, formats, validation timing, accessible errors; bounded by letting people describe themselves accurately.
- departing-from-convention.md: when to follow vs deviate from conventions; bounded by checking convention w/ people it might exclude.
- errors-and-input-tolerance.md: error recovery + tolerant input; usability side of anxiety + naming entries.
- feeds-scrolling-and-pacing.md: stopping points, infinite scroll, autoplay; neighbors motion + endless-feed switches.
- safety-and-abuse-resistance.md: misuse cases, blocking + reporting, vulnerable people; continues indirect users + fragile contexts (stalking, residents contesting changes, institutional fragility) + keeps displayed name separate from legal name.
