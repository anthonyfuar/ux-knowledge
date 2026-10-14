# Doherty Threshold

## In one line
Every system reply < 400 ms (former norm: 2,000 ms) → no idle gaps on either side of human-machine exchange → output per unit time climbs steeply. Use for: response-time budgets; loading states, progress bars, other waits; weighing deliberate delay; checking whether this law fits timing in question.
- No aliases. Class: effect/principle.
- Theme: Motor + time. Most affects: response-time budget < 400 ms, loading animations + progress bars, perceived performance.
- Core rule: respond < 400 ms; slower work → skeleton, inline cue or real progress bar.
- Citation status: traces to 1982 IBM paper arguing for sub-second response. 400 ms = popular threshold attributed to it; 400 ms replacing 2,000 ms standard = likewise popular attribution → cite 400 ms as popular threshold attributed to 1982 paper, not its own finding.

## Applies when / does not apply when
|Timing question|Cite|Not|
|---|---|---|
|system response to request|Doherty Threshold: 400 ms|—|
|direct-manipulation feedback (pressed state, keystroke echo, drag)|own 0.1 s limit (1968 analysis); also first of widely cited three response-time limits (0.1 s, 1 s, 10 s)|not this law|
|1 s + 10 s limits|further, separate attention limits|not this law|
|1968 response-time levels (table below)|separate source, often filed under Doherty Threshold|not this law|
|preventing double submission (button disabled while request in flight, idempotent requests)|error prevention; error-prevention usability heuristic|not response-time matter; no timing law|
|payment/other processing wait at checkout|1968 levels set budget; 400 ms usually out of reach here → mitigate|—|

Only 400 ms system-response figure = Doherty Threshold.

## Decision rules

### Set the budget
- Response-time budget per interaction level, not one global target.
- Answering in ≤ 400 ms pays off: focus stays on task + more work done → acknowledge every input < 400 ms.
- If response > 400 ms → either speed it up or mitigate wait; spinner mitigates but does not meet threshold.
- If work slower → instant feedback first, then animation/progress bar. Respond < 400 ms; otherwise animation + progress indicators cut perceived wait.
- If trimming slow response → crossing threshold (under 0.1 s, 1 s, 2 s, ~15 s) changes experience; trimming 10 s to 7 s may buy nothing.
- If action repeats → keep response-time variation below what users can detect; for repeated actions consistency matters as much as speed.
- Latency budgets = cognitive budgets: slow system costs users twice: waiting + longer think time.
- If arguing for performance work → slow-response cost figures (Evidence) as cost framing, labeled industry estimates.
- Responsiveness = among central UX qualities → consider showing how fast system answered; visible response time (e.g. search retrieval time) signals fast system to users.

1968 response-time levels:
|Interaction|Respond within|
|---|---|
|activating control|≤ 0.1 s|
|keystroke echo|0.1–0.2 s|
|routine request acknowledged|≤ 2 s|
|complex impromptu request acknowledged|≤ 5 s|
|simple record lookup|≤ 2 s|
|first lines of next page|≤ 1 s|
|complex graphic|begins to appear ≤ 2 s; finishes ≤ 10 s|
|error report|2–4 s after user finishes input unit|
|hard break in attention|~15 s|
|context restored after failure|≤ 15 s|

Caveat: levels = one expert's reasoned estimates, flagged by author as needing field validation → treat as expert guidance, not measured data.

### Fill + place waits
- Perceived-performance work → waiting feels shorter + system seems to answer sooner.
- Hidden processing/pending load → motion on screen: gives eye something to follow.
- Percent-done indicator for any noticeable wait.
- Drive progress bars by real work; progress-bar accuracy = design obligation (point from 1985 progress-indicator research).
- Make progress indicators accelerate toward end.
- Show progress during waits; weigh honesty when shown progress not real.
- If wait > ~2 s → place after completion point, never mid-task.
- If operation > ~15 s → move to background + notify.
- Treat waits as potential negative experience peaks.

### Weigh a deliberate pause
- Work genuinely finishing sooner can still gain trust + how valuable its result seems when result held back on purpose.
- Use deliberate pauses sparingly + honestly; role = signal effort.
- Run well-being + honesty check first (see Humane bound).

### Cite the right law
- Identify mechanism first → then pick law; if no law fits → cite heuristic.

## Why it works

