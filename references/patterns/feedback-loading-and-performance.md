# Feedback, loading and perceived performance

## Scope + laws behind these patterns
- Use for: usability patterns, system response + waiting: indicator by expected wait · response-time budgets · perceived speed · progress bars · layout stability · touch timeouts · announcing changes · protecting flow · auto-advance in work queues.
- Applies when: designing/reviewing action feedback, loading states, slow operations, or interface feeling slow, jumpy or silent.
- Laws underneath:
  - ../laws/doherty-threshold.md: system response within 400 ms.
  - ../laws/flow.md: removing friction, protecting deep work, natural stopping points.
  - ../laws/selective-attention.md: announcing changes so none get missed.
  - ../laws/peak-end-rule.md: progress bars not stalling at end.
  - ../laws/goal-gradient-effect.md: sense of steady progress during waits.

### Which indicator fits the expected wait?
- When: any action w/ wait. Thresholds from 1982 system-response-time work + 1968 conversational-computing response-time work.

|Expected wait|Do|Avoid|
|---|---|---|
|Under 0.1 s|Direct-manipulation feedback: pressed state, keystroke echo, drag following pointer. Matches first classic response-time limit + 1968 work|No feedback at all|
|Under 0.4 s|System's response itself where possible, no indicator (Doherty Threshold)|Any indicator|
|About 0.4–2 s|Old content stays on screen + small inline activity cue|Briefly flashing spinner|
|Over about 2 s, layout known|Skeleton matching final layout; also prevents layout shift|Skeleton shaped unlike replacing content: same jump as no placeholder|
|Over about 2 s, duration estimable|Determinate progress bar driven by real work|Bar on timer|
|Over about 15 s|Work to background, free user + notify on completion|User left waiting in foreground|

- If structured first load → skeleton.
- If refresh → stale data stays visible w/ inline cue + "last updated" time; not skeleton, not spinner.
- If short wait + result has no known shape → spinner; only then.
- Hypothetical: pharmacy stock checker: first load = card skeletons shaped like result cards; pull-to-refresh keeps old stock levels w/ small cue + "last updated" stamp.

### Which response-time number is which?

|Number|Meaning|
|---|---|
|0.1 s|First of three classic response-time limits: response feels instantaneous; for direct-manipulation feedback|
|1 s|Classic limit: user's flow of thought stays uninterrupted|
|10 s|Classic limit: attention stays on task|
|400 ms|Doherty Threshold; system response|

- Origin: three classic limits build on 1968 response-time work + later research on human perceptual cycle. 1982 IBM work cut target system response time from 2,000 ms to 400 ms.
- Misreading: Wrong: pressed states + keystroke echo justified by Doherty Threshold → Right: attribute them to 0.1 s limit.

### Response-time budget: one target or one per interaction class?
- When: setting performance targets.
- Do:
  - 400 ms = ceiling for replying to any action expecting response; under it → people stay focused + productive.
  - Feedback confirms both result + causing action.
  - Separate budget per interaction class: control feedback · typed echo · conversational reply · page turn · job run · background execution.
  - One response carries several messages (heard, accepted, working) → meet deadline of most time-critical one.
  - Unavoidable waits over ~2 s → at closure points, right after felt completion (finished step, submitted form). Bigger completions tolerate longer waits.
  - Beyond ~15 s → work to background, free user, notify on completion.
  - Complex results → progressively: complex graphic starts within 2 s, complete within 10 s.
  - Multi-part answers → one part every 2–4 s (1968 response-time work).
  - Durations consistent for repeated actions.

|Interaction class|Budget|
|---|---|
|Control acknowledgement|≤0.1 s|
|Keystroke echo|0.1–0.2 s|
|Routine request acknowledged|≤2 s|
|First lines of next page appear|≤1 s|

- Avoid: one blanket target, e.g. "2 seconds", for all interactions; stalls mid-thought or between sequence steps; blank screen until everything ready.
- Why: missing feedback breaks flow. Beyond ~15 s conversational interaction lost + busy users grow demoralised (1968 response-time work). At ~2–4 s waits people notice duration changes of roughly 8% → larger jitter reads as unreliable.
- Hypothetical: tax-filing portal: field validation echoes instantly; "submit return" acknowledges at once, calculation runs after submission (closure point); full assessment comes by notification.

### Work genuinely takes time: how to make the wait easier?
- When: work genuinely takes time + real speed impossible.
- Do: progress bar + something animated for eye to follow through wait.
- Why: even imprecise progress bar lightens wait.
- Case: Uber Express POOL wait screen (2019 behavioural science work) used three levers:
  1. Goal-gradient: every step explained → sense of steady progress.
  2. Operational transparency: arrival estimate shown w/ method behind it.
  3. Idleness aversion: animation w/ both entertainment + information value.
  - 2019 A/B experiment: redesigned screen cut post-request cancellations by 11%.
- Hypothetical: passport-renewal portal lists each stage passed (received, checked, printing) + explains method behind delivery estimate, not static "processing".

### Progress bar: what drives it + how is it shown?
- When: showing progress on wait.
- Do:
  - Percent-done bar driven by actual progress → doubles as heartbeat: stops if process hangs.
  - Graphic indicator over number unless precision needed.
  - Multi-pass operations → one progress segment per pass.
  - Nested operations → progress of current step + whole task.
  - Time remaining shown when system can estimate it.
  - Indicator placed where user looks.
  - Indeterminate indicator only when system truly cannot estimate duration: shows system alive, no help planning.
