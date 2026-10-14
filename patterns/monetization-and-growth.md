# Monetization and growth

## Scope + principles behind these patterns
- Use for: humane patterns on how product earns + grows: revenue model · free tiers + paywalls · subscriptions over things already owned · virtual currency · randomised paid rewards · referrals · value shared w/ contributors · legal risk.
- Applies when: designing/reviewing pricing, trials, in-product purchases, rewards programmes, referral loops or contributor terms.
- Out of scope here: exit + cancellation → defaults-and-choice-architecture.md; named monetization tricks → ../ethics/deceptive-patterns.md.
- Principles underneath:
  - ../principles/intentional.md: revenue model choice.
  - ../principles/transparent.md: free-tier limits, owned things, virtual currency, legal risk.
  - ../principles/empowering.md: owned things, value shared w/ contributors.
  - ../principles/resilient.md: randomised paid rewards, legal risk.
  - ../principles/respectful.md: referrals + messages sent in someone's name.

## Two tests for any rewards programme, price display or referral loop
1. Whose goal does it serve?
2. Would person endorse influence if they saw it whole?
- Same test closes ../ethics/deceptive-patterns.md taxonomy.
- Why tests needed: mechanic changes character once money or social standing rides on it. Variable reward = compulsion loop; paid variable reward = stronger one.

### Choosing how the product earns: which revenue model?
- When: choosing/revisiting how product earns.
- Do: prefer models growing when product genuinely good (paid outright, subscription for delivered value, service fee, contextual advertising) over models growing w/ session length.
- Steps: per candidate revenue model → write down what it would reward team for building next quarter.
- Avoid: attention-based revenue in product meant to stay calm, then asking designers to defend attention against incentive paying for their work.
- Why: Intentional: pick model not needing attention to grow.
- Hypothetical: meal-planning service weighs flat fee vs ads; writing down what each would reward next quarter: fee rewards better plans while ads reward longer browsing.

### Freemium, trial or paywall: what to say before sign-up?
- When: freemium, trials, any paywall.
- Do: every tier's price in same units at same moment; state plainly where free tier stops; name amount + billing date before card taken; reminder before trial converts to paid.
- Avoid: free-tier limit revealed only once person's work sits inside product; free option buried beneath paid one; price rise disclosed only in help article.
- Why: Transparent (say what free tier does before sign-up).
- Hypothetical: photo-storage service's plan page states storage size where free tier stops + asks for card only on screen naming monthly amount + first billing date.

### Subscription between a person + something they already own: what keeps working?
- When: subscription sits between person + device, file or capability already paid for outright.
- Do: before purchase state exactly what stops working if person stops paying; anything bought outright keeps working after subscription ends; person's own content stays readable + exportable when plan ends.
- Avoid: printer refusing own cartridges once plan cancelled; finished work sealed inside lapsed subscription; update withdrawing function hardware shipped w/.
- Why: Transparent + Empowering (do not switch off what people own).
- Hypothetical: drawing tablet's cloud plan lists before purchase what stops on cancelling (sync between devices); drawings saved on tablet stay openable + exportable afterwards.

### Points, coins, gems or credits: how to keep real cost legible?
- When: points, coins, gems or credits sit between person + their money.
- Do: cash equivalent beside every purchase; sell currency in amounts mapping cleanly onto item prices; running total of money spent.
- Avoid: bundles sized so remainder always stranded; several currencies + conversion rates making price comparison impractical.
- Why: Transparent. Multiple currencies + conversion rates = price-comparison prevention + hidden costs patterns of deceptive-pattern taxonomy, in game wrapping.
- Hypothetical: transit app sells ride credits in packs matching fares exactly → none left over; wallet screen keeps running total of money spent.

### Purchase w/ an unpredictable outcome: allow it?
- When: purchase produces unpredictable outcome: loot boxes, packs, spins, mystery bundles.
- Do: randomised paid rewards = gambling mechanics; publish odds; cap spend on randomised rewards per period; offer same items at plain fixed price; keep randomised paid mechanics out of anything minors can reach.
- Avoid: defending paid randomness as excitement.
- Why: Resilient. Persuasive design works best on still-maturing brains. Paid random rewards build purchase flow on same intermittent reinforcement driving slot machines → avoid it.
- Hypothetical: puzzle game hides paid mystery chest from minors' accounts + caps what adults can spend on chests each week.

### Money or standing rides on a streak: which tests apply?
- When: money or social standing rides on unbroken streak.
- Do: apply monetization tests too (streaks, leaderboards + social comparison as progress mechanics → habits-streaks-and-gamification.md).
- Why: paid streak repair, subscription justified by streak number, or public rank → habit aid becomes monetised compulsion loop.
- Hypothetical: reading-habit app keeps streak private + free to restore after illness, no paid "streak shield".

### Growth depends on people bringing in others: what may be sent in their name?
- When: growth depends on people bringing in others.
- Do: per-message consent for every message sent as person; show exact recipients + wording before anything sent; imported contacts used once, only for stated purpose. Reward what newcomer receives, not invitation count.
- Avoid: harvested address books; reminder waves supposed sender never saw; invitation step disguised as account setup.
- Why: Respectful.
- Case: in 2015 one network paid 13 million dollars over reminder invitations sent in members' names.
- Hypothetical: savings app's referral page lists contacts person picked + exact message text; nothing goes out until they tap send; reward goes to newcomer, not to invite count.

### Product's worth comes from what people contribute: who gets the value?
- When: worth depends on what people contribute (posts, photos, code, answers, reviews, rooms, vehicles, labour) or on data trail of all of it.
- Do: contributors = partners in business, not its audience; say plainly what contributions earn business; pay contributors/share revenue where their work draws others in; notice + genuine say before changing rules governing contributions; anyone can leave w/ what they made, in form usable elsewhere.
- Avoid: keeping everything contributions earn while calling it free service; rule change devaluing years of someone's work, announced only once already in effect.
- Why: Empowering + Transparent.
- Hypothetical: tutoring marketplace tells tutors well ahead of any commission-rule change + lets them comment before it takes effect.

### Growth depends on something local rules restrict: who carries the legal risk?
- When: growth depends on people doing something local rules restrict: letting rooms, driving for hire, subletting, reselling, working second job.
- Do: in commitment flow state rule applying at person's location + its penalty; compliant path = default; refuse to publish what local rule forbids; where you encouraged behaviour, carry consequence yourself, not leaving fine, eviction or record w/ individual.
- Avoid: launching first + negotiating later on assumption of short fight, then defending position by pointing at hardship of people you exposed to fines.
- Why: Transparent + Resilient (do not route legal risk onto users).
- Hypothetical: ride-for-hire app shows new driver local licence rule + fine for driving w/o one before first trip; driver can accept rides only once licence on file.

## Related
- habits-streaks-and-gamification.md: streaks, counters + leaderboards as progress mechanics.
- defaults-and-choice-architecture.md: exit + cancellation, opt-in, equal-weight decline.
- ../ethics/deceptive-patterns.md: named tricks (hidden costs, price-comparison prevention) + closing test of whose goal is served.
- transparency-and-honesty.md: true cost before click; data, purpose + revenue explained together; honesty tests.
- lists-options-and-choice.md: usability side: pricing tiers, option counts + comparison.
- feeds-scrolling-and-pacing.md: variable rewards + stopping points in feeds.
- ../evidence/business-cost-of-deception.md: fines, refunds, churn + trust loss.
- ../methods/counter-metrics.md: pairing each growth metric w/ harm it could hide.
