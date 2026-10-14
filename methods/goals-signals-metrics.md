# Goals, signals, metrics

## Use when
- Deriving feature metrics from what people want from it: goal in their own words → observable signal → number.

## Key terms
|Term|Meaning|
|---|---|
|Goal|what person wants, in their own words|
|Signal|observable behaviour / attitude|
|Metric|number computed from signal|
|HEART-style framework|source this method adapts; letters = happiness, engagement, adoption, retention, task success|

## Steps
1. **Write goal** in person's words. When adapting HEART-style framework, translate its "happiness" category into person's own objectives.
2. **Pick signal**: observable behaviour / attitude.
3. **Compute metric** from signal.
- Order rule: goals before signals, signals before metrics; never reverse.
- Metric w/ no goal behind it = habit, not measure.

## Worked rows
|Goal (person's words)|Signal|Metric|Surface|
|---|---|---|---|
|Catch up on friends quickly + get on w/ day|sessions end at caught-up marker|share of sessions ending within 2 min of reaching "all caught up" marker|stopping points in feeds|
|Get interrupted only when it matters|notifications acted on vs dismissed|actioned-to-dismissed ratio by category; categories people snooze|notifications|
|Know what app knows about me|data-page visits; exports; deletions completed|time to complete deletion; share finding data page unaided|—|
|Keep up practice in way fitting my life|returns after gap w/o getting chased; progress screen opened by choice|return rate after missed day; share of sessions reaching benefit person stated; share hiding / resetting counter|streaks + counters|
|Feel safe here|blocks; reports resolved; appeals|report time-to-acknowledge; safety survey score by segment|—|
|Have chosen this myself, not had it chosen for me|algorithm controls used; unpersonalized view opened|share of active people having adjusted ranking|steering controls|

## Decision rules
- If metric proposed first → ask which goal it serves + which signal it counts; no goal → habit, not measure → back to step 1.
- If goal not in person's own words → rewrite before choosing signals.
- If category = "happiness" → translate into person's own objectives.

## Output
- Per feature: goal → signal → metric rows, in this order; each metric traceable to person's goal.

## Hypothetical example
- Hypothetical: pension-savings app. Goal: "know whether I am on track to retire when I planned." Signal: people open projection screen, adjust contribution, then leave. Metric: share of projection visits ending w/ saved change / confirmed "on track" view.

## Related
- counter-metrics.md: pairs each growth metric w/ user-goal metric + harm it could hide.
- measure-what-you-value.md: choosing metrics reflecting value to people.
- engagement-vs-empowerment-metrics.md: asks of every number: would person recognize it as own goal?
- activation-moment.md: usability side; locates first real success + measures path to it.
- [Feeds, scrolling and content pacing](../patterns/feeds-scrolling-and-pacing.md): stopping points = catching-up row's surface.
- ../patterns/notifications-and-interruptions.md: what interrupts, when, under whose control = interrupted-only-when-it-matters row's surface.
- [Habit, progress and gamification mechanics](../patterns/habits-streaks-and-gamification.md): streaks + counters = keeping-up-practice row's surface.
- [Recommendations, ranking and personalization](../patterns/recommendations-and-personalization.md): steering controls = chosen-not-chosen-for-me row's surface.