- Avoid: timer-driven bar independent of work: hides failures. Bars racing early + stalling near 100%: worst moment last (Peak-End Rule).
- Evidence: 2007 study: same process, fixed-length bar accelerating near end feels faster than constant-speed one.
- Hypothetical: hospital imaging upload: one segment per pass (compress, encrypt, transfer), bar for current file + one for whole study, beside file list clinician watches.

### Late-arriving content: how to keep layout stable?
- When: images, fonts, ads or other content arrive after first paint.
- Do: reserve space for late content; inline critical above-the-fold styles; move decorative layers w/ transforms, not layout offsets; layout-stability metric (e.g. cumulative layout shift) in performance budget.
- Symptom → cause: interactive target moving under pointer as page settles → breaks reading focus + causes mis-clicks.
- Why: fast but jumpy page still feels unreliable.
- Limits: performance audit scores = proxies; perfect score does not prove users on slow networks find page fast. Absolute positioning alone does not stop element counting toward layout shift.
- Hypothetical: hotel booking page reserves photo frame + price box before load → "book" button stays under guest's thumb.

### Touch: how long do transient controls stay?
- When: touch interfaces w/ video controls, toasts or time-limited buttons.
- Do: persistent, or long timeouts.
- Avoid: disappearing controls tuned for focused mouse user.
- Why: touch users often relaxed/distracted + re-engage from disengaged posture. Evidence: temporal pointing (2016 research): target available only within time window gets harder to hit as window shrinks.
- Hypothetical: recipe app on kitchen tablet keeps "undo" toast + timer controls on screen until cook dismisses them.

### Operation so fast people doubt it: hold the result back?
- When: operation so fast users doubt it did anything valuable.
- Do: where work genuinely ends sooner but result's trust + perceived value can gain from waiting → hold result back on purpose.
- Avoid: deceptive deliberate delay (guardrails: ../ethics/using-psychology-responsibly.md).
- Hypothetical: insurance claim checker finishes instantly but shows checked documents one by one before verdict, each genuinely checked.

### Interface changes state or content: how to announce it?
- When: interface changes state or content.
- Do:
  - Each meaningful change gets cue too strong to miss.
  - Check if other changes land at same moment + pull attention from meaningful one.
  - New UI (panel, search box, menu, error) beside element person acted on.
  - Announce w/ one animation + dim unchanged parts.
  - Floating elements near focus of attention in contrasting colour, e.g. back-to-top button low on screen.
- Avoid: simultaneous changes elsewhere; competing animations; moving background behind change.
- Why: Selective Attention: weak cues → change blindness.
- Hypothetical: clinic booking app: tapping date opens chosen day's free slots right under it w/ one slide-in; rest of calendar dims.
- Hypothetical: loan application: failed submit shows each error next to faulty field, w/o rotating promo banner running at same moment.

### Deep work: how to protect flow?
- When: tuning core loop, or users in deep work (writing, editing, triage, analysis).
- Do: features + content findable; strip purposeless friction; system quick. During deep work suppress modal promos, non-urgent notifications + forced context switches. Hide interface chrome once work starts.
- Why: Flow: findability, no purposeless friction + speed: all three together keep people engaged.
- Trade-off: removing context (e.g. hiding inbox inside conversation) aids focus but can hurt users needing overview → decide per task.
- Hypothetical: radiology viewer: once reading session starts, worklist sidebar + announcement banner collapse; non-urgent messages wait until report signed.

### Work queue: open the next item automatically?
- When: users process queue: messages, reviews, ratings, tasks.
- Do: item completed/archived → open next one; user never has to decide what comes next. One action per step leads straight into similar items.
- Avoid: returning to hub after every action: fresh decision each time (decision fatigue).
- Limits:
  - Auto-advance only in work queues user started (triage, review, rating), always w/ visible "done for now" or stop control.
  - Consumption feeds (video, stories, articles) get no default auto-advance; they end on natural stopping point (Flow; Zeigarnik Effect) → see feeds-scrolling-and-pacing.md.
- Hypothetical: expense-approval tool opens next pending claim after "approve", "done for now" button always in view.
- Hypothetical: home-inspection app: closing one checklist item opens next item in same room w/ same pass/fail action + stop control.

## Related
- ../methods/thresholds-and-formulas.md: measurable response-time limits.
- progress-goals-and-completion.md: progress indicators, head starts, multi-step completion.
- dashboards-and-data-displays.md: skeleton tiles, refresh, per-tile loading on dense data screens.
- memorable-moments-and-endings.md: designing peaks, endings + failure moments, incl. end of wait.
- ../ethics/using-psychology-responsibly.md: guardrails on deliberate delays + perceived-speed techniques.
- feeds-scrolling-and-pacing.md: stopping points + autoplay; humane bound on auto-advance.
- notifications-and-interruptions.md: what may interrupt + when; notify-on-completion, suppressed non-urgent notifications.
- calm-technology-and-device-etiquette.md: peripheral attention + quiet signalling; bounds how loudly to announce changes.
- ../laws/doherty-threshold.md: system response within 400 ms.
- ../laws/flow.md: friction, deep work, stopping points.
- ../laws/selective-attention.md: change blindness.
- ../laws/peak-end-rule.md: no stall at bar's end.
- ../laws/goal-gradient-effect.md: steady progress during waits.
- ../laws/zeigarnik-effect.md: why consumption feeds end on stopping point.
