# Transparency and honesty

## Scope + principles behind these patterns
- Use for: humane patterns for honest disclosure of data use, revenue, ranking + advertising · controls doing what label says · true cost up front · tests of design honesty.
- Applies when: designing/reviewing disclosures, ad labelling, price display, button + close-control behavior, ranking/recommendation explanations, or any mechanic leaning on bias or working against product's stated purpose.
- Principles underneath:
  - ../principles/transparent.md: most entries serve it.
  - ../principles/intentional.md: veil-of-ignorance + purpose-consistency tests.
  - ../principles/empowering.md: interface explaining algorithm.

### Disclosing what the product does w/ data?
- When: disclosing product's practices (explain data, purpose + revenue together).
- Do: state why each data item needed, how it makes money + what it collects, at same detail level as data itself. Cannot explain data practice, or would rather not → do not do it.
- Avoid: "your data is used for ads" as whole disclosure. Omission dressed up as simplicity = not honest disclosure.
- Why: ../principles/transparent.md.
- Hypothetical: fitness tracker's data page lists each data item beside feature it powers + whether it earns revenue.

### Ranking, targeting or generation shapes what people see?
- When: ranking, targeting or generation shapes what people see (let interface explain algorithm).
- Do: "why am I seeing this" explanation on ads + recommendations. Expose attributes algorithm used. Following-only + chronological views alongside ranked ones. Publish honest usage figures, normalized by run time, + say hours alone not goal.
- Avoid: feeds mixing recommendations + paid content w/ no explanation. Celebrating billions of hours watched as headline.
- Case: one semi-annual engagement report adjusts viewing figures by run time.
- Why: ../principles/empowering.md; steering controls in recommendations-and-personalization.md.
- Hypothetical: podcast app shows "suggested because you finished other history series" under each pick + offers "subscriptions only, newest first" tab.

### Paid placement appears?
- When: wherever paid placement appears (make ads unmistakably ads).
- Do: label ads consistently. Separate ads visually from content, navigation + answers. Sponsored items out of generated summaries.
- Avoid: native ads indistinguishable from posts. Ads shaped as giant fake "Download" button. Ads drawn as hair or dust speck on screen. Restyling organic results to resemble ads.
- Why: ../principles/transparent.md.
- Hypothetical: hotel-search results tag every paid listing "Ad" in same spot + style each time, divider between paid + unpaid results.

### Any button, link or close control?
- When: any button, link or close control (controls do exactly what their label says).
- Do: follow control conventions: close button closes, uninstall uninstalls. Primary + dismiss actions visually honest.
- Avoid: red close button starting upgrade. "Decline" as faint grey text beside bright "accept".
- Why: ../principles/transparent.md.
- Hypothetical: photo-editing app's "Close" on upgrade pop-up only closes it; upgrade offer = separate, plainly labelled button.

### Consequence larger than it looks?
- When: action's consequence larger than it looks (show true cost before click).
- Do: attach action's time, steps + scope to action itself. All mandatory charges beside headline price. Optional fees in one table before checkout.
- Avoid: shipping cost revealed only at last step. 15% service fee appearing only after person's effort sunk.
- Why: ../principles/transparent.md.
- Hypothetical: concert-ticket site folds booking fee + venue levy into headline price + lists optional parking + refund cover in one table before checkout; "transfer tickets" states upfront it cancels original barcodes.

### Adding a convenience or personalization feature?
- When: adding convenience/personalization feature (name trade-off).
- Do: state, internally + to people, what feature trades: data, attention, autonomy or third-party harm. Decide whether exchange fair. Teach data literacy in context → consent informed, not blind.
- Avoid: presenting convenience as free.
- Why: ../principles/transparent.md.
- Hypothetical: smart thermostat's auto-away setting explains on switch-on: it uses motion sensor + what sensor reveals about when home empty.

### Design leans on a cognitive bias?
- When: design leans on cognitive bias, e.g. inertia, loss aversion, sunk cost, reciprocity ("if they knew" test).
- Ask:
  1. How would person feel if they understood exactly what happens, + would they choose it?
  2. Would you accept this used on your parent or your child?
  3. What would future whistleblower say about it?
- Avoid: optimizing conversion w/ tactics you would hide from person converted.
- Why: ../principles/transparent.md; ../laws/cognitive-bias.md = usability-side law on biases design can lean on, bounded by this test. More tests in ../ethics/influence-vs-manipulation.md.
- Hypothetical: subscription-box cancel screen warns leaving "throws away everything you have built", leaning on sunk cost; person would not choose it if they saw tactic → fails test.

### Decision sorts people into unequal positions?
- When: decision sorts people into unequal positions: account holder vs located person; driver vs street resident; camera buyer vs everyone it films; reviewer vs reviewed (decide w/o knowing what side you would land on).
- Ask: veil-of-ignorance question = would this arrangement look acceptable if you did not know what position you would end up in? Origin: put at center of a theory of justice.
- Do: rule nobody would accept from weaker side → record as finding, not trade-off.
- Avoid: weighing account-holder benefits against everybody else's costs as though audience = account holders only. Counting buyer's consent as consent from people affected by purchase.
- Why: ../principles/intentional.md + ../principles/transparent.md.
- Hypothetical: neighborhood-review app's policy on photos of other people's homes, checked from reviewer's side + from side of household shown.

### Mechanic works against the product's stated purpose?
- When: mechanic works against product's stated purpose: streak in something meant to calm, urgency in something meant to relieve stress, comparison score in something meant to build confidence, hoarding loop in something meant to declutter (purpose-consistency test).
- Steps:
  1. Write product's purpose in person's own words on one line.
  2. Next line: write what mechanic does to person's day.
  3. Read both lines together.
  4. They contradict → state as finding: this mechanic fails purpose-consistency test.
  5. Change mechanic, or admit purpose = marketing copy.
- Avoid: judging mechanic only against engagement targets; there it always looks fine. Softening wording while mechanic keeps working opposite way.
- Why: ../principles/transparent.md + ../principles/intentional.md.
- Hypothetical: decluttering app adds badge collection rewarding buying storage gadgets → line 1 (own less) contradicts line 2 (hunts for more items).

### Citing evidence for or against a design decision?
- When: citing evidence for/against design decision (verify stories + statistics).
- Do: check founding anecdotes + third-party numbers before using them. State uncertainty in evidence you cite. Do not cherry-pick report suiting you.
- Avoid: quoting headline statistic w/o its rebuttal.
- Case: tale of oaks planted centuries ahead to replace hall's beams = debunked → do not repeat it.
- Case: in one short-term-rental dispute, each side relied on numbers other side rejected.
- Why: ../principles/transparent.md.
- Hypothetical: team arguing for dark-mode default cites vendor's battery-saving figure + notes vendor sells feature + independent figures missing.

## Related
- ../principles/transparent.md: principle most transparency entries serve.
- ../ethics/deceptive-patterns.md: named deceptive patterns, how each works + honest alternative.
- ../ethics/influence-vs-manipulation.md: further tests of whether persuasive lever serves person or exploits them.
- privacy-data-and-security.md: data minimisation, consent, access + deletion, tracking.
- recommendations-and-personalization.md: algorithm-ranked feeds + steering controls going w/ explaining them.
- monetization-and-growth.md: revenue models, free tiers, virtual currency, referrals.
- ../evidence/business-cost-of-deception.md: fines, refunds, churn + trust loss from deceptive patterns.
- ../laws/cognitive-bias.md: usability-side law on biases design can lean on; if-they-knew test bounds such use.