### Mechanism
- Under ~400 ms, exchange w/ system feels continuous → attention not broken.
- When real speed impossible → animation + progress indicators occupy attention during wait.
- Faster response does not reduce demand on computer; compresses same demand in time, because users do more work.
- No single acceptable response time exists; acceptable depends on where in activity wait falls (1968 analysis).
- Psychological closure: people chunk actions; each chunk ends in felt sense of completion. Delay inside chunk → goal + intermediate content held in short-term memory, where they decay/get disrupted; delay right after closure costs far less.
- Closures hierarchical: bigger completion recently reached → longer wait tolerated.
- Step-down discontinuities (1968): mental efficiency drops in steps as response time grows, not smoothly. Past certain point, 10 s reply may serve thinking-heavy work no better than 1- or 5-minute reply: attention already moved elsewhere.
- Waiting awareness sets in at ~2 s. Conversation silence > ~4 s feels like dropped line.
- Psychological present = ~2.3–3.5 s span felt as now.
- Think-time coupling (1979 measurements): each extra second of system delay added ~1 s to user's next think time. Users not calmly planning while waiting: they hold queued next actions in short-term buffer; delay breaks buffer → user must rebuild it.
- Some operations never feel instant however built (1985 progress-indicator research) → progress indicators needed.
- Progress indicator signals request received, accepted + interpreted + under way (list from 1968 analysis).
- Uncertain wait duration → tension + stops people scheduling another task or relaxing; known progress makes dead time usable.
- Percent-done bar = heartbeat: if program dies, bar stops; static hourglass shows neither speed nor crash.
- Progress-bar benefit comes from perceived progress → inaccurate bar still eases wait but hides hangs. Perception, not precision, drives benefit.
- Deliberate pause signals effort → raises perceived value + trust.
- Idleness aversion (2010): people dread idling + need justification to keep busy → wait filled w/ information or light entertainment feels shorter.
- Operational transparency, also called labor illusion (2011): customers seeing work done for them value service more, even w/ longer wait.

### Origin
- 1968 conference paper: different acceptable delays for 17 interaction kinds; introduced psychological closure + 15-second limit.
- 1979: think-time coupling measurements.
- 1982 IBM paper on economic payoff of fast system response: argued for sub-second response, w/ productivity rising steeply as response time falls.
- Later secondary summaries, not 1982 paper's text: 400 ms target replacing prior 2,000 ms (2 s) standard + label 'addicting' for applications responding < 400 ms = popular attributions. 400 ms far stricter than old 2 s bar.
- Productivity-vs-response-time curve (early-1980s IBM work): transactions per hour rise steeply as response falls below 1 s.
- 1985: first controlled test of progress indicators (see Evidence).

## Evidence

### Response time + productivity
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Productivity rises faster than proportionally as response time falls, sharp gain below 1 s; transaction rates rise steeply once response < 1 s|1982 IBM paper|vendor-authored industry paper; 400 ms later became popular threshold attributed to it|respond < 400 ms; otherwise animation + progress indicators|
|Programmer completed ~180 transactions per hour at 3 s response vs 371 at 0.3 s = +106%|early-1980s IBM measurements|industry measurements|latency budgets = cognitive budgets|
|Cutting system response by 2.7 s saved 10.3 s user time per interaction|same measurements|↑|slow system costs twice|
|17 s to user's next command at 3 s response vs 9.4 s at 0.3 s (17/9.4 s)|secondhand summary|secondhand, not peer-reviewed|—|
|Reported '339%' forecaster gain = in fact 3.39× rate (99 to 336 transactions per hour) = ~239% increase|1982 paper|small samples (5 forecasters, 15 engineers), before/after comparisons, no controls|quote increase as ~239%|
|Each extra second of system delay added ~1 s to next think time → overturned belief: ~2 s delay harmless because people think while waiting|1979 think-time coupling measurements|industry measurements|count think time in latency budget|

Caveats on 1982 figures: small samples (5 forecasters, 15 engineers), before/after comparisons + no controls; by IBM staff from IBM internal lab + project measurements → cite as industry engineering benchmark, not independent controlled study. Vendor-authored: authors = staff of hardware maker selling faster processors.

### Cases: cost of slow response
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Built for 300 users w/ 80% of transactions at ≤0.5 s; at 390 users average response rose to 4 s + average task time rose 50% (32 to 48 minutes). Slowdown cost extra 22,500 terminal hours per month, estimated at $900,000 = 15× cost of processor able to give sub-second response to 500 users|1979 national health-research computing utility|vendor-authored before/after report in 1982 paper; no controls; cost estimated|cost framing for performance work, labeled industry estimates|
|Cutting response from 2.3 s to 0.84 s → 39% less effort, 58% more output per programmer-month, 3.0 vs 6.9 trouble reports per 100 function points|programming project|vendor-authored before/after report in 1982 paper; no controls|same|

### Time perception
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|For 2–4 s intervals, ~±8% differences detected w/ 75% accuracy|classic time-perception data cited in 1968 analysis|classic psychophysics cited in 1968 conference paper|keep response-time variation below what users can detect|
|Time discrimination finest (under 10%) for 0.6–0.8 s intervals; coarser (20–30%) for 6–30 s intervals|same body of data|same|consistency matters as much as speed for repeated actions|
|Result feedback loses effectiveness when later than ~2 s|time-perception evidence|same|give result feedback within ~2 s|

