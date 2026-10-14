# Thresholds and formulas

## Use when
- Spec, finding / rationale needs number: response-time budget, target size, option count, threshold, formula, or choice of what to measure in test.
- Holds each UX law's measurable form (response-time limits, target sizes, formulas), each quantity w/ origin + how to apply it.
- Rule: only quantities w/ traceable origin listed; add none w/o citation.

## Response time
|Limit|Meaning|Origin|Strength + caveat|Apply as|
|---|---|---|---|---|
|0.1 s|response feels instantaneous; limit for direct-manipulation feedback|1968 estimates; fits ~100 ms perceptual cycle of model human processor|part of practitioner's set (0.1 s / 1 s / 10 s) built on 1968 estimates + model human processor work|pressed state appears within 0.1 s|
|1 s|user's flow of thought stays uninterrupted|same practitioner's set|—|server round trip budget: 400 ms / 1 s|
|10 s|user's attention stays on task|↑|—|budget long jobs against it|
|400 ms|Doherty Threshold: system response < 400 ms|popular figure attributed to 1982 paper|paper itself argues for sub-second response; 400 ms = figure quoted from it|acknowledge every user input < 400 ms; server round trip at 400 ms / 1 s|

- Tag each response-time figure w/ own source; limits have different origins. 400 ms (Doherty Threshold, 1982) = separate system-response threshold, not part of 0.1 s / 1 s / 10 s set.
- If work runs slower than Doherty Threshold → instant feedback first, then animation / progress bar.
- Showing system's response speed (e.g. search's retrieval time) signals speed.
- Wrong: response-time limit justifies double-submit protection → Right: none does; preventing double submits = error prevention.

### Finer levels (1968 expert estimates)
|Interaction|Level|
|---|---|
|Control activation|≤ 0.1 s|
|Keystroke echo|0.1–0.2 s|
|Routine request acknowledged|≤ 2 s|
|Complex impromptu request acknowledged|≤ 5 s|
|Simple record lookup|≤ 2 s|
|First lines of next page shown|≤ 1 s|
|Complex graphic|begins ≤ 2 s, finishes ≤ 10 s|
|Error report|2–4 s after input unit ends|
|Delay = hard break in user's work|~15 s|
|Context restored after failure|≤ 15 s|

- Budget response time per interaction level, not as one global target.
- Caveat: reasoned expert estimates, flagged by their author as needing field validation; not measured data.
- Wrong: these levels belong to Doherty Threshold (often filed there) → Right: separate source.

## Task duration
- Parkinson's Law benchmark = user's expected task duration.
- Measure expected vs actual task time → aim to finish under user's expectation, e.g. w/ autofill + reuse of entered data.

## Choice and memory
|Quantity|Value|Origin|Strength + caveat|Apply as|
|---|---|---|---|---|
|Hick's Law|RT = a + b log2(n), n = number of options|experiments published 1952 + 1953|—|decision speed critical → cut options, split across steps, or add recommended default|
|Miller's Law|about 7 ± 2 items|1956 paper|later research argues capacity nearer 4; prior knowledge + setting shift how many items one can hold|chunk information|
|Working memory|4–7 chunks, each fading after ~20–30 seconds|—|—|assume anything seen more than a few steps / ~20 seconds ago = gone; keep inputs, selections + compared attributes visible on later screens|

- Hick's Law mechanism: deciding takes longer as options get more complex + as log of their count rises.
- Wrong: Miller's Law caps number of items → Right: reason to chunk, never cap.

## Cognitive load
- Relative condition efficiency (1993) = (standardized performance − standardized mental-effort rating) ÷ square root of 2.
- Compare design variants on outcome per unit of perceived effort, not success rate alone.
- 2008 study found load measures respond differently to intrinsic, extraneous + germane load.
- Limit: physiological load signals (e.g. task-invoked pupil dilation) reliable in lab but largely have not held up outside it.

## Attention and emphasis
|Quantity|Value / finding|Origin|Strength + caveat|Apply as|
|---|---|---|---|---|
|Selective Attention|region's share of eyetracking fixations vs its share of screen area|—|—|metric for whether region gets seen|
|Right-rail filtering|1 of 132 content-area fixations (0.8%) on right rail taking 25% of content area = ~33 times fewer than its size predicts|eyetracking|one user|—|
|Von Restorff Effect|one isolated item in list of same-category items recalled better|1933 experiments|—|keep highlights few → no standout mistaken for ad, no highlights fighting each other|
|One primary standout per decision area|default|—|practical default, not research rule|—|
|Serial Position Effect|primacy + recency effects in recall|—|—|key items first + last; least important in middle|

