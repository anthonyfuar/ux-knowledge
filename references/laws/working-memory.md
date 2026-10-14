# Working Memory

## In one line
Working memory (WM) = mind's short-lived workbench: what task needs sits there briefly while operated on; small + fast-decaying, holds few chunks (4–7), each fading after ~20–30 s. Interface should offload this active workspace; design for recognition over recall: remembering = system's job, not user's.

- Matters most for persisting input across screens, visited states + breadcrumbs, comparison tables. Theme: Memory.
- Class: construct. Historical aliases: primary memory, immediate memory, short-term memory or short-term store, provisional memory, operant memory.

## Applies when / does not apply when
|Applies when|Watch out|
|---|---|
|any task where people briefly hold + manipulate information|capacity not fixed: prior knowledge + circumstances shift it|
|items on screen yet needing active tracking|still cost WM capacity: visible items not free|
|people decide, reason or choose, not only recall|crowding WM degrades choices too|
|learning features where retention = goal|"desirable difficulty" aids retention, hurts usability: use only where retention = goal, never in routine task flows|

## Which number to plan with
Name claim meant; 7±2, 4–7 + ~four = different claims, never merged into one "rule".

|Figure|Meaning|Use / caveat|
|---|---|---|
|~4 to 7 chunks, each fading after roughly 20 to 30 seconds|design working range|backed by later capacity research proposing ~four; not from one study|
|~4 new chunks at once|planning figure (2001 estimate)|plan ~4, not 7, especially for brief or unpredictable displays; 4-7 = broad working range|
|~3-5 chunks|central limit, young adults (2001 paper, 2010 review)|central-store estimate under tightly controlled conditions; real-task span varies w/ strategy|
|roughly 3 items|visual WM load plateau (2013)|holds whether items stay on screen or sit in memory|
|~4 / 1 chunk|items in focus of attention (embedded-process view / its narrower-focus variant)|memory can hold many active items|
|~3 variables|practical ceiling for relations handled at once (relational complexity)|pre-compute comparisons|
|seven (Miller's Law)|not design cap; later research points to ~four|invited address April 15, 1955, published 1956: cite 1956, though some copies say 1955|
|3-4, ~4-6 (1975), as few as 3 (1999), 7|explainers' figures|from different tasks + conditions|

## Decision rules
Show state, do not ask people to remember
- Treat anything seen > a few steps or > ~20 seconds ago as gone; keep inputs, selections + compared attributes visible on later screens.
- Keep inputs, visited states, breadcrumbs + comparisons visible; never rely on users remembering what they saw.
- Mark visited information (breadcrumb trails, distinct visited-link look) → recognition replaces recall.
- System, not people, holds key details from screen to screen: later screens re-show them; when several items weighed, side-by-side table does it.
- Keep user's own input visible later, e.g. search results headed by query as first typed.
- Show only relevant + needed items: what people saw earlier often slips from memory.
- Support user-made external memory: comparison tables, carts as shortlists, saved lists, candidates parked in separate tabs (page parking) w/ stable URLs + preserved state.
- Let system hold information people know they can look up.

Holding + operating
- Plan ~4 new chunks at once (2001 estimate), not 7, especially for brief or unpredictable displays; 4-7 = broad working range.
- Users cannot run parallel mental operations (e.g. comparing several numbers at once) → sequence them or let comparison view do it.
- Keep worked-on object selected + stable across consecutive actions.
- Limit how many items users track at once; on-screen items do not free capacity if users must track them.
- Do not make users hold codes or values in mind while navigating or deciding.
- Never make users translate or convert code while holding it in mind; show final, familiar form.
- Allow no interruptions between showing information + using it.

Chunk + encode
- Pre-chunk content; learned groupings let more fit within same limit.
- Give ready-made familiar groupings (dates, standard formats), not ones users must build: chunks help only when recognized.
- When users must recall items distinctly → vary types or form sub-groups, not uniform run.
- Pair visual w/ short verbal label rather than more same-kind material.
- Present related image, label + status together as one unit.
- Write microcopy for gist: gist survives, exact wording does not.

Stress, people + context
- Payment, medical, legal, error + emergency flows run under stress → simplest flows, visible state, recoverable steps.
- Suspect WM load before low motivation.
- Judge difficulty w/ representative users, incl. older + less experienced ones; estimate capacity generously only for specialist expert audiences.
- On small screens → compensate w/ summaries, sticky context + fewer cross-section dependencies.
- For long, interrupted work → free-text notes on data sets, charts + models, plus action histories → people can resume after breaks.
- Put help in place, not in separate help center (retrieval easiest where memory formed).
- Give children smaller loads; audio + visuals aid encoding, but do not assume they double central capacity.
- Memory demands = accessibility issue; minimize them for learners + cognitively diverse users (correlational + longitudinal studies: WM predicts learning better than IQ in some groups).

Attention + load
- Declutter simple screens; never put essentials in periphery of demanding screens; do not load memory while users must ignore noise.

Learning features
- Use retrieval practice, spaced reminders + user-generated input rather than passive reading.

Citing
- Many error-prevention fixes (idempotent submit, undo, soft delete, constraints) need no law → cite heuristic alone, not borrowed timing or motor law.

## Why it works
1. Decisions run on it: behavior + decisions take direction from WM; reasoning rests on it → crowding it degrades choices, not only recall.
2. Every element costs: people weigh everything shown against what they came to do → each visible thing can become choice to make.
3. Decay by intervening decisions: recall of earlier-held items weakens w/ each extra decision in between.
4. Recognition beats recall: fresh material hard to hold ready, material met before easy to recognize → showing state + prior choices lowers load.
5. Context-bound retrieval (cue-dependent forgetting): retrieval easiest in context where memory formed.
6. Offloading: people forget what they know they can look up.
7. Gist: message's gist survives in memory, exact wording does not.
8. Recoding: pays off only once translation nearly automatic; otherwise next group lost while person converts last one (1956 paper).
9. Variation by person + state: capacity rises through childhood, falls w/ age; cut by stress, sleep loss + alcohol.
10. Designer capacity bias: product teams, especially developers, self-select for large WM → flow easy for team can overload typical users.
11. Interrupted expert work: expert tasks span hours or days w/ frequent interruptions; each step's rationale sits in WM, lost when attention moves elsewhere.
12. Closely tied to cognitive-load.md.

## Models and terms
|Term|Meaning|Design use|
|---|---|---|
|Short-term memory|older term: retention lasting only seconds or so|WM adds manipulation of held items|
|Multicomponent model (1974, extended 2000): central executive|steers attention, suppresses distraction, coordinates dual tasks|—|
|Multicomponent model: phonological loop|rehearses speech-like material|—|
|Multicomponent model: visuospatial sketchpad|holds images, shapes + locations|pair visual w/ short verbal label|
|Multicomponent model: episodic buffer (added 2000)|binds verbal, visual, spatial + semantic pieces into one episode; links to long-term memory|present image, label + status as one unit|
|Embedded-process view|WM = activated part of long-term memory; can hold many active items, ~4 in focus of attention|—|
|Narrower-focus variant|focus of attention holds 1 chunk at a time|—|
|Long-term working memory (1995)|expert retrieval structures act as extra working space|—|
|Three-level framework (2003–2018)|WM as attention to memory; focus holds ~one item, shifts in ~300 ms; bottleneck = controlling attention, not attending|—|
|Relational complexity|capacity = number of relations handled at once; ~3 variables = practical ceiling|pre-compute comparisons|
|Time-based resource-sharing model|load = temporal density of attention demands; memory refreshed in idle gaps|—|
|Inhibition-deficit hypothesis|older adults filter out irrelevant input less well|—|

## Origins
|When|What appeared or was shown|
|---|---|
|more than 100 years ago, at start of neural research|early prefrontal-tissue removal (ablation) experiments led researchers to tie frontal cortex to thought, not senses|
|1935, 1936|lesion (ablation) studies first showed prefrontal ablation harms delayed-response performance|
|1960s|term working memory coined; used in computer-analogy theories of mind|
|1968|term applied to "short-term store" of one memory model|
|present day|focus = processing, not storage alone → most current theorists either let WM supersede short-term memory or count short-term memory as part of it|

Neural-basis work = background only: supports WM as distinct, limited system.

## Evidence
Capacity
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Young adults hold ~3-5 chunks when rehearsal, grouping + sensory traces blocked|2001 paper + 2010 review of converging memory experiments|tightly controlled conditions|plan ~4 new chunks|
|Running-span tasks (list ends unpredictably): people recall only last 3-5 digits|running-span tasks|—|plan ~4 new chunks, especially for unpredictable displays|
|Longer verbal units (idioms, brief sentences): young adults hold only 3 or 4|2008 study|—|—|
|Problem-solving models fit best w/ capacity near 4|problem-solving models|"near"|—|
|Arbitrary word pairs trained into new chunks; w/ rehearsal blocked, people recalled ~3 units whether single words or learned pairs → capacity counted in chunks, not words|memory experiment|—|pre-chunk content|
|Neural marker of visual WM load rose w/ set size up to roughly 3 items, then plateaued, whether items on screen or remembered|2013 EEG experiment|—|visible items not free: limit tracked items|
|Shifting focus of attention between items takes ~300 ms; operating again on same item faster|2003|—|keep worked-on object selected + stable|
|7-year-olds held ~1.5 items vs ~3.0 for older children + adults|coloured-shape array studies|—|smaller loads for children|
|Sensory memory masked → people held ~4 items total whether all visual or split between seeing + hearing; unmasked, two modalities beat one|2007 cross-modal study|—|audio + visuals aid encoding, do not double central capacity|
|14-month-olds (capacity ~three objects) remembered four when two of each of two kinds (two cats, two cars), but not four of one kind|2014 infant looking-time study|—|vary types or form sub-groups|
|Pairs + triples shown at once recalled more easily than singletons; chunk stored as one item whatever its content|2020 adult visual-memory study|—|vary types or form sub-groups; pre-chunk content|

Recoding + expertise
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|20 people had spans of 9 binary digits + 7 octal digits|recoding experiment reported 1954, described in 1956 paper behind Miller's Law|—|—|
|After 5-10 minutes learning grouping-and-renaming scheme, every person's binary span rose, but less than their octal span predicted; shortfall grew w/ larger recoding ratios|same 1954 recoding experiment|—|do not make users convert codes in their head|
|Experimenter drilled each scheme on himself: his span of 12 octal digits worth 24 binary digits at 2:1 ratio, 36 at 3:1, ~40 at 4:1 + 5:1|same 1954 recoding experiment|single person|recoding pays off only once nearly automatic|
|Undergraduate long-distance runner raised digit span from 7 to ~80 over ~20 months + ≥ 230 hours of practice, by recoding digits as race times|1980 expert-memory training study|single trained person|chunks help only when recognized|
|He still grouped only 3–4 digits at a time, never rehearsed > 6 digits or > 4 groups per supergroup; his letter span did not improve|same 1980 training study|—|give ready-made familiar groupings|
|Such trained span gains attributed to long-term memory structures|later accounts, 1995 + 2000|—|—|

Interference + timing
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|People held 1 to 6 digits while judging sentences about letter order; holding 1-2 did not hurt reasoning, holding more did|1974 dual-task experiment|—|do not make users hold values while deciding|
|30-second distractor before recall removed recency effect, left primacy; short-term capacity estimated 3-4 chunks|1966 free-recall experiments|separates short- from long-term contributions to serial-position effects|no interruptions between showing + using information|
|Roughly 15-30 seconds of distraction cancels recency effect|—|"roughly"|no interruptions between showing + using information|
|Long-term recency appears when distractor follows every item|1974|—|—|

Load + distraction
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Peripheral distractor slowed letter search when other positions empty (low load), not when non-target letters filled them (high load)|1995 lab experiment|—|declutter simple screens|
|Even personally interesting distractors (cartoon characters) stopped distracting under high load|2007 lab experiment|—|—|
|Visual cortex responded less to distractors under high load|2005 imaging study|—|—|
|WM load raises distraction, while perceptual load reduces it|2016 review|review|do not load memory while users must ignore noise; essentials never in periphery of demanding screens|

State, person + device
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Acute stress rapidly weakens prefrontal WM networks|—|—|simplest flows under stress|
|Apparently careless or unmotivated users may lack capacity to hold instructions|2009 finding in children|"may"|suspect load before motivation|
|Capacity correlates positively w/ education + IQ, negatively w/ age|—|correlation|judge difficulty w/ representative users|
|Less prior text visible on phone → difficult text understood more slowly than on large screen (small screens lose screen-as-memory)|—|—|summaries, sticky context, fewer cross-section dependencies|
|Recognition far easier than recall: holding fresh material ready far harder than identifying material met before|—|established principle, no single study named|recognition over recall|

Learning + development
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|WM capacity first linked to reading comprehension|1980 study|—|—|
|WM at age 5 beat IQ at predicting academic success|one longitudinal study|one study|memory demands = accessibility issue|
|Screening flagged ~1 in 10 mainstream children as having WM deficits|screening|"about"|↑|
|Among 37 learning-disabled children, baseline WM, not IQ, predicted learning 2 years later|—|—|↑|
|Dual n-back training reported to raise fluid intelligence (2008); replicated (2010); two 2012 studies did not|2008, 2010, 2012 studies|contested|—|
|Meta-analyses of ~30 WM training studies disagree on IQ gains, agree effects weaken w/ task's distance from trained one|meta-analyses|—|near-transfer claims only|
|Spatial WM gains + 16-percentage-point higher admission to academic track 4 years later|randomized trial, 580 six-year-olds|—|—|
|Training transfers poorly to general ability: near-transfer claims defensible in brain-training products; general-intelligence claims contested|—|contested|—|

Case
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Google Search landing + results: one auto-focused field, autocomplete, filters only after query, query kept visible on results, retrieval time shown, results in spaced chunks, borders around videos + featured snippets; landing page little changed since 1998 launch|product case|evidence = longevity + adoption, no study|hicks-law.md, Working Memory, doherty-threshold.md, chunking.md, proximity + connectedness all applied in one flow|

## Misreadings and limits
- Wrong: cap menu at seven "because of Miller's Law". → Right: seven = reason to chunk, not limit; capacity possibly nearer four.
- Wrong: visible dashboard low-load because nothing to remember. → Right: more than ~3 interacting variables overload people even w/ all data visible → pre-compute comparisons.
- Wrong: flow easy because team finds it easy. → Right: teams (designers + developers) have above-average WM while real users often tired, stressed, older or distracted → test w/ representative, older + less experienced users.
- Wrong: inattentive or "careless" behaviour = low motivation. → Right: often WM overflow → externalize state + instructions.
- Wrong: grid of look-alike cards = Similarity or Selective Attention problem. → Right: neither; uniform cards correctly read as one content type; problem = comparing across cards (Cognitive Load, Working Memory).
- Wrong: 7±2, 4–7 + ~four = one rule. → Right: different claims; name the one meant.
- Wrong: WM training raises general intelligence. → Right: transfers poorly to general ability; near-transfer claims defensible in brain-training products, general-intelligence claims contested.
- Limit: 3-5 chunks = central-store estimate under tightly controlled conditions; real-task span varies w/ strategy.
- Limit: desirable difficulty only where retention = goal.

## Check questions
- [A] (Working Memory): UI shows state instead of asking people to remember? Look for query or input lost on next screen, no visited-link styling, no breadcrumbs, comparisons needing memorized details.
- [A] (Working Memory, Cognitive Load): can users finish steps w/o holding value (code, price, name) from another screen or while scanning similar material? Look for retyping code shown elsewhere, or remembering one name while scanning similar names.
- [A] (Working Memory): comparisons of more than 2-3 interacting variables pre-computed? Look for plan or pricing matrices w/o pre-computed comparisons.
- [A] (Working Memory): stressful states (error, payment) demand less memory than normal states? Look for transient error toasts, hidden recovery steps, input lost after failure.
- [A] (Working Memory): can users record their reasoning in long, interrupted tasks? Look for no notes on models, charts or data sets, + no action history.
- [A] (error-prevention + recovery heuristics, Working Memory): errors tied to their fields + announced to screen readers (live region or focused error summary)? Look for red borders only, vanishing toasts, errors far from their fields.

## Symptoms → fixes
|Symptom|Laws / heuristics|Fix|
|---|---|---|
|Query or selections forgotten on next screen|Working Memory|keep inputs visible; comparison tables, visited states, breadcrumbs|
|Codes or IDs copied from elsewhere get mistyped|Chunking, Working Memory|show in delimited groups of 3-5, accept paste, keep code visible where entered|
|Errors or payment failures spiral into abandonment|Working Memory, Cognitive Load|show problem, input + next step together; stress cuts capacity → simplify recovery most of all|
|Refreshing data blanks screen or gives no sign of what changed|Doherty Threshold, visibility-of-system-status heuristic, Working Memory|skeleton on first load only; later keep stale data visible w/ inline cue + "last updated" time. Doherty Threshold here: response over 400 ms → speed up or mitigate; spinner mitigates, does not meet threshold. Visibility heuristic here: show what changed + when|
|Card declined or payment times out|Working Memory, Peak-End Rule (negative peak), error-recovery heuristic|keep all fields, clear only security code; give plain-word reason + another payment method; on timeout check order status before any retry|
|Grid of look-alike cards hard to compare|Cognitive Load, Working Memory (comparing across cards)|show deciding attributes (price, rating, key spec) consistently, plus sort + filters|
|Filters, query or scroll position lost on Back|Working Memory, Tesler's Law (system should carry state), user-control heuristic|keep state in URL; restore scroll position + filters on return|

## Hypothetical examples
- Hypothetical: traveler silently repeating newly announced gate while walking through terminal = phonological loop rehearsing speech-like material.
- Hypothetical: tax preparer reopens half-finished return after weekend, cannot recall why one deduction got flagged; reason lived only in WM. Note field on flagged line would have kept it.
- Hypothetical: university course catalog marks previewed courses, shows path Faculty > Program > Course, keeps shortlisted courses side by side in comparison panel: visited state, breadcrumb + comparison carry memory work.

## Humane bound
- No recorded case of Working Memory turned against people; general [influence-versus-manipulation test](../ethics/influence-vs-manipulation.md) applies.
- Recorded risk: crowded WM degrades choices, not only recall; capacity cut by stress + sleep loss, falls w/ age → flow judged by team's ease overloads typical users → memory demands = accessibility issue.
- Bounded by ../principles/inclusive.md principle; read ../patterns/inclusive-and-accessible-design.md, especially its entry on accounting for anxiety + emotional state.

## Related
- chunking.md: capacity counted in chunks, not words; shares mistyped codes + IDs fix.
- cognitive-load.md: closely tied to WM; shares value-holding question + fixes for error or payment failure + look-alike cards.
- selective-attention.md: WM load raises distraction while perceptual load reduces it.
- millers-law.md: seven claim; seven = reason to chunk, not limit + not design cap.
- doherty-threshold.md: refreshing data + 400 ms bound.
- peak-end-rule.md: payment failure as negative peak.
- teslers-law.md: system should carry state across Back.
- similarity.md: uniform cards correctly read as one content type.
- hicks-law.md: applied w/ Working Memory in search case.
- [Usability heuristics mapped to laws](../checklists/usability-heuristics-map.md): "Error prevention" relates to Postel's Law, Fitts's Law (spacing of destructive targets) + Working Memory; "Recognition rather than recall" relates to Working Memory, Miller's Law + Chunking; "Help users recognize, diagnose and recover from errors" relates to Peak-End Rule + Working Memory; classic heuristics date from 1990, revised 1994.
- [Mapping memory demands in a flow](../methods/mapping-memory-demands.md): where flow asks people to remember.
- ../patterns/inclusive-and-accessible-design.md: memory demands as accessibility issue (persona spectrum, accessibility floors).
- ../guides/laws-and-principles-crosswalk.md: humane principle bounding Working Memory.
- Pattern files applying Working Memory: ../patterns/navigation-and-menus.md, ../patterns/forms-and-data-entry.md, ../patterns/search-and-results.md, ../patterns/dashboards-and-data-displays.md, ../patterns/complexity-management.md, [AI, assistants and automated features](../patterns/ai-and-automated-features.md).