### Progress indicators + waits
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Even imprecise progress bar makes wait more bearable|stated principle|no study cited|show progress; weigh honesty when not real|
|Percent-done indicator → significantly higher ratings on 10-item emotional scale (F = 13.70, p = .0006); 86.1% of participants liked indicators; w/o indicator, participants stopped watching screen during wait|1985 controlled within-subject experiment: 48 volunteers, mostly computer-science graduate students, ~14 queries each, constant 10 s or random 1–17 s delay, w/ or w/o percent-done indicator|first controlled test showing progress indicators improve how waits feel; mostly expert participants|percent-done indicator for any noticeable wait|
|Earlier finding (people prefer constant over variable delay) not replicated|same 1985 experiment|constant-vs-variable result = suggestive only|—|
|Bar speeding up near completion felt faster than constant-speed bar for same process|2007 HCI experiment|—|make indicators accelerate toward end|
|Trust + perceived result value can rise w/ pause added on purpose; far shorter real work time does not cancel effect|stated principle|no study cited|deliberate pauses sparingly + honestly|
|Wait design, three levers: goal gradient (every wait step explained), operational transparency (arrival estimate + method behind it), idleness aversion (animation during wait) → post-request cancellations fell 11%|Uber Express POOL, 2019 behavioral science work + A/B experiment|one company's A/B test; single in-house experiment, not general effect size|treat waits as potential negative peaks|

### Case: Google Search
- Home screen nearly unaltered since going live in 1998. Flow pieces: one text box focused on load; suggestions while typing; typed query stays on screen; refinement filters appear only once search has run; result-fetch time displayed; results grouped w/ white space between; video + featured-snippet results framed by border.
- Evidence = longevity + adoption, not study.
- Lesson: Hick's Law, working memory, Doherty Threshold, chunking, proximity + connectedness combined in one flow.

## Misreadings and limits
- Wrong: citing universal 2-second rule for response time → Right: 1968 analysis gives different limits per interaction level; some interactions need 0.1 s, others tolerate minutes.
- Wrong: assuming faster always better → Right: faster not always valued more; trust can rise w/ pause added on purpose, + honesty rules apply to such pauses.
- Wrong: tagging every timing as Doherty Threshold, e.g. citing it for pressed state under 100 ms → Right: 0.1 s, 1 s + 10 s = separate limits (1968 analysis; widely cited three limits); Doherty Threshold = 400 ms system-response threshold.
- Wrong: citing Doherty Threshold or any timing law for disabling button to prevent double charges → Right: belongs to error prevention + idempotency; cite error-prevention usability heuristic.
- Wrong: animating progress bar on timer → Right: hides hangs; bar should stop when work stops.
- Wrong: citing 400 ms figure or 'addicting' label as 1982 paper findings → Right: popular attributions from later secondary summaries. 'addicting' label usually reported together w/ 1982 threshold; some later accounts trace wording to dramatized film about response time, not to paper; 400 ms 'addictive' framing comes from television dramatization, not from IBM report → cite as reported characterization, not measured finding, + treat as well-being warning.
- Wrong: citing 1982 paper as independent controlled study → Right: industry engineering benchmark by IBM staff from internal measurements.
- Limit: 1968 levels = reasoned estimates, unvalidated.

### Wider mistake: attaching a law to behavior it does not explain
- Doherty Threshold = system response time; not 0.1 s pressed state + not double-charge prevention (error prevention + idempotency instead).
- Peak-End Rule: concerns emotional peak + real end of episode, not mid-journey Skip tap → always name both halves (peak + end), never ending alone.
- Rule: identify mechanism first, then pick law; if no law fits → cite heuristic.

### Overstated evidence to avoid
- Parkinson's Law comes from humorous essay.
- Pareto Principle's 80/20 split = approximate.
- 1982 Doherty Threshold figures = vendor-authored.
- Goal-Gradient Effect rests on animal studies + 2006 human field study of real rewards: customers accelerating more toward first reward more likely to earn another + returned sooner → never restate it as finding about why people drop out.
- Complexity bias: 1989 study illustrates it well (most participants proposed rules more elaborate than hidden rule = any three ascending numbers), but study's own conclusion concerns reasoning strategies shifting w/ task. Three-number rule-discovery task itself dates from 1960.

