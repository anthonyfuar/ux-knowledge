# Progress, goals and task completion

## Scope
- Carrying people through multi-step tasks, programs + goals: plain progress, honest head starts, near sub-goals, info kept alive between steps, closing open loops, task duration.
- Open when designing/reviewing progress indicators, reward programs, setup checklists, profile-completion meters, any multi-step flow/long task.

## Laws behind these patterns
|Law|Role here|
|---|---|
|../laws/goal-gradient-effect.md|speed-up near end; head starts; near sub-goals|
|../laws/zeigarnik-effect.md|open loops, unfinished tasks|
|../laws/parkinsons-law.md|task duration vs expectation|
|../laws/doherty-threshold.md|one law behind progress patterns|
|../laws/flow.md|long tasks: challenge between frustration + boredom|

### Show progress or leave it implicit?
- When: multi-step tasks, profiles, programs.
- Do: show progress plainly → pushes completion.
- Why: people speed up nearing goal's end (Goal-Gradient Effect).
- Origin: goal-gradient hypothesis proposed 1932. 1934 experiments: rats in straight alley sped up nearing food. Decades after, evidence mainly animal. 2006 human field evidence: loyalty-card customers bought faster nearing free reward.
- Limit: speed-up only for real, reachable rewards.
- Hypothetical: after each session, physiotherapy app home screen shows how many sessions of prescribed plan done + how many remain.

### Grant a head start?
- When: reward programs, setup checklists, profile-completion meters.
- Do: give some initial progress as share of whole → remaining distance looks small. Credit only work really done (account creation, sign-in) / genuine gift. Show finish line + name next step.
- Avoid: fake progress; inflated totals; quietly raising threshold by bonus size.
- Why: artificial progress still motivates.
- Caveat: head start may only reframe work fixed anyway.
- Evidence:

|Finding|Study (year, kind)|Design consequence|
|---|---|---|
|Both need 8 paid washes: 10-stamp card w/ 2 pre-filled → 34% of customers redeemed vs 19% w/ blank 8-stamp card|2006 car-wash field experiment|same paid washes, pre-filled start → higher redemption|
|12-stamp card w/ 2 free stamps likewise beat plain 10-stamp card|same car-wash research|head start beat plain card again|

- Hypothetical: home-insurance setup checklist opens w/ "account created" + "identity verified" ticked (person just did both), names next step "add property details", shows where list ends.

### One distant goal or near sub-goals?
- When: long journeys, programs, goals where people drift.
- Do: split into near sub-goals: short cycles, frequent visible rewards (e.g. 25 pages/day, not 52 books this year). Place near milestone where users drift. Bridge reset: goal reached → show next, ideally partly done already → post-reward slump does not become exit point. Let users adjust goal difficulty.
- Avoid: one distant reward (too far → no acceleration toward it); finish lines moved to serve business over user's goals.
- Why: goals pull hard only near end.
- Hypothetical: language-certification course: syllabus in units, badge each; unit done → next appears w/ first lesson marked done (closing quiz covered it); learner can switch unit pace lighter/heavier.

### Information seen in one step, needed in a later one?
- When: info from one step (code, price, instruction) needed later.
- Do: carry it forward on screen (e.g. sticky summary/step recap). Multi-step instructions: one step at a time, persistently visible.
- Avoid: interstitials, promotional modals, detours between seeing info + using it.
- Why: 15-30 seconds of unrelated activity erase what users held in mind.
- Hypothetical: passport-renewal flow pins step-1 reference number in summary bar until payment step asks for it; no offer screens between.

### How do unfinished items get closed?
- When: unfinished tasks, drafts, X-of-Y-done counters, interrupted work.
- Do: let users close open loops: every unfinished task, draft/X-of-Y-done counter gets clear, reachable finish. Open items archivable/dismissible. Offer resume-where-you-left-off for interrupted work (Ovsiankina effect).
- Avoid: permanent nag meters, cliffhangers, teaser subject lines forcing return.
- Why: Zeigarnik Effect (open loops); never-closing loops → rumination + clutter.
- Hypothetical: project tool: person marks abandoned draft "won't do" → leaves open counter; interrupted data import reopens at row where it stopped.

### How long should the task take?
- When: sizing task length.
- Do: keep task time within expected duration, ideally under (Parkinson's Law). Offer time-saving features. Signal clearly when more content follows. Long tasks: keep challenge between frustration + boredom (Flow).
- Hypothetical: year-end payroll wizard states remaining sections upfront, pre-fills unchanged employee details, marks "more below" where section continues past fold.

## Related
- habits-streaks-and-gamification.md: humane bounds on streaks, counters + rewards; effect on vulnerable people.
- feedback-loading-and-performance.md: progress bars tied to real work, waits, response-time budgets.
- onboarding-and-first-use.md: setup checklists, activation, re-engagement nudges.
- forms-and-data-entry.md: multi-step forms + checkout showing progress.
- feeds-scrolling-and-pacing.md: stopping points; open loops + moving finish lines turning into capture.
- ../ethics/using-psychology-responsibly.md: guardrails for goal-gradient + open-loop levers.
- ../principles/finite.md: bounds never-closing loops + moved finish lines.
- ../methods/measuring-flow.md: checks challenge-skill match in long tasks.
- ../laws/goal-gradient-effect.md: law behind progress display + head starts.
- ../laws/zeigarnik-effect.md: law behind open loops.
