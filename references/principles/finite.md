# Finite

## In one line
- Finite = experience has edges; quality of time over endless quantity.
- Rule: replace auto-refilling feeds, autoplay + variable rewards w/ explicit choices + natural stopping points.
- Open when: design/review touches feeds, scrolling, autoplay, variable rewards, session length, usage limits or sleep.

## Core practices
Highest weight; check first.
1. "All caught up" marker, not silent feed backfill.
2. Load More/pagination, not infinite scroll, where people search/compare.
3. "Up next" + deliberate tap, not autoplay.
4. Variable rewards turned into predictable, scheduled delivery.
5. Usage visible + backed by enforced limits.
6. Sleep protected by default.

## Commitments w/ a pattern entry
All entries in ../patterns/feeds-scrolling-and-pacing.md.

|Commitment|Do|Avoid|
|---|---|---|
|Stopping point|"all caught up" indicator; scroll position kept when person returns||
|Loading|"load more"|infinite scroll|
|Continuous loading|only for aimless browsing of homogeneous content||
|Feed access|feed traversable by keyboard + screen reader||
|Autoplay|"up next"; autoplay off by default + always off for minors|autoplay|
|Volume|a little meaningful content|volume|
|Rewards|predictable, scheduled delivery|variable rewards|
|Extended use|moderation prompt after extended use||
|Attention + sleep|protect both, especially w/ short-form media||

## Guidance held here (no pattern entry)

### Where does a session end?
- Do: define what finished means: daily edition, session length chosen on entry, or graceful hand-off once person's intention met.

### Showing usage + setting limits?
- Do: show time spent, pickups + session counts vs earlier periods.
- Do: back awareness w/ enforceable limits: timers genuinely pausing product; focus mode people can schedule.
- Wrong: banner dismissed w/ one tap = usage limit → Right: enforces nothing → no limit.
- Case: Apple's Screen Time + Google's Digital Wellbeing = built-in device usage tools, two parts: insight (personal use reports) + restraint (daily caps, temporary holds on attention-pulling apps, notification settings).
- Empowerment starts w/ device-level features, e.g. usage reports + limits.
- Caveat: unsettled whether knowing own usage alone suffices to change it.

### Icons, sounds + animation pulling people back?
- Do: mute saturated icons, sounds + surprise animation; offer grayscale mode.
- Do: red counters only for genuinely urgent items.
- Hypothetical: graduate student hides red badge counts on laptop dock + silences every app sound while writing = personal way to strip sensory lures.

### Does the job need a screen at all?
- Ask first. If not → complete it via ambient, glanceable, haptic or spoken routes (low-interface utility).
- Why: task done w/o opening app never creates moment where feed can capture session.
- Limit: screenless natural-language devices replace very little today → treat as direction of travel, not shipping answer.

### Tempted to build a hook?
- Avoid: streaks, reminders/schedules meant to make product pacemaker of someone's day.
- Do: protect people's off-hours.
- Rule: retention should come from help delivered, not people's inability to stop.

## Why it matters
- Engagement feedback loop: longer sessions → more data + ad views; sessions lengthen because each refines ranking filling next.
- Whole loop built to hold people, not benefit them.
- Critique of feeds: every stopping cue deliberately stripped out + stream made self-refilling.
- Infinite scroll removes pause brain needs to catch up w/ its impulses.

## Key concepts
|Term|Meaning|
|---|---|
|Random-reinforcement feedback loop|data improves targeting → targeting extends sessions → sessions yield more data + ad exposure|
|Three layers of distraction|distraction costs (1) task at hand, (2) longer life person meant to lead, (3) capacity to form + hold goals at all|
|Layer 3|held deepest harm, because reflection + self-regulation underpin goal-setting|
|Layer 1|only layer repaired by better timing|

- Rule: state finding's distraction layer. Alert costing ten minutes of focus not same severity as mechanic eroding someone's ability to keep own aims.

## Audit questions
Scope: bounded, high-quality time. All principles' questions → ../checklists/humane-design-audit.md.

|Check|Passes when|
|---|---|
|Visible "all caught up" state?|feed ends when new content ends; no silent recommendation backfill|
|Person-triggered Load More instead of continuous loading, or continuous loading justified for task?|infinite scroll only for aimless browsing of homogeneous content; paging for search, comparison + goal-directed lists|
|Autoplay replaced by "up next" card needing deliberate tap?|no countdown; autoplay off by default for minors|
|Moderation prompts after extended use?|"still watching?" check-ins, session-intent prompts + dashboards making time visible|
|Small amount of meaningful content over volume?|no padding to extend sessions|
|Can people see elapsed time, pause + set enforced limits?|timers pause app when they run out|
|Every reward predictable + scheduled, not variable payoff?|no pull-to-refresh jackpot; no withheld/unpredictable badge counts|

## Neighbours to check
- Check alongside: intentional.md, inclusive.md, resilient.md.
- Working w/ neighbours → [Principles index](index.md).

## Related
- ../patterns/feeds-scrolling-and-pacing.md: when/do/avoid entries for stopping points, infinite scroll, autoplay, variable rewards.
- ../patterns/habits-streaks-and-gamification.md: streaks, counters + rewards + their effect on vulnerable people.
- ../ethics/attention-hijacks.md: levers taking attention against person's interest + counter to each.
- ../evidence/addiction-and-variable-rewards.md: evidence on compulsion loops, variable rewards + time lost.
- ../methods/engagement-vs-empowerment-metrics.md: telling capture metrics from benefit metrics.
- ../ethics/influence-vs-manipulation.md: tests: does persuasive lever serve person or exploit them?
- ../laws/zeigarnik-effect.md: usability-side law on unfinished tasks + open loops.
- ../guides/laws-and-principles-crosswalk.md: psychological lever each principle guards + principle bounding each law.
- ../checklists/humane-design-audit.md: audit questions for all seven principles together.
- [Principles index](index.md): seven principles side by side + how to work w/ neighbours.
- Pattern files tagged Finite: ../patterns/ai-and-automated-features.md, ../patterns/recommendations-and-personalization.md, ../patterns/notifications-and-interruptions.md, ../patterns/feeds-scrolling-and-pacing.md, ../patterns/habits-streaks-and-gamification.md.
