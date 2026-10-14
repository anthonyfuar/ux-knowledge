# Complexity management

## Scope + laws behind these patterns
- Use for: usability patterns allocating irreducible complexity: keep it off primary surface · progressive disclosure · mobile first · progressive enhancement · start simple · offload user tasks · complex expert applications · settings pages.
- Applies when: designing/reviewing feature-heavy products, expert tools, settings/preferences pages, any add/hide/remove-option decision.
- Laws underneath:
  - ../laws/teslers-law.md: who absorbs irreducible complexity.
  - ../laws/occams-razor.md: simplest working solution first.
  - ../laws/hicks-law.md: fewer visible options.
  - ../laws/cognitive-load.md.
  - ../laws/pareto-principle.md: most-used items first.
  - ../laws/paradox-of-the-active-user.md.
  - ../laws/cognitive-bias.md: complexity bias; distrust own taste for complex solutions.

### Who carries the irreducible complexity?
- When: any process w/ inherent complexity.
- Do: explicitly name core (irreducible) complexity → explicitly assign its carrier. Default: system + builders absorb it, not user.
- Avoid: leaving allocation implicit.
- Why: Tesler's Law: saving each of millions of users one more minute usually worth one more week of one engineer's simplifying work. Some retellings add "a day" → quote undated form unless explicitly citing industry framing.
- Limit: counterpoint to Tesler's Law: people resist losing complexity → users answer simpler application w/ harder tasks.
- Hypothetical: online prescription refill cannot work w/o patient identity, medicine + pick-up pharmacy (team: these three = core complexity); system fills identity + last pharmacy from account → patient only confirms medicine.

### Feature-laden control surface: what stays on it?
- When: features accumulated on control surface.
- Do: physical/primary surface minimal; step-by-step structured menus take removed complexity.
- Avoid: one control per feature on primary surface.
- Why: Tesler's Law + Working Memory: menus hold complexity → minimal primary surface, little load on WM.
- Hypothetical: home thermostat wall unit = one dial + one confirm button; holiday mode, schedules + frost protection → step-by-step menu on companion screen.

### Progressive disclosure: default view or secondary layer?
- When: advanced features, secondary actions, extra content.
- Do: split by importance: key actions in first view; rest (expert features, supplementary content, minor actions) one layer down, close at hand: hover menu/accordion/toggle/dropdown.
- Avoid: hiding rest so well users take visible subset for all on offer (see navigation-and-menus.md).
- Why: Cognitive Load + Hick's Law: only key actions + content shown → less muddle, mental load + visual noise → attention on task. Scope: progressive disclosure = any control hiding content until person asks.
- Hypothetical: tax-filing form lists common deductions; "More deductions" toggle opens rarer ones in place → filers see everyday set first.

### Responsive product: which screen first?
- When: any responsive product.
- Do: smallest screen first; supporting features off by default, added selectively as viewport + device capability grow.
- Avoid: squeezing full desktop design onto phone; separate cut-down mobile site.
- Why: limited space forces only key tasks + content onto screen.
- Hypothetical: city transit site: phones show next departures + route search; service maps + fare tables appear as viewport widens; one site, no separate mobile one.

### Progressive enhancement: what must work everywhere?
- When: product reaches many browsers + devices of varied capability.
- Do: baseline = essential content + function for every user + device, must alone fully serve product purpose; enhancements only where browser capability + space allow.
- Avoid: core purpose depending on enhancement.
- Why: moves effort onto essential, off nice-to-have.
- Hypothetical: bank branch finder: plain address + opening-hours list works in any browser; interactive map loads only where browser + screen support it.

### Starting a design: how much goes in?
- When: start of any design.
- Do:
  - Never-introduced complexity > complexity trimmed later → start simple; add complexity only when needed.
  - Try simplest working solution first.
  - Test need for every element.
  - Trim interface until any further cut would muddy content's meaning or make it hard to locate; stop there.
  - Prune hard: element w/ no significance + nothing of worth to user comes out.
  - Simpler version of element available → swap it in.
  - Done-test: any element still removable → not finished; aim = minimal design; less = better.
- Avoid:
  - Treating off-canvas main menu / charm-driven motion as automatic experience upgrade.
  - Over-simplifying: stripping elements → abstract, meaningless interface.
  - Trading clarity for simplicity.
- Why: Occam's Razor. Limits: only for choosing between equally performing options; removing elements for simplicity must never break function.
- Hypothetical: first version of tenant repair-request form = one problem field, photo upload + preferred visit time; each further field must show what it adds before going in.

### Complicated solution feels smarter: trust it?
- When: complicated solution feels smarter than simple one (complexity bias).
- Do: distrust pull toward elaborate option = sign of problem not yet grasped. Assumption gate: none enters until problem watched + lived w/ longer.
- Avoid: adding assumptions before observing.
- Why: Cognitive Bias (complexity bias); each added assumption → failure more likely.
- Evidence: 1989 rule-inference study: hidden rule merely "any three ascending numbers"; given one sample triple, asked to infer rule → most participants proposed rules more elaborate than real one.
- Hypothetical: team designing school-absence reporting flow drafts branching rules engine; watching parents use it: single reason field + free text covers what they do.

