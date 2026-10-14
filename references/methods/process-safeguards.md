# Process safeguards

## Use when
- Support refunds people over subscription, add-on / exit flow.
- Harm comes from every product in category competing same way.
- Anything review called risky, about to ship.
- What these cover shows up as product decision, not meeting.
- Assumes instruments w/ own method files: foresight exercises (second-order thinking, futures wheel, premortem, misuse-case brainstorming, four quadrants of design responsibility), should-we gate (three-gate check), metric pairings (counter-metrics), rules for reading test honestly (reading experiments honestly).

## The three safeguards
|Safeguard|Trigger|Serves mainly|Also|
|---|---|---|---|
|Fix the flow, not the complainer|refunds for unwanted subscriptions / add-ons / unfindable exits|Transparent|Intentional|
|Change the floor|harm from every product in category doing same rational thing|Intentional|Resilient|
|Stage the rollout, withdrawal condition written first|shipping anything review called risky|Intentional|Resilient|

Together they serve Transparent, Intentional + Resilient principles.

### Fix the flow, not the complainer
- When: support refunds people saying they never meant to subscribe, never chose add-on, or could not find way out.
- Do: read every such refund ticket as report on specific screen; count tickets by screen; show count beside screen's revenue.
- Do: estimate affected people not complaining before sizing flow problem.
- Avoid: settling w/ whoever complained while flow ships unchanged.
- Avoid: answering complaint by explaining where disclosure sat hidden, instead of moving it.
- Why: those noticing + pursuing refund = small, articulate fraction of those affected. Settling w/ complainers = cheaper path → such flows survive for years.
- Hypothetical: gym-membership app's support team tags each "did not mean to renew" refund w/ its source renewal screen; each month screen's owner sees tally next to screen's revenue, + one named person must close tickets by changing screen.

### Change the floor when harm comes from competition
- When: damage produced by every product in category individually doing same rational thing.
- Do: say plainly one product's restraint alone loses person + fixes nothing.
- Do: publish safeguard + how it works, so rivals copy it.
- Do: make detection + alerts work across competing products, not only your own.
- Do: give authority managing consequence the data it needs.
- Do: back standard / rule binding everyone, your own product included.
- Avoid: unilateral concession costing customer + changing no outcome.
- Avoid: its twin, shrug claiming nothing can be done because rivals will not follow.
- Hypothetical (competition harm): every pay-later checkout competes on fewest approval steps while household debt across all of them builds unseen.
- Hypothetical (competition harm): home-camera makers race on how far cameras see while ways for neighbours to detect covert recording lag behind.
- Hypothetical (changing floor): best-known smart-lock maker publishes how its alert tells every co-resident when new digital key added; shoppers come to expect it from every lock on shelf.

### Stage the rollout, withdrawal condition first
- When: shipping anything review called risky, e.g. new habit mechanic, ranking change, anything minors reach.
- Do: release to small share of people first.
- Do: keep comparable group never receiving feature → separates its effects from seasonality + season-long trends.
- Do: read counter-metrics by segment, not in aggregate.
- Do: agree in writing before launch what numbers / reports pause, cap or remove feature, + who may make this call w/o reopening argument.
- Avoid: full launch w/ monitoring promised for afterwards.
- Avoid: kill switch nobody has authority to pull.
- Avoid: rollout whose next stage happens automatically.
- Hypothetical: homework app's new daily-practice reminder goes first to small share of classes; comparable classes never get it; counter-metrics read per age group; written pause trigger + person allowed to pull it set before first class sees it.

## Pitfalls
|Symptom|Likely cause|Fix|
|---|---|---|
|Same refund reason recurs for years|complainers settled, flow unchanged|count tickets by screen beside revenue; change screen|
|Problem sized from complaints alone|people w/o complaints not estimated|estimate them first|
|One product's restraint, no change in outcome|unilateral concession|publish, share detection, back binding standard|
|"Rivals won't follow, so nothing to do"|shrug|change floor for everyone|
|Harm found after full launch|no staged release / holdout|small share first + never-exposed group|
|Kill switch exists, nobody pulls it|no named authority|name who may call it, in writing|

## Related
- ../principles/transparent.md: main principle for fixing flow.
- ../principles/intentional.md: main principle for changing floor + staged rollout; also served by fixing flow.
- ../principles/resilient.md: also served by changing floor + staged rollout.
- second-order-thinking.md: assumed foresight exercise.
- futures-wheel.md: assumed foresight exercise.
- premortem.md: assumed foresight exercise.
- misuse-case-brainstorming.md: assumed foresight exercise.
- [Four quadrants of design responsibility](four-quadrants-of-responsibility.md): assumed foresight exercise.
- three-gate-check.md: assumed should-we gate.
- counter-metrics.md: assumed metric pairings.
- [Reading product experiments honestly](reading-experiments-honestly.md): assumed rules for reading test honestly.
- ../ethics/ethics-review-workflow.md: ethics review steps before launch; its Monitor step holds staged rollout w/ holdout group + written withdrawal trigger.
- ../ethics/deceptive-patterns.md: check flagged screen against its named deceptive patterns, each w/ honest alternative.
- ../patterns/defaults-and-choice-architecture.md: opt-in, equal-weight decline + symmetric exit for flows refund tickets point at.
- [Business consequences of deceptive design](../evidence/business-cost-of-deception.md): fines, refunds, churn + trust loss to set beside screen's revenue.
- ../patterns/safety-and-abuse-resistance.md: safeguards for dual-use products, vulnerable people + children.
- ../patterns/departing-from-convention.md: usability side of rolling out redesign.
- [Turning a behavioral insight into a tested change](behavioral-insight-to-tested-change.md): usability-side method; tests before rollout.
- [Team and personal practices for humane design](team-and-personal-practices.md): habits keeping team able to make these calls.
