# Law misapplications

## Use when
- Before citing law in design / review / rationale → check citation fits.
- Each row: wrong use of law → why it fails + correction.

## How rows are filed
- Rows grouped by theme.
- Misapplication naming laws from two themes → filed under its first law's theme.
- `Also see` lines under theme point to such rows filed elsewhere.

|Theme|Laws|
|---|---|
|Perception + grouping|Gestalt laws (../laws/gestalt-principles-overview.md), ../laws/common-region.md, ../laws/proximity.md, ../laws/similarity.md|
|Memory + cognition|../laws/millers-law.md, ../laws/chunking.md, ../laws/working-memory.md, ../laws/cognitive-load.md|
|Attention|../laws/selective-attention.md, ../laws/von-restorff-effect.md, ../laws/zeigarnik-effect.md, ../laws/flow.md|
|Decisions|../laws/hicks-law.md, ../laws/choice-overload.md, ../laws/cognitive-bias.md, ../laws/occams-razor.md, ../laws/pareto-principle.md|
|Motor control + time|../laws/fittss-law.md, ../laws/doherty-threshold.md, ../laws/parkinsons-law.md, ../laws/goal-gradient-effect.md|
|Expectations + emotion|../laws/jakobs-law.md, ../laws/mental-model.md, ../laws/aesthetic-usability-effect.md, ../laws/peak-end-rule.md|
|Complexity + robustness|../laws/teslers-law.md, ../laws/postels-law.md, ../laws/paradox-of-the-active-user.md|
|Cross-cutting|all laws (../laws/index.md)|

## Perception + grouping
|Law|Wrong use|Why it fails → correction|
|---|---|---|
|Gestalt laws|rank grouping cues by fixed strength (e.g. 'connectedness always wins')|rankings come from demonstrations; winner depends on cue magnitude → make cues agree + test|
|Common Region|add borders + cards 'just in case'|extra containers = more visual processing → check spacing first|
|Proximity, Common Region|remove containers w/o adding space|enclosure + whitespace trade off → widen gaps between groups|
|Similarity|vary tile size to show importance, w/ no other cue|size variation blurs whether items still same type → add labels / affordances|

## Memory + cognition
Also see:
- 'Adding working-memory demands to make users focus', filed under Attention, also belongs here (names Cognitive Load).
- 'Hick's Law cited for navigation', filed under Decisions; correction → ../laws/serial-position-effect.md + Chunking (this theme).
- 'Hick's Law cited for sequential informational screens', filed under Decisions; correction → Cognitive Load (this theme).

|Law|Wrong use|Why it fails → correction|
|---|---|---|
|Miller's Law|cap menus, results, dropdowns, slides / radio groups at five to seven items 'because of Miller's Law'|2000 source called this cap superstition; on-screen options recognized, not memorized → seven = reason to chunk, not limit; ~five results per page only adds paging + comparison work|
|Chunking|chunk / paginate content users scan / compare|→ chunk what users memorize + transfer; keep comparable items together|
|Chunking|assume expert-level density + groupings help novices|chunks work only if user already knows pattern → progressive disclosure / modes|
|Working Memory|assume everything-visible dashboard low-load since nothing to remember|more than ~3 interacting variables overload working memory (WM) even w/ all data visible → pre-compute comparisons|
|↑|judge flow easy because team finds it easy|teams have above-average WM → test w/ representative, older + less experienced users|
|↑|read inattentive / 'careless' behaviour as low motivation|seemingly careless behaviour often = WM overflow → externalize state + instructions|
|Cognitive Load, Hick's Law|treat fewer clicks as goal (fixed click budget)|extra steps cheap when each clearly signals path to goal (information scent, term from 1999 work) → measure per-step success + hesitation, not click count|
|Cognitive Load|give up clarity for simplicity|→ clarity wins|
|↑|hide part of option set|users take whatever options stay in view for all available options|

## Attention
|Law|Wrong use|Why it fails → correction|
|---|---|---|
|Selective Attention, Cognitive Load|add WM demands to make users 'focus'|loaded WM increases distraction|
|Selective Attention, Von Restorff Effect|assume bigger, bolder / differently styled element gets noticed|element outside user's focus region, or ad-styled, often ignored → place it in reading path|
|Selective Attention|judge salience from designer's own view|designers already know where to look + what changed → test salience w/ real users|
|↑|ship several changes at once|they compete + go unnoticed|
|↑|style content like ads|gets filtered out|
|Von Restorff Effect|emphasize many things|standouts cancel each other out + can read as ads|
|↑|assume highlighted item remembered|highlighting draws eye but does not guarantee memory encoding → state why item matters + tie it to task|
|↑|use colour / motion as only contrast|excludes people w/ low vision, colour vision deficiency / motion sensitivity|
|Zeigarnik Effect|completion meters / cliffhangers w/ no way to close them|open loops cost rehearsal effort + rumination → let people finish, dismiss / resume|
|↑|cite it for checklist starting w/ steps already credited (head start)|head start works via perceived nearness to goal (endowed progress, Goal-Gradient Effect); Zeigarnik Effect = memory for interrupted tasks → fits checklist started + left, not head start|
|Flow|call endless scroll / long sessions 'flow'|flow serves user's own goal; compulsive time-on-site = hyperfocus / capture, not flow|