### Flow makes people decide, remember or read: what can the system take over?
- When: flow makes person decide, remember or read.
- Do: system takes over deciding, remembering + reading via anticipatory design, reuse of user-supplied data, defaults user can still change.
- Steps: audit flow for three load causes → what screen offers (excessive options, missing clarity) · what it asks (excessive thought).
- Avoid: asking for what user already supplied.
- Why: Cognitive Load; Tesler's Law (system absorbs complexity). Humane bounds on such defaults → defaults-and-choice-architecture.md.
- Hypothetical: travel-insurance quote reuses trip dates + destination from booking; cover level pre-selected, changeable in one tap.

### Complex expert application: capability w/o clutter?
- When: tools for trained specialists (research, finance, analytics, operations) serving many domains + both novices + experts.
- Do:
  - Keep capability, cut clutter: options shown only when relevant to item in focus.
  - Let users skip ahead, go back + jump between steps; no rigid sequence.
  - Show secondary information in place.
  - Bridge to tools specialists already rely on.
  - Free-text notes on data sets, charts + models, + action history → users recover reasoning after break (../laws/working-memory.md).
- Avoid: rigid linear workflows; hiding so much → primary data loses interpretive context.
- Why: many domains + both novices + experts served → keep capability, cut clutter; notes + action history → reasoning recovered after break (Working Memory).
- Hypothetical: freight-planning tool shows hazardous-goods fields only once shipment flagged hazardous.
- Hypothetical: grant-application builder lists all sections in sidebar; applicant fills them in any order, returns to earlier ones w/o losing entries.
- Hypothetical: audit tool: expanding ledger row shows entry's change trail inside list, w/o opening new page.
- Hypothetical: hospital-scheduling tool takes roster pasted from staff's existing rota software, writes results back in rota software's format.

### Settings page w/ many toggles: organise + save how?
- When: products w/ many settings/toggles.
- Do:
  - Group by task/object under labelled sections (../laws/common-region.md, ../laws/chunking.md).
  - Most-used settings first, confirmed by analytics (Pareto Principle).
  - Search matches setting names, synonyms, descriptions + values, not only exact names.
  - One visible save model: auto-save per change + inline saved confirmation, or explicit save + sticky bar from first change.
  - Warn before navigation discards unsaved changes.
  - Dependent setting shown disabled w/ reason, not hidden.
  - Advanced settings behind progressive disclosure (Tesler's Law).
- Avoid: single Save button at end of long scrolling settings page; changes silently lost on navigation.
- Why: long settings page load = scanning + finding (../laws/cognitive-load.md, ../laws/selective-attention.md), not choosing among alternatives. Save control out of view → unnoticed. Silently lost changes break visibility of system status.
- Misreadings:
  - Wrong: cite Choice Overload for settings page → Right: independent toggles, not alternatives to choose between.
  - Wrong: cite Fitts's Law for settings page → Right: problem = finding control, not reaching it.
  - Before citing any law for settings page → check ../guides/law-misapplications.md.
- Hypothetical: banking app settings grouped: cards, statements, alerts, security; search "paper" finds "statement delivery"; "overdraft alert threshold" greyed out w/ note "turn on overdraft alerts first".

### Defining what to build: outcome first or screens first?
- When: framing product/feature before design.
- Do:
  - Work backwards: first define real outcome people want.
  - Imagine ideal solution (e.g. teleportation for commuting) → add only layers current technology forces.
  - Count each layer pushed onto user (licences, skills, upkeep) as cost.
  - Treat product as necessary evil; should take minimal time + attention.
  - Design processes + systems, not screens.
- Avoid: success measured by time spent operating interface.
- Why: every layer between person + outcome costs them time + attention.
- Hypothetical: people do not want to file tax return; want affairs in order w/ tax office. Ideal = nothing to file; current constraint: office needs income confirmed → sends pre-filled return person only checks.

### Reviewing a design: how to surface unclear parts?
- When: design under peer review.
- Do: peer critiques in repeated rounds; ask reason behind every choice (../methods/design-critique.md).
- Why: ineffective/unclear parts surface once designers must justify every choice.
- Hypothetical: each critique round of hotel check-in kiosk: designer explains every screen element; elements w/o reason → removal list.

## Related
- ../methods/who-absorbs-complexity.md: allocating irreducible complexity between system + user.
- ../methods/cutting-to-essentials.md: applying Occam's Razor; simplify w/o losing function.
- ../methods/lightening-mental-effort.md: steps to cut extraneous load.
- ../methods/design-critique.md: structured critique; repeated peer-critique rounds.
- navigation-and-menus.md: navigation depth + visibility; where hidden options go unseen.
- ai-and-automated-features.md: AI absorbing complexity, intent-based interaction, automation hand-over.
- defaults-and-choice-architecture.md: humane bounds on defaults system sets when absorbing decisions.
- ../guides/law-misapplications.md: wrong uses of each law + correction; check before citing law for settings page.
- ../laws/teslers-law.md: who absorbs irreducible complexity.
- ../laws/occams-razor.md: simplest working solution among equally performing options.
- ../laws/hicks-law.md: fewer visible options.
- ../laws/cognitive-load.md: load from scanning, finding, deciding.
- ../laws/pareto-principle.md: most-used items first.
- ../laws/paradox-of-the-active-user.md: underlies these complexity patterns.
- ../laws/cognitive-bias.md: complexity bias.
- ../laws/working-memory.md: notes + history → users recover reasoning.
- ../laws/selective-attention.md: scanning load on long settings pages.
- ../laws/common-region.md · ../laws/chunking.md: labelled setting groups.