- Symptom → cause: region w/ far fewer fixations than its share of space → users filter it out, whatever its contents.

## Targets and pointing
|Quantity|Value / finding|Origin|Strength + caveat|Apply as|
|---|---|---|---|---|
|Fitts's Law|farther target → longer to acquire; larger target → less time|1954|model has no size threshold; same distance-and-size relationship behind every formula variant|steps below|
|Error rate|climbs when movement quick + target small|—|—|—|
|Positional touch targets|~7 mm in scrolling centre of screen; ~12 mm in corners|field observation reported in 2017|adjustment, not floor|apply on top of platform / accessibility minimum|
|Throughput|accuracy-adjusted throughput in bits/s; effective width (We) from spread of actual hit points|1956 + 1964 work; standardized in ISO 9241-9|fitting a + b constants contested; fitting method can create differences > real ones between devices|device + layout testing|

1. Meet platform / accessibility minimum target size first.
2. Apply 2017 positional figures as adjustment on top.
3. Then size relatively: frequent / critical targets larger + closer to current focus, w/ more spacing from neighbours, in easy-reach zones.
- Compare devices / layouts by throughput, counting misses; otherwise aggressive users look falsely fast.

## Prioritizing and complexity cost
|Quantity|Value|Origin|Strength + caveat|Apply as|
|---|---|---|---|---|
|Pareto Principle|most effects (roughly 80%) trace back to minority of causes (20%)|observation: 20% of Italy's population owned 80% of its land|80/20 split approximate|rank features, issues + user segments by impact; invest first in small set giving most value to most users|
|Tesler's Law, industry framing|1 lost minute per user per day × 1,000,000 users, vs single added engineer-week|—|—|weigh build cost against summed user cost|
|Tesler's Law cost formula, generalized|complexity frequency × active users × cost per encounter|2017|user cost almost always wins over one-off build cost|compare multiplied user cost w/ one-off build cost|

- One-off build cost of absorbing complexity = often one week or more of team time.
- Pick time window (week, year / customer lifetime) + currency (time, money / utility) before computing.
- Caveat: 2017 worked example (3 encounters per week × 1,000,000 users × 0.5 minutes) mixes seconds + minutes in its totals → quote formula, not worked example's figure.

## Remembered experience
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Trial A = 60 s at 14°C; trial B = 60 s at 14°C + 30 s warming to 15°C; most people chose to repeat longer trial|1993 experiment|"most"|better ending can outweigh added duration in memory|
|Colonoscopy + lithotripsy patients' pain ratings followed worst moment + last moment, whatever procedure length|1996 clinical study|—|duration + averages matter less than peak + end|
|Adding 3 minutes w/ scope left in place but no suction / inflation → gentler ending, lower overall unpleasantness, more willingness to return|2003 clinical study|—|soften last step of painful flows even if it adds a little time|
|Choice-supportive bias: people recall own past choices as better than reality|2000 research|—|collect in-the-moment ratings beside retrospective surveys|
|Perceived ease tracked aesthetic ratings more than actual ease did|1995 Aesthetic-Usability study; 26 ATM interface layouts; 252 participants|—|measure task success separately from satisfaction|

- Mechanism: retrospective ratings track peak, end + person's current mood.
- Collect in-the-moment ratings (experience sampling) alongside retrospective surveys.
- Wrong: end-of-journey score records each step → Right: never read it this way.
- Time surveys away from unresolved problems liable to color recall.

## Learning over repetitions
- Power law of learning (1980): task time falls w/ repetitions, straight line on log-log axes.
- For Jakob's Law + learnability: compare familiar + novel designs across repeated trials, not on one first use.
- Plot time per repetition → find each design's saturation point (where practice barely helps) + plateau time.
- If task rare → choose design quickest to learn; if daily → one fastest at plateau.
- Wrong: tutorial shown once = learning → Right: practice frequency + recency set fluency.

## Progress and goals
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Effort rises as goal nears; rats sped up as they neared food|proposed 1932; animal work 1934|—|show steps remaining; grant honest head start|
|Customers accelerating more toward first reward more likely to earn another + returned sooner|2006 goal-distance study|—|per-user acceleration toward first goal = early retention signal|
|10-stamp card w/ 2 stamps pre-filled → 34% redemption vs 19% for blank 8-stamp card; same 8 purchases required|2006 endowed-progress study|—|reframe fixed work as already started; never add fake steps|

