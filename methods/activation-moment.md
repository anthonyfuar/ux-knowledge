# Activation moment (time to value)

## Use when
- Locate product's first real success = activation / aha action; measure new users' path to it.
- Time to value = new user's time to reach activation action.

## Steps
1. **Define retention first.** Fix "retained" for this product before viewing any early behaviour.
2. **List candidate early actions** plausibly delivering core value. Each = count + time window: N items within D days after sign-up.
3. **Compare cohorts.** Per candidate: retention of new-user cohorts reaching it vs not.
4. **Test causation.** Step 3 = correlation only → experiment: action made easier for random half of new users (template / shortcut / nudge). Pass = retention rises; action-rate rise alone does not pass.
5. **Measure time to action** per cohort: median + spread + never-reach share → cut steps before action (shorter path).
6. **Recheck** activation action after major product changes.

## Decision rules
- If choosing among candidates → pick action reached by most retained + few churned users; avoid picking action merely for biggest retention gap between cohorts.
- If cohort gap looks convincing → still not cause; motivated users do more of everything, so reaching action may not drive retention → step 4.
- If experiment lifts action rate but retention does not rise → causation not shown; pass = retention.
- If setting time-to-value target → derive from product's own baseline; avoid borrowed universal "within N minutes" figure.
- If product / its audience changed substantially → expect aha action drift → recheck (step 6).

## Output
- One activation action (count + window), chosen by retained vs churned reach pattern.
- Experiment result read on retention.
- Time to action per cohort: median, spread, never-reach share; list of pre-action steps removed.
- Paired counter-metric for harm activation metric could hide (see Related).

## Pitfalls
|Symptom|Likely cause|Fix|
|---|---|---|
|Activation action chosen; retention unmoved after push|picked biggest gap / read correlation as cause|choose by retained vs churned reach; confirm w/ randomized test|
|Test called win on action rate|wrong pass condition|judge on retention|
|Target copied from elsewhere|no own baseline|measure own median + spread first|
|Old aha action still tracked long after launch|drift after product / audience change|recheck after each major change|

## Hypothetical examples
- Hypothetical: library e-lending app fixes retained = borrows again in later month; written down before anyone opens first-week click data.
- Hypothetical: same app's candidates = first hold placed, first reading list saved, family member's card linked.
- Hypothetical: one candidate as count + window = borrows N titles within D days after sign-up.

## Related
- ../patterns/onboarding-and-first-use.md: patterns on activation + time-to-first-value targets.
- teaching-inside-the-task.md: first use designed for early first real success.
- [Turning a behavioral insight into a tested change](behavioral-insight-to-tested-change.md): workflow around step 4 experiment.
- [Reading product experiments honestly](reading-experiments-honestly.md): reading activation experiment w/o fooling team.
- counter-metrics.md: pair activation metric w/ metric for harm it could hide.
- engagement-vs-empowerment-metrics.md: habit-loop retention vs returns because product helped.
- goals-signals-metrics.md: goals → observable signals → metrics.