## Check questions
- [A] (response-time limits: 1968 analysis; 0.1 s limit of widely cited three; not Doherty Threshold) Direct-manipulation feedback (pressed state, echo, drag) within ~0.1 s? Look for: no pressed state; typing lag.
- [A] (Doherty Threshold) System responds < 400 ms? Look for: silent waits; no immediate input acknowledgement.
- [A] (Doherty Threshold) Unavoidable waits covered by animation/progress indicator? Look for: blank screens during processing.
- [A] (Doherty Threshold: closure) Waits > ~2 s fall after completion point, never mid-task? Look for: spinners between sequence steps; validation interrupting typing.
- [A] (1968 response-time levels, Doherty Threshold) Operations > ~15 s run in background w/ notification? Look for: modal blocking screens during long jobs.
- [A] (Doherty Threshold, Goal-Gradient Effect) Every progress bar driven by real work? Look for: bars filled by timer; spinners w/o estimate where estimate possible.

## Symptoms → fixes
|Symptom|Likely cause (laws)|Fix|
|---|---|---|
|App feels sluggish|Doherty Threshold|acknowledge input within 400 ms; animation/progress bar for longer work|
|Long operation holds users hostage|↑|waits after completion points; past ~15 s move job to background + notify; drive progress bars by real work|
|Content jumps while loading + causes mis-clicks|Doherty Threshold, Fitts's Law|reserve space for late content; never move target under pointer; layout stability in performance budget|
|Refreshing data blanks screen or gives no sign of what changed|Doherty Threshold; visibility-of-system-status heuristic (what changed + when); Working Memory|skeleton only on first load; on later refreshes keep stale data visible w/ inline cue + last-updated time|
|Payment/other processing wait at checkout|1968 levels set budget (routine request acknowledged within 2 s; ~15 s = hard break); Doherty Threshold's 400 ms usually out of reach here → mitigate|acknowledge at once; show processing state; block resubmission (error prevention); past ~15 s explain current status|

## Hypothetical examples
- Hypothetical (showing response speed): payroll tool shows calculation time next to each finished pay run → signals fast system.
- Hypothetical (loading animation): train-booking app draws journey-list skeleton while timetables load → screen never blank.
- Hypothetical (progress bar): patient portal exporting full medical record shows percent-done bar advancing only as each document packaged, + stopping if packaging stalls.
- Hypothetical (deliberately added delay): loan-eligibility checker finishes instantly but holds answer briefly behind "checking your details" step → defensible only if checks real + pause passes well-being + honesty check.

## Humane bound
- Turned against people: speed tuned for compulsion; sub-400 ms applications once called addicting = reported characterization, not measured finding; deserves scrutiny.
- Turned against people: artificial delay inflating perceived value of trivial work.
- Turned against people: progress bar deliberately misrepresenting progress; bars help even when inaccurate → honesty = designer's choice.
- So-called addicting responsiveness + artificial delays need well-being + honesty check before use.
- Fast apps called addicting, progress bars helping even when inaccurate + trust-raising artificial delays = levers; each can mislead → weigh against well-being + honesty via influence-versus-manipulation lever tests.
- Bounded by Transparent: no faked progress, no faked effort.
- Bounded by Intentional: zero + excessive friction both destroy value.
- Bounded by Finite: against compulsive use.
- Further reading for this bound: influence versus manipulation; using psychology responsibly; convenience + friction evidence.

## Related
- ../methods/thresholds-and-formulas.md: measurable form of every law, response-time limits included.
- flow.md: replies within 400 ms keep focus on task.
- goal-gradient-effect.md: progress shown during waits; shared question: progress bars driven by real work?
- peak-end-rule.md: wait can become experience peak.
- fittss-law.md: content jumping while loading causes mis-clicks.
- working-memory.md: screen-blanking refreshes hide what changed.
- ../checklists/usability-heuristics-map.md: links Doherty Threshold to heuristic visibility of system status (related laws: Doherty Threshold, Goal-Gradient, Zeigarnik); holds error-prevention heuristic for double charges; classic usability heuristics date from 1990, revised 1994.
- ../principles/transparent.md: humane principle bounding Doherty Threshold; no faked progress or effort.
- ../principles/intentional.md: humane principle bounding Doherty Threshold; zero + excessive friction both destroy value.
- ../principles/finite.md: humane principle bounding Doherty Threshold against compulsive use.
- ../ethics/influence-vs-manipulation.md: lever tests for fast-as-addicting, inaccurate progress bars + artificial delays.
- ../ethics/using-psychology-responsibly.md: humane guardrails; flags addicting sub-400 ms responsiveness + deliberately added delays as ethically sensitive levers.
- ../evidence/convenience-and-friction.md: what removing/adding friction does; bounds cases where speed alone = goal.
- ../guides/laws-and-principles-crosswalk.md: shows humane principle bounding Doherty Threshold.
- ../patterns/search-and-results.md: applies Doherty Threshold.
- ../patterns/feedback-loading-and-performance.md: applies Doherty Threshold to perceived performance.
- ../patterns/progress-goals-and-completion.md: applies Doherty Threshold to task completion.
- ../patterns/ai-and-automated-features.md: applies Doherty Threshold to AI assistants + automated features.
