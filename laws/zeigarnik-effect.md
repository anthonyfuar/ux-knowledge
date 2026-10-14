# Zeigarnik Effect

## In one line
Memory favors interrupted or unfinished tasks: completed task recalled worse than one broken off or left open. Design takeaway only (original study measured recall only): signal more content exists + show progress clearly. Matters most for progress indicators, more-content signifiers + head starts from real completed steps.

- Class: effect or principle; no aliases. Theme: Attention.

## Applies when / does not apply when
|Applies when|Does not apply when → cite instead|
|---|---|
|progress + further content clearly signaled (only condition where it works in design)|progress or continuation hidden|
|checklist user started, then left|pre-credited checklist step / head start → endowed progress, goal-gradient-effect.md|
|recall of started-and-interrupted task|urge to resume interrupted tasks + "resume where you left off" features → Ovsiankina effect|
|design uses, read as extrapolation from 1927 doctoral thesis|claims of proven design effect|

## Which effect to cite
|Situation|Cite|Mechanism|
|---|---|---|
|Users remember unfinished draft or open task|Zeigarnik Effect|memory for task started + interrupted|
|Users feel pulled to resume interrupted task; resume features|Ovsiankina effect|urge to resume interrupted tasks|
|Step pre-credited as done / head start|Goal-Gradient Effect (endowed progress)|perceived nearness to reward raises effort|
|Near goal people return more, then leave right after completing|goal-gradient data + released tension|unfinished goal near completion keeps pulling; completion releases tension|

Related to, but distinct from, endowed progress effect + goal-gradient hypothesis: those raise effort via perceived nearness to reward; this effect = memory for task started + interrupted. Cite each only for own mechanism.

## Decision rules
Signal + show
- Signal plainly: more content exists → people go looking.
- Make progress plain → people push on to finish.

Resume + close
- Make started-then-left tasks easy to resume: show unfinished work clearly (saved drafts, continue where you left off).
- Close loops explicitly: confirm completion.
- Always offer clear way to finish, archive or dismiss open item.

Head starts
- Grant head start only from real completed steps or genuine gift toward goal.
- Never inflate total; never add nonexistent steps.

Sending users back
- If flow must send users back (to fix earlier field, rerun setup) → frame as forward progress + keep all completed work.

Next goal
- Tie next goal to real value; never manufacture incomplete tasks or endless loops to pull people back (engagement dark pattern).

## Why it works
1. Pull toward closure: open task grips memory, pulls toward closure; visible incompleteness or more-content signs harness this tension.
2. Field theory: starting task creates task-specific tension keeping related details accessible; finishing releases it; interruption keeps it alive.
3. Intrusive reminder: open loop = intrusive reminder of unfinished goal while attention elsewhere.
4. Rehearsal cost: several open items cost continuous rehearsal effort (see cognitive-load.md).
5. Doubling-back aversion: reluctance to retrace steps or restart (feels like undoing progress), even when going back saves effort. If going back not framed as progress → people push on w/ worse path to avoid "going back".

Origin
|When|What appeared or was shown|
|---|---|
|1920s (dated 1927)|memory study behind effect: doctoral thesis in Berlin within field theory (degree 1927)|
|—|research began from, + commonly illustrated by, waiter recalling unpaid orders in detail, forgetting them once settled|
|1935|further early work on memory benefit of interrupted tasks|

## Evidence
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Incomplete tasks recalled more readily than completed ones|1920s experimental memory study (1927 doctoral thesis)|design uses = extrapolation; replication record mixed; rests on early work (1927, 1935); quote no sample size|signal more content + show progress, as takeaway only|
|Unfinished goal near completion keeps pulling people back (more visits, longer sessions); completion releases tension → exits peak right then|goal-gradient data|link to Goal-Gradient Effect|show next goal right after completion|
|Largest share of session endings came right after reward earned; endings rarer as next goal neared|2006 online rating program|—|show next goal right after completion|

Do not quote sample size for studies behind Zeigarnik Effect or Von Restorff Effect.

