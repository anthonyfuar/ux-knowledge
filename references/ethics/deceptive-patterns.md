# Deceptive patterns (dark patterns)

## Contents
- Use when
- Before naming a pattern
- Review steps
- Exit and billing
- Price and basket
- Emphasis, wording and controls
- Data, consent and accounts
- Pressure and attention
- Grey zone: shady patterns
- Persuasion or manipulation
- Related

Taxonomy, named deceptive (dark) patterns: mechanism + humane alternative to ship.

## Use when
- Reviewing flow for deception.
- Naming pattern in finding.
- Choosing replacement to ship.

## Before naming a pattern
- Term 'dark patterns' coined 2010; field increasingly uses 'deceptive patterns' instead.
- Deceptive patterns = engineered, not accidental. Several stacked in one flow → intent clear.
- Usually demanded by someone accountable for single metric.
- Deceptive patterns work short term; backfire via refunds, fines + lost trust. Case: settlements over deceptive patterns have reached 13, 62, 105 and 245 million dollars.
- In design reviews → use established names below.

## Review steps
1. Walk flow; each pattern found → its established name from this file.
2. If several patterns stack in one flow → record intent as clear, not accident.
3. If cue may count as legitimate persuasion → run test in Persuasion or manipulation (below).
4. Pick honest alternative listed under pattern.
5. Run second audit beside this table: six advantages system holds over human persuader ([persuasion asymmetries](persuasion-advantages-of-systems.md)).
6. Write finding in shape of ../guides/write-a-finding.md.

## Exit and billing

### Roach motel
- Mechanism: easy to join, hard to leave. Forms: phone-only cancel; hidden account deletion; must retype email 'to be removed'.
- Honest alternative: symmetric exit = leaving as fast + fully online as joining; one honest confirmation on leaving.
- Hypothetical: language school: online enrollment, withdrawal by signed letter posted to office → withdraw button on same account page, then one plain confirmation.

### Forced continuity
- Mechanism: card taken for free trial → billing starts silently when trial ends → cancellation buried.
- Origin: 1920s negative-option book clubs.
- Honest alternative: price + billing date stated at sign-up; reminder before billing starts; one-step online cancel.
- Hypothetical: meditation app takes card for trial, then charges w/o notice → sign-up screen shows price + first charge date; reminder before charge; one-step online cancel.

## Price and basket

### Sneak into basket
- Mechanism: extras (insurance, priority boarding, memberships) pre-added to purchase; decline option hidden inside another control.
- Honest alternative: add-ons unchecked w/ visible prices; default path buys only what person chose.
- Hypothetical: online pharmacy pre-adds paid 'express handling' line to every order, removable only in shipping dropdown → add-on unchecked, price shown, default order = picked items.

### Hidden costs
- Mechanism: shipping, tax/service fees shown only at final step, after effort sunk.
- Honest alternative: total price from first screen; optional fees in one table before checkout.
- Hypothetical: city parking-permit portal shows base fee, then adds processing + card fees on last screen → full total on first screen; optional fees in one table before payment.

### Price comparison prevention
- Mechanism: tier prices withheld, fragmented or in different units until deep in flow.
- Honest alternative: all tiers priced in same units, shown at once.
- Hypothetical: home-internet provider quotes basic plan per month, premium per day, business only after address entry → all plans per month, one screen.

### Confusopoly
- Mechanism: deliberately confusing offers + bundles → rational comparison impractical.
- Honest alternative: plain, comparable plans.
- Hypothetical: pet-insurance site sells overlapping bundles whose cover differs only in fine print → few plain plans in one comparison grid.

## Emphasis, wording and controls

### Misdirection
- Mechanism: visual emphasis draws eye to pricier option or one collecting more data. Form: free tier buried.
- Honest alternative: emphasis on what most people want. Highlight = claim about option; must hold true.
- Hypothetical: telehealth booking: paid video consult in big highlighted tile, free nurse phone line buried at bottom → emphasis on what most patients want; free option at equal weight; any highlight states only what holds true of its option.

### Trick questions
- Mechanism: double negatives; opt-out phrasing; 'on' meaning different things in different rows.
- Honest alternative: short positive statements; options unchecked by default; 'on' + 'off' mean same in every row.
- Hypothetical: bank settings page asks 'Do not stop paper statements?' next to row where 'on' means fewer mailings → 'Send paper statements' w/ unchecked box; 'on' = receive, in every row.

### Disguised ads
- Mechanism: ads styled as content, navigation, download buttons or on-screen debris.
- Honest alternative: distinct, consistent ad labels. Ads never inside answers/feeds w/o marking.
- Hypothetical: job board styles paid listings exactly like regular results + puts paid link in its assistant's answer → same 'Sponsored' label + style on every paid slot, answers included.

### Bait and switch
- Mechanism: control promises one outcome, delivers another.
- Honest alternative: controls do exactly what label says.
- Hypothetical: benefits-claim portal's 'Save draft' button submits claim → 'Save draft' only saves; submitting = separate, labelled step.

### Hidden No
- Mechanism: decline option shrunk, greyed out or missing. Forms: mandatory phone-number path hiding available email path; install walls w/ no way to dismiss.
- Honest alternative: equal-weight No on every prompt.
- Hypothetical: clinic patient portal: 'Enable SMS reminders' bright button + 'Not now' faint grey text → both same size + weight.

### Confirmshaming
- Mechanism: guilt-inducing copy on decline link.
- Honest alternative: neutral decline wording.
- Hypothetical: online course exit popup words decline link as learner giving up on career → 'No thanks'.

## Data, consent and accounts

