# Anti-patterns and humane alternatives

## Contents
- Use when
- Lookup table
- Details per anti-pattern
- Related

Quick reference for most common harmful product patterns only (not every one): name to use, harm to people, humane alternative to ship.

## Use when
- Fast first pass over flow.
- Review finding needs pattern name + replacement.
- If no shared name (dash in Name column) → describe plainly in finding.
- More names → deceptive-patterns.md: full taxonomy w/ review names, mechanism + humane alternative each; 16 more named patterns, e.g. confusopoly, nagging, price-comparison prevention + behavioral-targeting lock-in.

## Lookup table
|#|What you see|Name to use|
|---|---|---|
|1|Infinite feed silently backfills new content + autoplay countdown starts next clip|Bottomless bowl / infinite scroll|
|2|Surprise content on pull-to-refresh; badge counts withheld/inflated|Variable reward / slot-machine loop|
|3|Pre-ticked consent boxes; tracking on unless opted out; banners: service assumes consent|Preselection / opt-out by default|
|4|Online sign-up, cancel needs phone call/many screens; guilt copy on decline|Roach motel, forced continuity; confirmshaming (guilt copy)|
|5|Fees only at last step; add-ons pre-placed in cart; decline hidden in another control|Hidden costs, sneak into basket|
|6|Sponsored items look like ordinary content; close button starts upgrade; tiny grey decline|Disguised ads, misdirection|
|7|Opaque ranking, no levers user can adjust; personalized 'for you' feed = only view|—|
|8|AI decisions execute silently, no appeal|—|
|9|Zero-click purchasing, sharing/sending; one-tap deletion w/o undo|—|
|10|Group, admin/automated actions override personal privacy settings|—|
|11|Tracking, location sharing/monitoring protected only vs strangers|—|
|12|Happy-path MVP; 'edge cases' deferred to later release never arriving|—|

## Details per anti-pattern

### 1. Bottomless bowl (infinite scroll)
- Harm: removes stopping cue + choice point to continue or stop → binges, rabbit-hole drift. Also breaks orientation, keyboard use + low-bandwidth access. Worst for minors.
- Ship instead:
  - New content ends → 'all caught up' marker.
  - Load More showing seen vs total, e.g. '48 of 312 seen'.
  - Search results + comparison tasks → pagination, not infinite scroll.
  - Autoplay countdown → 'up next' item, plays only after deliberate tap.
  - After long viewing sessions → ask if still watching before continuing.
- Limit: continuous loading OK only for aimless browsing of similar items.
- Hypothetical: kids' reading app chains short stories via autoplay countdown → 'up next' card waits for tap; end marker once new stories run out.

### 2. Variable reward (slot-machine loop)
- Harm: variable-reward loop drives compulsive checking.
- Ship instead: batch new items for predictable person-chosen times. Badge counts true: never withheld, never inflated.
- Hypothetical: work task tool flashes random 'something new' badge on refresh → updates batched into digest at time each person picks; badge = real count.

### 3. Preselection (opt-out by default)
- Harm: works because most people keep whatever default they get; loss aversion + inertia do rest.
- Ship instead:
  - Ask opt-in when choice matters, stating person's benefit.
  - Withdrawing consent as easy as giving.
  - Consent, identity/money at stake → no default at all.
- Hypothetical: pharmacy loyalty sign-up pre-ticks 'share my purchase history w/ partners' → unticked; ask when partner offer relevant, stating member's gain; one-switch withdrawal, same place.

### 4. Roach motel / forced continuity / confirmshaming
- Harm: hiding exit to keep customers = coercion. Revenue held only by friction collapses once friction goes.
- Ship instead:
  - Symmetric exit: same channel + step count as sign-up.
  - On cancel → one honest confirmation.
  - Decline option worded neutrally, no guilt.
  - Reminder before free trial turns paid.
- Hypothetical: gym chain: app sign-up, in-person cancel → in-app cancel w/ same steps as joining, one honest confirmation, plain 'Cancel membership' wording, reminder before any trial turns paid.

### 5. Hidden costs / sneak into basket
- Harm: exploit effort already sunk into flow + skimming.
- Ship instead: total price on first screen; add-ons unchecked, each price visible; all tiers in same units, shown at once.
- Hypothetical: ferry-booking site adds cancellation-cover fee at payment + pre-adds seat selection → total on first screen; add-ons unchecked w/ prices.

