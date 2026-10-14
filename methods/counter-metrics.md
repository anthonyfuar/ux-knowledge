# Counter-metrics

## Use when
- Setting / reading feature's growth metrics: before launch + while monitoring after launch.
- Why: until team measures what it values, it over-values what it measures.

## Steps
1. **Pair every growth metric** w/ user-goal metric + counter-metric flagging harm. See pairing table below.
2. **Track abuse beside growth**: moderation false positives + negatives; periodic surveys: people feel safe? safety tools seem sufficient to them?
3. **Before launch, per counter-metric:** set trip value + attached action. Counter-metric w/ no agreed response = decoration.
4. **Name one person** w/ authority to act on tripped counter-metric w/o reopening debate.
5. **Agree in writing, before any numbers exist:** where growth metric + its counter-metric move together, counter-metric beats growth metric until cause understood. Written beforehand because ordering gets contested once chart exists to argue over.
6. **When counter-metric trips →** apply response table below.

## Pairing table
|Growth metric|User-goal metric|Counter-metrics (harm flags)|
|---|---|---|
|Opens per week (banking app)|financial peace of mind; task done in one visit|compulsive re-opens; anxiety reports|
|Session length (feed)|person found what mattered, then left|regret after use; late-night sessions; self-reported "wasted time"|
|Daily active people (habit / progress feature)|practice continued at person's own pace; benefit person reports|near-zero-length sessions; activity crowded into last minutes before midnight; returns driven by loss-framed reminders; guilt / anxiety about missing one day|
|Streak length + completion rate|value per session; return after gap|share stopping entirely after one break; count of paid streak repairs / freezes bought; heaviest-use decile growing faster than median user; counters hidden / reset by people|
|Sign-ups / newsletter opt-ins|informed opt-ins staying subscribed|unsubscribes within one week; spam flags; complaints|
|Conversions|help requests answered + person's problem solved|refunds; chargebacks; complaints about friction when cancelling|
|Messages sent|continued conversations|first messages never replied to; blocks / reports following unreplied message|
|Shares / forwards|shares of content read|misinformation spread; pile-ons|

## Response when a counter-metric trips
|Situation|Do|Avoid|
|---|---|---|
|Harm signal moves on any segment, cause unknown|investigate w/ deadline; feature holds current rollout stage|expanding rollout further meanwhile|
|Harm real, from size / pace of mechanic|cap / slow it: lower frequency, drop escalation, shrink audience, exclude minors|leaving size + pace unchanged|
|Harm real + by-design product of mechanic, or hits most vulnerable group hardest|rework what mechanic counts, or withdraw it|changing only mechanic's wording|
|Harm concentrates among heaviest users while aggregate metric improves|aggregate invalid for this decision; act on affected segment|citing aggregate gain|
|Growth + counter-metric move together|counter-metric wins until cause understood (per written agreement)|reopening ordering over chart|

## Output
- Pairing table per feature: growth metric, user-goal metric, counter-metrics.
- Abuse tracking: moderation error rates both ways + periodic safety survey.
- Per counter-metric: trip value + attached action, set pre-launch.
- Named person w/ authority to act.
- Written precedence rule: growth metric + counter-metric move together → counter-metric over growth metric until cause understood.

## Pitfalls
|Symptom|Likely cause|Fix|
|---|---|---|
|Counter-metric on dashboard, nobody acts when it moves|no agreed trip value / action / owner|set all three before launch|
|Debate restarts at each harm signal|no written precedence, no empowered owner|step 4 + step 5|
|Aggregate healthy while harm clusters among heaviest users|harm concentrated in segment|read segment; aggregate invalid for this call|
|Harm "fixed" by new copy|wording change used for design-driven harm|rework count / withdraw|

## Hypothetical example
- Hypothetical: language-learning app pairs "daily active learners" w/ "lessons a learner says helped" + counter-metrics late-night catch-up sessions + paid streak freezes. Pre-launch: trip values, actions + named owner written down. During staged release, freeze purchases move in one age group, cause unknown → owner holds release at current stage + sets investigation deadline.

## Related
- measure-what-you-value.md: metrics reflecting value to people; baselines, headcounts + segments.
- goals-signals-metrics.md: person's goal → observable signals → user-goal metric.
- engagement-vs-empowerment-metrics.md: capture metrics vs benefit metrics.
- [Reading product experiments honestly](reading-experiments-honestly.md): test mechanic's counter-metric w/ same rigour as its win.
- process-safeguards.md: staged rollout w/ withdrawal condition written first.
- [Habit, progress and gamification mechanics](../patterns/habits-streaks-and-gamification.md): streaks + counters = mechanics behind pairing table's habit + streak rows.
- ../ethics/ethics-review-workflow.md: counter-metrics dashboard w/ tripped thresholds + actions sits in its post-launch stage.
- activation-moment.md: usability side; activation metric also to pair w/ harm it could hide.