- Goal distance for goal-gradient analytics (2006): d = (r − n)/r. Model visit rate, units per session + mid-session exits against d.
- Use behavioral logs for goal-gradient analysis, not hypothetical surveys.
- Phrase goal-gradient falsifiers as retention prediction, not as claim about why other users dropped out.
- Open question to A/B test: does "70% complete" or "3 steps left" motivate more? 2006 paper left this open.

## Accessibility floors
|Floor|Value|Source|
|---|---|---|
|Text contrast|4.5:1|WCAG 2.2 AA|
|Large text + non-text UI contrast|3:1|WCAG 2.2 AA|
|Target size|24 × 24 CSS px, or equivalent spacing|WCAG 2.2 AA|
|Zoom|content stays usable at 200%|WCAG 2.2 AA|
|Target size, iOS|44 × 44 pt|platform|
|Target size, Android|48 × 48 dp|platform|

- Meet these floors in every spec; cite as standards, not as laws / research effects.
- Pair each floor w/ supporting law: Fitts's Law → targets; Von Restorff Effect + figure-ground → contrast; Working Memory → error summaries.

## Measuring in tests
|Check|Passes when|Law / principle|
|---|---|---|
|Behavioral analytics used|rage clicks (repeated rapid clicks on one element), dead clicks + step-by-step funnel drop-off point to broken affordances + friction hotspots|—|
|Cause of struggle explained|analytics paired w/ session review + observation (analytics show where, not why)|—|
|Accessibility + performance covered|automated audits (partial proxies) backed by manual keyboard + screen-reader passes|accessibility floors|
|Satisfaction read correctly|end-of-session satisfaction paired w/ moment-by-moment measures (in-session ratings, behavioral logs) + task success|Peak-End Rule|
|Polished prototype judged fairly|behavioral metrics weighted over satisfaction|Aesthetic-Usability Effect|

- Why pair: end-of-session satisfaction reflects remembering self + over-weights peaks + endings; retrospective interviews + surveys also level some details + sharpen others; appeal inflates self-reported ease.
- Symptom to watch: attractive design's ratings rise after use while plain design's ratings fall.

## Hypothetical examples
- Hypothetical: hospital pharmacy tool's spec sets pressed state within 0.1 s, budgets drug lookup at its own interaction level + full-ward report against 10 s attention limit, w/ instant acknowledgement then progress bar.
- Hypothetical: tax portal weighs prefilling employer details: frequency × active users × cost per encounter over one tax year, currency = citizens' time, vs one-off build cost; formula quoted, not someone else's worked total.

## Related
- [UX laws index](../laws/index.md): all 30 laws by theme w/ core idea + design rule.
- ../evidence/citation-caveats.md: contested numbers + misattributions to check before quoting figures.
- [Stating and citing evidence accurately](../evidence/stating-evidence.md): quoting studies, numbers + origins accurately.
- [Feedback, loading and perceived performance](../patterns/feedback-loading-and-performance.md): response-time budgets applied to indicators, skeletons + waits.
- ../patterns/calls-to-action-and-touch-targets.md: target size, spacing + placement in practice.
- ../patterns/inclusive-and-accessible-design.md: humane side of accessibility floors.
- [Pareto chart for prioritizing](pareto-chart.md): step list behind Pareto row.
- measure-what-you-value.md: humane bound on measurement; metrics reflecting value to people.
- ../laws/doherty-threshold.md: 400 ms threshold, its source + its misfiling.
- ../laws/parkinsons-law.md: expected task duration as benchmark.
- ../laws/hicks-law.md: decision-time formula.
- ../laws/millers-law.md: 7 ± 2 + its later revision.
- ../laws/working-memory.md: chunk capacity + decay; error summaries.
- ../laws/cognitive-load.md: relative condition efficiency + load measures.
- ../laws/selective-attention.md: fixation share vs area share.
- ../laws/von-restorff-effect.md: isolation + contrast.
- ../laws/serial-position-effect.md: primacy + recency.
- ../laws/fittss-law.md: targets, throughput, positional figures.
- ../laws/pareto-principle.md: 80/20 + its origin.
- ../laws/teslers-law.md: complexity cost formula.
- ../laws/peak-end-rule.md: remembered experience studies + survey rules.
- ../laws/aesthetic-usability-effect.md: perceived vs actual ease.
- ../laws/jakobs-law.md: learning curves for familiar vs novel designs.
- ../laws/goal-gradient-effect.md: goal distance, acceleration + head starts.