### 6. Disguised ads / misdirection
- Harm: turn inattention into agreement; person bears burden of telling what is what.
- Ship instead: ads labelled distinctly + consistently; every control does exactly what label says; decline as visible as accept.
- Hypothetical: property-listing app styles paid listings as ordinary results + labels upgrade button 'Done' → consistent 'Sponsored' label; 'Done' only closes; 'No thanks' as visible as 'Upgrade'.

### 7. Opaque ranking w/o levers (no shared name)
- Harm: people lose options they never see; product goals silently override person's own.
- Ship instead:
  - Chronological + following-only views alongside any ranked feed.
  - Controls to mute, tune + reset recommendations.
  - 'Why am I seeing this' explanation for ranked items.
  - Full unpersonalized catalog one tap away.
- Hypothetical: library e-book app opens only on ranked 'picked for you' shelf → 'newest' + 'from authors I follow' views, 'why this book', mute/reset, full catalog one tap away.

### 8. Silent, unappealable AI decisions (no shared name)
- Harm: erode accountability; silent automation leaves people less capable when w/o tool.
- Ship instead:
  - Queue AI outputs for human review + approval, not silent execution.
  - Legible reasoning + shown confidence.
  - Decisions reversible + open to appeal.
  - Generated answers w/ sources + corroboration.
  - Gate high-stakes queries.
- Hypothetical: hiring tool auto-rejects applicants by AI score w/o notice → scores queued for recruiter approval; reasoning + confidence shown; applicant can appeal; decision reversible.

### 9. Zero-click and one-tap irreversible actions (no shared name)
- Harm: remove pause protecting people vs impulse, accident + regret.
- Ship instead:
  - Before any money moves → review screen w/ total.
  - Sharing decided item by item.
  - Confirmation strength scaled to severity.
  - Moving money, sharing/deleting → delay-then-undo.
  - Catastrophic operations → type-to-confirm.
- Hypothetical: banking app sends transfer instantly on swipe → review screen w/ total, short delay w/ undo, type-to-confirm to close account.

### 10. Group or admin overrides of personal privacy (no shared name)
- Harm: case: group/admin actions overriding personal privacy settings have outed people to hostile families. Frictionless association (adding/listing people w/o their say) serves list compilers + hate groups.
- Ship instead: person's own privacy settings always beat group, admin/automated actions; tagging/listing by others only after person approves.
- Hypothetical: school-parents app lets admin add any parent to public member list despite parent's 'hidden' setting → personal setting wins; listing awaits parent's approval.

### 11. Tracking protected only vs strangers (no shared name)
- Harm: most common attacker vs tracking + monitoring features shares victim's home, devices + passcodes.
- Ship instead:
  - Design vs intimate-partner threat model.
  - Observed person controls location/monitoring signal.
  - Alert tracked person on every platform + via every sense.
  - Discreet way for tracked person to stop tracking + report it.
  - Warnings at setup + accountability trail.
- Hypothetical: luggage-tag tracker guards only vs strangers → threat model covers partner w/ phone access; tracked person gets sound, vibration + on-screen alerts on any phone, discreet stop + report, setup warnings + access log.

### 12. Happy-path MVP (no shared name)
- Harm: people outside happy path = marginalized people. Safety work deferred until after launch rarely ships.
- Ship instead: founding scenario from most vulnerable person's view; misuse cases ship w/ mitigations at launch; affected people counted in absolute numbers.
- Hypothetical: telehealth MVP assumes each patient has private phone + stable address, defers shared-device cases → founding scenario = patient sharing device w/ abuser; misuse mitigations at launch; affected patients reported as absolute count.

## Related
- deceptive-patterns.md: all patterns w/ review names, mechanism + humane alternative.
- attention-hijacks.md: ten levers taking attention vs person's interest + counters.
- ../patterns/feeds-scrolling-and-pacing.md: stopping points, infinite scroll, autoplay, variable rewards.
- ../patterns/defaults-and-choice-architecture.md: opt-in, equal-weight decline, symmetric exit, personal settings beating group actions.
- ../patterns/friction-undo-and-confirmation.md: confirmation graded by consequence, undo windows, speed bumps.
- ../patterns/ai-and-automated-features.md: human review, appeal, sources + uncertainty for generated answers.
- ../patterns/safety-and-abuse-resistance.md: misuse cases, intimate-partner threat model, vulnerable people.
- ../guides/symptom-to-fix-index.md: usability-side counterpart; observed problem → explaining law → fix.
