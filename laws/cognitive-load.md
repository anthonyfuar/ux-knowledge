# Cognitive Load

## In one line
Cognitive load = interface's draw on person's thinking capacity, both from figuring it out + from operating it. Matters for: removing non-essentials, choosing defaults + data reuse, labeling icons.
- Type: construct (cognitive process/state), not effect. Parts: intrinsic + extraneous load. Aliases: none. Theme: Memory.
- Core rule: cut extraneous load: label icons, offer fewer choices, offload tasks, use common patterns, drop non-essentials.
- Load never reaches zero → manage it, do not try to eliminate it.

## Load types and terms
|Term|Meaning|Design handle|
|---|---|---|
|Intrinsic load|Effort of tracking goals, taking in anything new, carrying information goal calls for; inherent to task|Respect it: design cannot remove it, can split it|
|Extraneous load|Added by design, not task: effort buying no comprehension; typical source = purposeless elements or ones tugging attention elsewhere|Removable → cut it|
|Germane load|Effort on essential content + schema building; not independent load source|When extraneous load falls, freed resources flow to essential material|
|Schema|Organized knowledge unit letting many elements act as one|Established patterns speed schema building|
|Cognitive overload|Person's available capacity < what arriving information needs|Signs: abandonment, slowdown, feeling swamped, details slipping past, tasks getting harder|
|Split-attention effect (1990s load research)|Integrating information from separated sources adds load|Co-locate labels, inputs, help, data|
|Worked-example effect (1990s)|For novices, studying solved examples beats unaided problem solving|Give newcomers examples|
|Completion-problem effect (1990s)|Giving partly finished tasks to complete|Give newcomers prefilled starting states|
|Modality effect (1990s)|Related information split across seeing + hearing can ease load|Split it across both senses where it fits|
|Expertise reversal effect (1990s)|Aids helping novices burden experts|Make guidance dismissable; offer shortcuts|
|Time-based resource-sharing model (2004, 2007)|Load = share of time central attention stays busy (temporal density of attention)|Leave idle gaps|
|Relational complexity|Capacity = relation count person can handle at once; about 3 variables = practical ceiling|—|
|Digital amnesia|People expecting information to stay available encode it less deeply; consistent w/ transactive memory (remembering where information lives, not content)|Where learning matters, prompt recall|
|Desirable difficulty|Productive struggle worth keeping where learning/skill matters|Preserve it; do not offload it|