### Privacy zuckering
- Mechanism: tricking people into sharing more than intended. Form: permissions presented as required when not.
- Honest alternative: ask only for what task needs + say why; offer anonymous mode.
- Hypothetical: recipe app marks contacts + precise location 'required to continue' → asks only for what cooking features need, says why, offers use w/o identity.

### Friend spam
- Mechanism: contacts harvested for 'find friends' → invitations + reminders sent in person's name.
- Honest alternative: contacts used once, for stated purpose; per-message consent for anything sent as person.
- Hypothetical: fitness-challenge app imports contacts to find friends, then keeps emailing invites signed w/ user's name → import for matching only; each invite only after user approves it.

### Data repurposing
- Mechanism: data given for security, learning/health used by default for discovery, research/ads.
- Honest alternative: data bound to purpose given for; new uses announced in advance + off by default.
- Hypothetical: bank collects phone number for login codes, then lets others find account holder by it → number for login codes only; any new use announced first, off until enabled.

### Opt-out defaults and pre-ticked consent
- Mechanism: tracking, sharing + marketing on until person refuses.
- Honest alternative: opt-in; withdrawal as easy as consent.
- Hypothetical: smart-TV setup ships viewing-data sharing on → off until owner enables it; disabling = one switch, same place.

### Forced sign-in and forced accounts
- Mechanism: people cannot use content/appliances w/o account or social login.
- Honest alternative: let people try product w/o profile; account required only where identity truly needed.
- Hypothetical: kitchen scale refuses to weigh until linked to online account → weighs w/o account; account only for cross-device history sync.

### Behavioral targeting lock-in
- Mechanism: ads follow people across web; opting out made deliberately hard.
- Honest alternative: contextual advertising; one clear tracking opt-out, honored everywhere.
- Hypothetical: travel-deals network retargets hotel search on every site + scatters opt-out across partner pages → ads based on current page; one opt-out, applied network-wide.

## Pressure and attention

### False scarcity and fake activity
- Mechanism: fabricated activity claims, inflated badge counts, thousands of fake notifications.
- Honest alternative: only true + proportionate cues. Vs fake notifications → predictable delivery. Scarcity cues = white-hat (legitimate persuasion) when true.
- Hypothetical: language-learning app sends 'your classmates are studying right now' alerts when no classmate active → activity cues only when real + proportionate; reminders at predictable times.

### Withheld rewards
- Mechanism: likes/messages held back + released when person most likely to reopen app.
- Honest alternative: deliver when event happens, or in scheduled digest person chose.
- Hypothetical: neighborhood-forum app holds replies until user most likely to reopen it → replies on arrival or in digest at user-set time.

### Nagging
- Mechanism: repeated prompts to enable notifications, rate, install apps or sign in.
- Honest alternative: ask once, in context; honor durable 'no'.
- Hypothetical: grocery site asks for app install every visit → offer once at relevant moment; after 'no', stop asking.

### Foot-in-the-door cost hiding
- Mechanism: small first action opens something w/ much larger true cost.
- Honest alternative: show true cost in time, steps + scope before click.
- Hypothetical: loan app 'check my rate' button starts full application incl. credit check → button first states time, steps + included credit check.
- Hypothetical: HR portal 'confirm your address' link opens whole benefits re-enrollment across many screens → link says it opens re-enrollment, w/ steps + expected time, before click.

### Bottomless bowl and autoplay
- Mechanism: feeds refill + players auto-advance → moment of choosing to stop never arrives.
- Honest alternative: 'all caught up' marker; Load More; 'up next' needing deliberate tap.
- Hypothetical: e-learning platform auto-advances to next lecture → 'up next' card waits for tap.

### Manufactured social obligation
- Mechanism: auto-suggested tags, endorsements + follows → reciprocation loops.
- Honest alternative: no prompts whose main purpose = pulling people back.
- Hypothetical: workplace chat tool auto-prompts kudos for coworkers, then tells each recipient to return favor → no prompt whose main purpose = bringing people back.

## Grey zone: shady patterns
- Shady patterns = grey zone: company's agenda over person's w/o outright deception.
- Honest alternative: system advocates for person; disclose system's nature.
- Hypothetical: hotel-booking site 'best for you' sort quietly ranks higher-commission hotels first, w/o stating anything false → sort follows traveller's request; page discloses site earns commission + how ranking works.

## Persuasion or manipulation
- Reviewing pattern → distinguish persuasion from manipulation.
- White-hat = legitimate persuasion; black-hat = manipulative. Scarcity cues = white-hat when true.
- Test:
  1. Whose goal does influence serve?
  2. Would person endorse influence if they understood it?
- Hypothetical (black-hat): grocery app infers from usage when each shopper tired late at night + times impulse-buy pop-ups for those moments → serves business goal; shoppers would not endorse it if they understood it.

## Related
- [Persuasion asymmetries](persuasion-advantages-of-systems.md): six advantages system holds over human persuader; second audit beside this table.
- anti-patterns-and-humane-alternatives.md: quick table, most common offenders + what to ship instead.
- attention-hijacks.md: ten levers taking attention against person's interest + counter to each.
- [Influence versus manipulation](influence-vs-manipulation.md): usability-side counterpart; line-drawing test per psychological lever.
- ../patterns/defaults-and-choice-architecture.md: opt-in, equal-weight decline, symmetric exit.
- ../patterns/transparency-and-honesty.md: transparency of data, algorithms + business model; honest controls, true cost, honesty tests.
- ../evidence/business-cost-of-deception.md: evidence on fines, refunds, churn + trust loss.
- ../guides/write-a-finding.md: shape of review finding using pattern name.