## Misreadings and limits
- Wrong: pre-credited checklist head start works by Zeigarnik Effect. → Right: head start from real completed steps = endowed progress, via perceived nearness (Goal-Gradient); Zeigarnik Effect fits checklist started + left.
- Wrong: Zeigarnik Effect proves head start raises motivation to finish. → Right: design takeaway only; study measured recall, + head start = endowed progress (Goal-Gradient).
- Wrong: Zeigarnik Effect = urge to resume. → Right: Zeigarnik Effect = memory for unfinished tasks; Ovsiankina effect = urge to resume them + basis of "resume where you left off" features.
- Wrong: completion meters or cliffhangers w/ no way to close them. → Right: open loops cost rehearsal effort + cause rumination → allow finish, dismiss + resume.
- Limit: works in design only when progress + further content clearly signaled.
- Limit: evidence = 1927 doctoral thesis; design uses = extrapolation; replication record mixed.

Costs of open loops
- Unfinished goal consumes attention, causes stress.
- Unclosed loops → rumination + cognitive clutter.
- Cliffhangers, autoplay + completion meters can become compulsion loops.
- Inflated progress = ethically sensitive lever.

## Check questions
- [A] (Zeigarnik Effect): unfinished tasks + "more content" clearly signaled? Look for hidden continuation + no progress indicator on multi-step tasks.
- [A] (Zeigarnik Effect): can users finish, dismiss or resume every open loop? Look for permanent completion nags, cliffhanger teasers + no "resume" for interrupted work.
- [A] (Goal-Gradient Effect, Zeigarnik Effect): next goal shown right after completion? Look for dead-end success screens where users drop off.

## Symptoms → fixes
|Symptom|Laws|Fix|
|---|---|---|
|Multi-step flow abandoned midway|Goal-Gradient Effect, Zeigarnik Effect (as design takeaways)|step counter or progress bar + small, truthful head start; confirm cause w/ per-step drop-off, do not assume it|
|Users drop off on dead-end success screen|Goal-Gradient Effect, Zeigarnik Effect|show next goal right after completion, tied to real value|
|Users push on w/ worse path rather than go back to fix something|doubling-back aversion|frame going back as forward progress; keep all completed work|
|Open items nag forever|open loops w/o closure|offer finish, archive or dismiss; confirm completion|

## Hypothetical examples
- Hypothetical: home-insurance claim flow opens w/ "policy verified" + "photos uploaded" pre-ticked because customer did both earlier; head start only from real completed steps.
- Hypothetical: recipe app lets next step card peek in from screen edge, shows step counter, starts w/ "ingredients gathered" ticked only if cook already checked off every in-app shopping-list item: visible continuation, progress indicator + head start from real completed step.

## Humane bound
Bounded by ../principles/finite.md + ../principles/intentional.md principles.

Turned against people
- Cliffhangers, autoplay + ellipsis teasers driving compulsive return.
- Permanent nag meters, completion meters becoming compulsion loops, inflated progress.
- Named dark patterns built on open loops: bottomless bowl + autoplay; bottomless feed.
- Manufacturing incomplete tasks or endless loops to pull people back = engagement dark pattern → instead tie next goal to real value.

Further reading: [Feeds, scrolling and content pacing](../patterns/feeds-scrolling-and-pacing.md); [Progress, goals and task completion](../patterns/progress-goals-and-completion.md) (its entry on letting users close open loops); [Habit, progress and gamification mechanics](../patterns/habits-streaks-and-gamification.md); ../evidence/addiction-and-variable-rewards.md.

## Related
- goal-gradient-effect.md: endowed progress + perceived nearness = mechanism to cite for head start; shares next-goal question + abandoned-flow fix.
- cognitive-load.md: open loops occupy capacity.
- peak-end-rule.md: closing episode well.
- [Usability heuristics mapped to laws](../checklists/usability-heuristics-map.md): "Visibility of system status" relates to Doherty Threshold, Goal-Gradient Effect + Zeigarnik Effect; classic heuristics date from 1990, revised 1994.
- [Feeds, scrolling and content pacing](../patterns/feeds-scrolling-and-pacing.md): humane bounds on open loops (stopping points, autoplay, infinite scroll).
- [Habit, progress and gamification mechanics](../patterns/habits-streaks-and-gamification.md): humane bounds on completion meters, streaks + counters.
- ../evidence/addiction-and-variable-rewards.md: humane-design evidence on compulsion loops.
- ../guides/laws-and-principles-crosswalk.md: humane principle bounding Zeigarnik Effect.
- ../patterns/onboarding-and-first-use.md: patterns applying Zeigarnik Effect.
- [Progress, goals and task completion](../patterns/progress-goals-and-completion.md): patterns applying Zeigarnik Effect.