## Applies when / does not apply when
|Situation|Cite|Not|
|---|---|---|
|Screens w/ no choice to make (tour slides, sequential information)|Cognitive Load|Hick's Law: silent there|
|Many independent settings (burden = scanning + finding)|Cognitive Load (+ Selective Attention, Chunking, progressive disclosure, Tesler's Law)|Choice Overload: needs one choice among close substitutes; sixty separate toggles = scanning + finding load|
|Long filter / facet list|Cognitive Load|Choice Overload: multi-select facets not one pick among alternatives|
|Grid of look-alike cards hard to compare|Cognitive Load, Working Memory (comparing across cards)|Law of Similarity (uniform cards correctly read as one content type); Selective Attention|
|Splitting long form into steps|Chunking + Cognitive Load|Hick's Law only for choices within each step|

## Decision rules
Audit three causes first, by origin: what screen offers (excess options, missing clarity) · what it asks of person (excess thought demanded).

Load reducers, 7 in all, grouped by target (unranked):

|Acts on|Reducer|
|---|---|
|What users already recognize|Familiar patterns: prefer ones already in wide use|
||Icons = risk: word beside each, except small set virtually everyone decodes alike (see Hypothetical: icon needing a word)|
|Option set|Whole set in one view: never split part of it off into group out of sight|
||Low option counts; matters most in forms, drop-downs + navigation|
|What screen shows|Readable text, not merely legible|
||Cut whatever serves no need: imagery, surplus layouts, color, ornament|
|Work left to user|Shift needless work (memory, decisions, reading) off user: reuse data already given, anticipatory design, defaults user can edit|

If → then:
- If copy unclear → count as extraneous load, not intrinsic; fix it.
- If task itself complex → split into sub-parts done/learned separately, then combined.
- If task hardest → cut extraneous load hardest there.
- If simplicity + clarity conflict → clarity wins; never prize simplicity over clarity.
- If flow has several required actions → leave short pauses between them.
- If mid-task → never make users process irrelevant material (promotions, trivial confirmations).
- If key information newly shown → leave a few undisturbed seconds after it.
- If users must enter code → never make them hold one code while entering another: allow paste/autofill, or keep code visible.
- If adding drag, gestures, direct manipulation → only when processing benefit > motor + coordination cost; justify each interactive flourish by net benefit.
- If users may include stressed/low-income people → cut steps, jargon, decisions; leave headroom for invisible baseline load.
- If comparing design variants → compare outcome per unit of perceived effort, not success rate alone.
- If users newcomers → provide templates, examples, prefilled starting states.
- If users experts → make guidance dismissable + offer shortcuts (expertise reversal).
- If information sits in separated sources → co-locate labels, inputs, help, data (split attention).
- If offloading → offload routine effort; where learning/skill matters, prompt recall, not lookup, + preserve productive struggle (desirable difficulty).
- If many independent settings → apply Cognitive Load, Selective Attention, Chunking, progressive disclosure, Tesler's Law (relocate complexity).

## Why it works
Mechanism:
- Framing: load = working-memory capacity occupied at given moment.
- Overlooked details, weaker performance + frustration trace to one ceiling: working memory holds fixed amount; excess spills over.
- Fixed capacity → Hick's Law follows: more options + more complex options → longer processing + more load.
- One finite pool, two claims: visitor's purpose + decoding site's workings, restarting every visit (see Hypothetical: decoding a site while holding a goal).
- No element neutral: useless items get processed + held alongside useful ones → anything not serving goal competes w/ task.
- Established patterns aid schema building: people learn faster when mapping something new onto known pattern.
- Unaided novices default to means-ends analysis → eats capacity, leaves little for learning.
- Time-based resource sharing: memory traces refresh in small idle gaps → digit every 0.5 s loads memory more than one every 2 s.
- Same-kind material clashes most (holding one code while typing another); mixed kinds (numbers + spatial material) interfere far less.
- Users carry baseline load designer cannot see: noise, worry, anxiety, little web experience, financial scarcity → leave headroom.
- Icons, unexpectedly, often add load: no common icon vocabulary; outside a handful of glyphs nearly everyone reads alike, glyph meaning rests on icons each person met before. Decoding/recalling meaning costs effort + glyphs poorly kept in memory; word beside glyph removes guesswork.
- Unnoticed alternatives = price of splitting set + keeping part out of sight: people assume options in view = whole set.
- External tools (autocomplete, calculators, navigation, chatbots) cut load, but people expecting information to stay available encode it less deeply (digital amnesia). Easy information access can create illusion of knowledge.

Origin:
- Late 1980s: cognitive load theory takes shape; anchor = 1988 paper on why some material proves hard to learn + how teaching design bears on it.
- Core claim: teaching-material design can act as lever cutting learners' load.
- Twofold ancestry: largely extends information-processing ideas behind Miller's Law + grew out of problem-solving research. Tightly bound up w/ Miller's Law.
- Measure came only later: self-report rating of perceived mental effort.
- Relative condition efficiency (1993) = (standardized performance − standardized mental-effort rating) / square root of 2 → one efficiency score combining performance + effort.
- Three load types (intrinsic, extraneous, germane) first treated as additive; now thought to interact + overlap, not only add.

## Evidence
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Comparing 2 stimuli during retention hurt memory as much as holding 2 extra items → processing distractor forces it into memory|2013 study|—|Never make users process irrelevant material mid-task|
|Digit every 0.5 s loads memory more than one every 2 s|Time-based resource-sharing model, 2004 + 2007|Model|Leave short pauses + undisturbed seconds|
|Worked examples most efficient for learning, completion problems second, ahead of discovery practice (scored by combined performance + effort)|1993 instructional experiment|One 1993 comparison|Templates, examples, prefilled starting states for newcomers|
|Different load measures respond differently to intrinsic, extraneous, germane load|2008 study|—|—|
|Physiological signals (e.g. task-invoked pupil dilation) track load|Lab measures|Reliable in lab; mostly have not held up outside it|Do not rely on physiological signals outside lab|
|Overload degrades performance|Theory|Theoretical consequence of limited capacity, not measured study result|Cite as theory|
|Ordered (e.g. alphabetical) list speeds search|1985 menu research|Applies only to users knowing exact label|Pair long lists w/ type-ahead|
|Icons stick poorly in memory|Only unnamed research + general HCI finding|No specific study → cite as caution, not measured effect|Label icons|
|Popular claims about cognitive load in students/children|Various|Several rest on weak citations|Check sources before citing|
|Harms of cognitive offloading (media multitasking, deskilling after AI use)|Under active research|Treat as cautions, not settled effects|Keep load-bearing effort where skill matters|

## Misreadings and limits
- Wrong: more choices + features bring more satisfaction → Right: myth.
- Wrong: adding working-memory demands to make users "focus" (Selective Attention, Cognitive Load) → Right: loaded working memory increases distraction.
- Wrong: cutting clicks as goal, w/ fixed click budget (Cognitive Load, Hick's Law) → Right: extra steps cheap when each clearly signals path to goal (information scent, 1999 theory); measure per-step success + hesitation, not click count.
- Wrong: citing Hick's Law to size unordered menu → Right: unordered lists get scanned linearly; logarithmic benefit needs ordered list + known target.
- Wrong: citing Choice Overload for many independent settings → Right: Choice Overload needs one choice among close substitutes; sixty separate toggles = scanning + finding load.
- Wrong: simplifying until controls turn abstract → Right: complexity must live somewhere (Tesler's Law); clarity beats minimalism (Cognitive Load).
- Wrong: treating three load types as purely additive → Right: now thought to interact + overlap.
- Limit: load never reaches zero.

## Check questions
|Question|Look for|Laws|
|---|---|---|
|Can user finish each step w/o holding value (code, price, name) from another screen, or while scanning similar material?|Retyping code shown elsewhere; remembering one name while scanning similar names|Working Memory, Cognitive Load|
|Each step shows only needed, relevant information?|Anything self-animating; purely decorative ornament, imagery or color → each costs effort + clarifies nothing|Cognitive Load (extraneous)|
|Labels, explanations + data placed beside what they explain?|Legends, help text or definitions needing cross-reference across screen or pages|Cognitive Load (split attention)|
|Icons universal or labeled?|Custom glyphs w/o word; only the few glyphs nearly everyone decodes alike may stand alone|Cognitive Load|
|Every step light on choices, + drawn-out/intricate flow split across several steps?|One huge form or settings page|Chunking, Cognitive Load; Hick's Law only for choices within each step|
|All options in set shown together?|Visible options passing for whole set while rest sits in groups out of view|Cognitive Load|
|Every control exposes name + state to assistive technology?|Icon-only buttons w/o accessible name|Postel's Law, Cognitive Load|

## Symptoms → fixes
|Symptom|Likely cause|Fix|
|---|---|---|
|Abandonment, slowdown, users swamped, details slip past, tasks get harder|Cognitive overload|Audit three causes; apply seven reducers|
|Errors/payment failures spiral into abandonment|Working Memory, Cognitive Load|Keep problem, input + next step visible together; stress cuts capacity → simplify recovery most|
|Long filter/facet list slow to use|Cognitive Load (not Choice Overload)|Type-ahead within facet; grouped facets; recent/popular values pinned at top. Ordered list helps only users knowing exact label (1985 menu research)|
|Icons confuse|Cognitive Load|Word beside each icon outside small set nearly everyone decodes alike|
|Settings page w/ dozens of toggles hard to scan|Cognitive Load, Chunking, Common Region; Tesler's Law for progressive disclosure; Pareto Principle to verify usage w/ analytics; not Choice Overload|Task-based labeled groups; search over names, synonyms + descriptions; advanced settings behind disclosure|
|Field errors fire while user still types; valid fields get noisy checkmarks|Selective Attention through interruption, Cognitive Load; error-prevention heuristic|Validate on field exit or submit; once error shows, recheck live so it clears; keep valid fields quiet; move focus to first error or linked summary|
|Grid of look-alike cards hard to compare|Cognitive Load; Working Memory for comparing across cards (not Similarity, not Selective Attention)|Show deciding attributes (price, rating, key spec) consistently, + sort + filters|

## Hypothetical examples
- Hypothetical (element that serves no need): workplace-tool expense-report form shows decorative photo banner + rotating "tip of the day" panel beside fields; neither helps file claim, yet both get read + held as user hunts for amount box.
- Hypothetical (self-moving element pulls attention): pharmacy refill page runs scrolling ticker of health headlines next to dosage field; each movement drags eye away from prescription number user types.
- Hypothetical (decoding a site while holding a goal): patient opens clinic portal only to move appointment; while keeping new date in mind, must first work out where bookings live + what each menu leads to.
- Hypothetical (icon needing a word): home-thermostat app marks away schedule w/ custom suitcase-and-clock glyph; until word "Away" sits beside it, owners must guess what it does.

## Humane bound
Turned against people:
- Decision removed via default setting = decision made for person; default never neutral → enables self-serving defaults.
- Long, complex choice front-loaded so people give up + accept preselection.
- All friction removed for conversion, incl. load-bearing effort carrying deliberation, ownership + learning.

Bounded by:
- ../principles/intentional.md: choose defaults for well-being, withhold them where active choice matters, add friction on purpose.
- ../principles/inclusive.md: leave headroom for stressed, anxious + low-income users.

Read for this bound:
- ../patterns/defaults-and-choice-architecture.md: humane bounds on decision-removing defaults (opt-in, equal-weight decline).
- ../patterns/friction-undo-and-confirmation.md: deliberate pauses + undo.
- ../evidence/convenience-and-friction.md: evidence on what removing/adding friction does + effort worth keeping when offloading.

## Related
- working-memory.md: load = working-memory processing capacity in use at given moment; shares value-holding question + error-recovery + look-alike-cards fixes.
- chunking.md: shares split-long-flows question + settings-page fix.
- hicks-law.md: option count = load source.
- millers-law.md: tightly bound up; shared information-processing ancestry.
- selective-attention.md: settings pages, interruption by early validation, "focus" misreading.
- teslers-law.md: complexity must live somewhere; relocate it.
- common-region.md, pareto-principle.md: settings-page fix.
- choice-overload.md: when not to cite it.
- ../methods/lightening-mental-effort.md: step list for cutting extraneous load from screen/flow.
- ../checklists/usability-heuristics-map.md: heuristic "Aesthetic and minimalist design" maps to Aesthetic-Usability, Occam's Razor, Cognitive Load, Hick's Law; classic heuristics date from 1990, revised 1994.
- ../guides/laws-and-principles-crosswalk.md: humane principle bounding this law.
- Pattern files applying it: ../patterns/forms-and-data-entry.md, ../patterns/onboarding-and-first-use.md, ../patterns/search-and-results.md, ../patterns/layout-grouping-and-hierarchy.md, ../patterns/dashboards-and-data-displays.md, ../patterns/complexity-management.md, ../patterns/first-impressions-and-aesthetics.md, ../patterns/departing-from-convention.md.