## Decisions
Also see:
- 'Cutting clicks as the goal', filed under Memory + cognition, also names Hick's Law.

|Law|Wrong use|Why it fails → correction|
|---|---|---|
|Hick's Law, Tesler's Law|simplify until controls become abstract|→ keep controls' meaning; complexity has to go somewhere|
|Hick's Law|cite it to set unordered menu's length|unordered lists scanned linearly; Hick's Law applies only to ordered lists where user knows target|
|Hick's Law|cite it for navigation w/o checking item order + whether users know their target|→ model navigation as linear scanning; reduce, group + order items; cite Serial Position Effect / Chunking for placement|
|Hick's Law|cite it for sequential informational screens w/ no choices (tour slides, intro carousels)|Hick's Law = decision time among options; nothing to choose → cite Cognitive Load (attention spent before any value arrives) + Paradox of the Active User|
|Hick's Law|treat recommended option as license to hide essentials|→ recommend, do not conceal|
|Choice Overload|remove options users need to compare|→ side-by-side comparison, filters / search|
|↑|cite jam study as universal law|one field study; choice overload needs close substitutes, no prior preference, no dominant option + low expertise → replicate in own context before relying on it|
|↑|ask users whether they want more options|large option sets appeal in abstract but perform worse in use → measure behaviour instead of asking|
|Cognitive Bias|assume bias awareness removes it|awareness only improves odds of catching it|
|↑|expect averaged judgments to cancel bias|systematic errors point one way + survive averaging|
|Cognitive Bias (framing)|report percentages from 20-user tests|→ report small-test results as counts w/ confidence intervals; flip frame to check reading|
|Occam's Razor|cut elements until function breaks|→ remove only what keeps full function intact|
|↑|prefer simpler option even though it performs worse|parsimony applies only when alternatives perform equally|
|Pareto Principle|treat 80/20 as exact / universal|approximate lens for uneven systems|
|↑|read 'trivial many' as worthless|label 'trivial many' later revised to 'useful many' → keep capacity for long tail|
|↑|run Pareto analysis on a handful of data points|small samples mislead → weight counts by value|

## Motor control + time
Also see:
- 'Zeigarnik Effect cited for a pre-credited checklist head start', filed under Attention, also names Goal-Gradient Effect.

|Law|Wrong use|Why it fails → correction|
|---|---|---|
|Fitts's Law|enlarge target while ignoring spacing + reach|size, spacing + placement all matter|
|Fitts's Law|make buttons ever larger|returns diminish; oversized buttons stop reading as buttons|
|Fitts's Law|treat screen corners + edges as fast targets on touch|edge targets slower on touch; edge shortcut holds only for mouse-like pointing devices|
|Fitts's Law|cite it as proof layout usable|predicts movement time only, not search, decision / comprehension|
|Fitts's Law, Jakob's Law|hide unavailable controls|hidden controls break learned positions → disable them w/ explanation|
|Fitts's Law|cite it for slips between two close buttons|models movement time from distance + size; wrong-target slips = error prevention + spacing, w/ Fitts's Law at most supporting argument for larger, separated targets|
|Doherty Threshold|assume faster always better|trust can go up w/ deliberate pause, but honesty applies to such pauses|
|↑|cite universal '2-second rule'|1968 response-time work set different limits per interaction level, from 0.1 s to minutes, not one universal limit|
|↑|tag every timing as Doherty Threshold, e.g. pressed state 'under 100 ms'|0.1 s, 1 s + 10 s = separate response-time limits (from 1968 work + separate three-limit scheme); Doherty Threshold = 400 ms system-response threshold|
|Doherty Threshold (or any time law)|cite it for disabling button to prevent double charges|button disabling = error prevention + idempotency → cite error-prevention heuristic (../checklists/usability-heuristics-map.md)|
|Doherty Threshold|animate progress bar on timer|hides hangs → bar should stop when work stops|
|Parkinson's Law, Goal-Gradient Effect|present time-to-value target (e.g. 'first result within 2 minutes') as established|no research figure supports universal target → derive it from own cohort data + label it hypothesis|
|Parkinson's Law|cite it as experimental finding|began as line in humorous 1955 essay drawing on British Civil Service|
|Goal-Gradient Effect|treat it as supported by animal studies only|controlled human field evidence from 2006 (café stamp cards + online rating program), but w/ real rewards; no-reward control slowed; customers accelerating more = more likely to return|

## Expectations + emotion
Also see:
- 'Hiding unavailable controls', filed under Motor control + time, also names Jakob's Law.

|Law|Wrong use|Why it fails → correction|
|---|---|---|
|Jakob's Law|copy widespread deceptive / slow pattern + cite Jakob's Law to justify it|convention transfers learning, not approval → keep familiar structure, not known dark pattern / failure|
|Jakob's Law|novelty w/o purpose / testing|→ default to convention; test novel patterns|
|Jakob's Law|judge novel pattern on first-use performance|→ compare learning curves + plateaus over repetitions|
|Jakob's Law|force abrupt redesign|→ offer temporary opt-in + way to revert|
|Mental Model, Jakob's Law|take familiar design's preference win as proof of quality|mere exposure inflates liking → separate preference from performance|
|Mental Model|assume designers' models match users'|→ research where models diverge|
|Aesthetic-Usability Effect|read good ratings of polished UI as usability|perception inflated → measure task success|
|↑|rate polished product on one global score|halo spreads one impression across attributes → rate attributes separately|
|↑|expect aesthetic goodwill to cover serious problems|forgives minor issues only; product where people cannot find things earns nothing from it; users mind feature they cannot find far more than poor kerning (stated in 2015 source)|
|↑|design, review / approve w/ ideal placeholder content|→ stress-test w/ longest, shortest + ugliest real data, w/ sparse data (e.g. recommendation feature before data exists to power it) + on low-end devices; separate execution quality from product viability when judging design|
|Peak-End Rule|average satisfaction across journey|peaks + endings dominate memory, negative ones most|
|↑|treat Skip tap / dismissed tour as 'end' of experience|episode continues into product after tour → onboarding lever = designed first success + clean ending of real task|
|↑|claim 'only the peak and the end matter'|peak-end pattern = rough tendency; day-long episodes, some VR content + some groups do not follow it; single most memorable moment can predict remembered experience better than peak + end|
|Peak-End Rule (duration neglect)|shorten mediocre flow + expect better memory of it|duration barely affects remembered value → improve worst moment + ending instead|
|Peak-End Rule|pad / prolong bad experience to improve its memory|nicer memory does not justify added real cost → fix worst moment + ending|

## Complexity + robustness
Also see:
- 'Simplifying until controls become abstract', filed under Decisions, also names Tesler's Law.
- 'Hick's Law cited for sequential informational screens', filed under Decisions; correction → Paradox of the Active User (this theme).

|Law|Wrong use|Why it fails → correction|
|---|---|---|
|Tesler's Law, Paradox of the Active User|design for rational user|→ design for real, irrational behaviour|
|Tesler's Law|equate 'looks simple' w/ 'easy to use' by removing controls|fewer visible controls can mean longer hidden sequences + memorized gestures → judge operational simplicity; keep capability experts need|
|Tesler's Law|remove all effort from high-stakes actions|instant, invisible completion of high-stakes action can feel unsafe / broken → keep meaningful participation + visible work|
|Tesler's Law|call burden irreducible so users keep carrying it|→ list irreducible core first; then check whether system could hold each piece (defaults, reuse, automation) before assigning it to user|
|Tesler's Law|ship automation w/o failure path|→ design automation's breakdown, diagnosis + handover; limit uninterrupted automation so people's skills stay current|
|Tesler's Law|expect simplification to cut users' total burden|after simplification users may take on harder tasks → total burden need not fall|
|Postel's Law|silently accept ambiguous input|→ lenient w/ input only when meaning unambiguous; set limits + give feedback|
|Postel's Law|apply its leniency inside system too|internal leniency hides defects + attackers can exploit it → liberal at human-facing edge, strict + validating toward downstream systems|
|Paradox of the Active User|front-load tours + manuals|→ contextual, always-available guidance|

## Cross-cutting: all laws
|Law|Wrong use|Why it fails → correction|
|---|---|---|
|All laws|apply laws as rules w/o research|they = heuristics → data decides|

## Hypothetical examples
- Hypothetical (Hick's Law cited w/o checking order / target knowledge): hospital intranet's top bar lists every department in no set order; team cites Hick's Law to defend its length w/o asking whether links ordered / whether staff know their target department.

## Related
- common-mistakes.md: most damaging misuses of this knowledge, usability + humane sides.
- defend-a-decision.md: rationale w/ law, origin year, mechanism, evidence + metric.
- ../laws/index.md: all 30 UX laws by theme w/ core idea, design rule + decision matrix.
- ../evidence/citation-caveats.md: contested numbers, misattributions + limits of each evidence body.
- ../methods/thresholds-and-formulas.md: each law's measurable form: response-time limits, target sizes, formulas.
- ../checklists/usability-heuristics-map.md: classic heuristics mapped to laws, used when no law explains problem (e.g. error prevention).
- ../ethics/using-psychology-responsibly.md: humane-design guardrails for every psychological lever.
- laws-and-principles-crosswalk.md: humane principle bounding each law.
