# UX laws index

## How to use this index
- 30 psychology-based UX laws, grouped by theme; each has own file: aliases, type, definition, rules, origin, mechanism, examples, related laws + pitfalls.
- Per law: origin (dated), core idea (one-line rule), design rule (what to do + scope caveats: when it applies, when not), interface decisions most affected (decision matrix by theme).
- Laws listed as related to given law share mechanism w/ it.
- UX law = heuristic informing decisions, never mandate.
- User research + project data outrank any UX law.
- Steps: 1. Find decision's theme → 2. pick law whose "Decisions most affected" matches → 3. check its scope caveat here → 4. open law's own file → 5. before citing, check ../guides/law-misapplications.md.

## Two families
|Family|Meaning|Laws|Role|
|---|---|---|---|
|Construct|Cognitive process/state|7: chunking.md, cognitive-bias.md, cognitive-load.md, flow.md, mental-model.md, selective-attention.md, working-memory.md|Explains|
|Effect or principle|Describes/predicts behavior|Other 23|Predicts/prescribes|

## Seven themes
|Short label|Theme|Laws|
|---|---|---|
|Perception|Perception and grouping|five|
|Memory|Memory and cognition|five|
|Attention|Attention and salience|four|
|Decisions|Decisions and simplicity|five|
|Motor/time|Motor control and time|four|
|Expectations|Expectations and emotion|four|
|Complexity|Complexity and robustness|three|

## Perception
Five laws: Common Region, Prägnanz, Proximity, Similarity, Uniform Connectedness = Gestalt psychologists' grouping laws. Proximity + Similarity formalized 1923; Common Region added 1992; Uniform Connectedness 1994. Shared background (Gestalt school, how cues combine + compete): [Gestalt grouping principles overview](gestalt-principles-overview.md).

|Law|Core idea|Design rule + scope|Origin|Decisions most affected|
|---|---|---|---|---|
|common-region.md|Items inside one bounded area (shared boundary) read as group|Border or background fill around related elements|1992, Gestalt grouping tradition|Card + panel containers; section backgrounds; form-field grouping|
|[Law of Prägnanz](pragnanz.md)|Least effort wins: complex image, or one open to several readings, seen in plainest version|Simple shapes + compositions; viewers make one form out of complex visuals|1910, from observing railroad-crossing lights|Icon + logo simplicity; shape clarity; less visual noise in complex figures|
|proximity.md|Objects close together read as one group w/ shared function|Tight gaps within groups, larger between; spacing always means something|1923, Gestalt grouping principles|Spacing scale between vs within groups; label-to-field distance; gaps between list items|
|similarity.md|Shared appearance ties items into one group; gaps between them do not break it|Body text one look; links + navigation another look users cannot confuse w/ it; audit accidental resemblance|1923, Gestalt grouping principles|Link + button styling vs body text; consistent component styling; accidental lookalikes|
|uniform-connectedness.md|Visible link between elements makes them seem more strongly related|Lines, arrows, frames + shared color link related functions; border also raises priority → reserve it|1994, first described as element connectedness|Borders on priority items; connector lines in steppers + diagrams; linking related controls|

## Memory
Five laws: Miller's Law, Working Memory, Chunking, Cognitive Load, Serial Position Effect.

|Law|Core idea|Design rule + scope|Origin|Decisions most affected|
|---|---|---|---|---|
|millers-law.md|About 7 ± 2 (plus or minus 2) items fit in working memory; later research argues number nearer 4|Chunk information; never cap menus/lists at seven items|1956|Chunk sizes; refusing arbitrary "seven item" caps; formatting long strings|
|working-memory.md|Small, fast-decaying mental workspace holding few chunks (4–7), each fading after about 20–30 s|Plan for about 4 new chunks at once (2001 estimate); 4-7 = broad working range. Prefer recognition over recall; keep inputs, visited states, breadcrumbs + comparisons visible|Term coined in 1960s; applied in 1968 memory research|Persisting input across screens; visited states + breadcrumbs; comparison tables|
|chunking.md|Meaningful units assembled from separate bits of information|Modules, dividers, headings, sensible line length, formatted strings (e.g. phone numbers). Scope: visual grouping aids scanning; splitting into memory-sized pieces matters only for what users must hold + retype. Visible navigation scanned, not memorized → no memory-based argument for chunking it|1956 paper on how much people can tell apart + recall at once|Content modules + dividers; headings + line length; input formatting (phone + card numbers)|
|cognitive-load.md|Demand UI places on person's thinking capacity, both to operate it + to make sense of it; parts: intrinsic + extraneous|Cut extraneous load: label icons, fewer choices, offload tasks, common patterns, drop non-essentials|Late 1980s; key publication 1988|Removing non-essentials; defaults + data reuse; labeling icons|
|serial-position-effect.md|First (primacy) + last (recency) items in sequence remembered best|Anchor 1-2 key items at ends of navigation/lists, least important in middle, rest ordered by task frequency or known key. Scope: recall effect for items met once in order (spoken menus, onboarding steps), not scanning rule for visible navigation|Term coined 1885|Order of items met once (spoken menus, onboarding, lists read before deciding); a few anchor items at bar ends|

## Attention
Four laws: Selective Attention, Von Restorff Effect, Zeigarnik Effect, Flow.

|Law|Core idea|Design rule + scope|Origin|Decisions most affected|
|---|---|---|---|---|
|selective-attention.md|Stimuli relevant to person's goal get attention; rest filtered out|Never give content ad-like styling or place it in ad zones; signal important changes w/ strong cues, one at a time|Research from 1953, 1958, 1960, 1963, 1973|Separating content from ads; signaling state changes; avoiding simultaneous changes|
|von-restorff-effect.md (Isolation Effect)|Item differing from similar items around it gets remembered|One distinct key action per area = practical default, not research rule (original study measured recall). Never make item distinct by color or motion alone|1933 study|Emphasis of primary action; limiting highlights; contrast beyond color + motion|
|zeigarnik-effect.md|Memory favors tasks interrupted or left unfinished|Signal more content exists + show clear progress = design takeaway (study measured recall only). Make started-and-left tasks easy to resume. Ovsiankina effect = urge to resume interrupted task, distinct from Zeigarnik (recall). Head start toward goal = endowed progress, different mechanism → cite goal-gradient-effect.md|1920s memory study, published 1927|Progress indicators; signifiers of more content; head start built from real completed steps (endowed progress: Goal-Gradient mechanism)|
|flow.md|Full absorption (enjoyment, total engagement, concentration charged w/ energy) when challenge matches skill|Discoverable features, friction removed, feedback for every action, challenge matched to skill|Term coined 1975|Scaling difficulty to skill; feedback on actions; removing friction + improving discoverability|

## Decisions
Five laws: Hick's Law, Choice Overload, Cognitive Bias, Occam's Razor, Pareto Principle.

|Law|Core idea|Design rule + scope|Origin|Decisions most affected|
|---|---|---|---|---|
|hicks-law.md (Hick-Hyman Law)|More choices + more complex choices → longer deciding; RT = a + b log2(n)|Recommend one option; split long choice sequences into steps; cut options where speed matters; stop before options turn abstract. Scope: only choice among options, not informational screens. Splitting data-entry form into steps = Chunking + Cognitive Load, not Hick's Law. Logarithmic benefit holds only for ordered list + known target = extension from 1985 menu research, not result of original lamp experiments|Work in 1952 + 1953; original 1952 experiments used lamps|Options per step; recommended defaults; progressive onboarding|
|choice-overload.md (overchoice)|Large option sets overwhelm people + sour whole experience|Feature one item; offer search + filters, side-by-side comparison; keep related options together. Scope: only picking one among alternatives, not many independent settings/toggles|Term overchoice coined in 1970 book|Search + filters; featured items; pricing compared in adjacent columns|
|cognitive-bias.md|Systematic, often unconscious judgment errors from mental shortcuts|Design around biases to protect users; watch for confirmation + complexity bias in team|1972 work|Framing of choices; guarding team decisions (confirmation, complexity bias); moments biased by memory|
|occams-razor.md|Assumption count = tie-breaker: hypotheses (or options) level on predictive power → prefer leanest in assumptions|Unfinished while any element still removable; first cuts = parts w/o function; baseline = simplest solution|—|Removing elements one by one; simplest solution as point of departure; critique process|
|pareto-principle.md (80/20)|Small share of causes (~20%) accounts for most effects (~80%)|Invest first where most users gain most; treat 80/20 split as approximate|1896-97 observation: 20% of Italy's population held 80% of its land|Prioritizing features + bugs; highest-impact flows; focusing research|

## Motor/time
Four laws: Fitts's Law, Doherty Threshold, Parkinson's Law, Goal-Gradient Effect.

|Law|Core idea|Design rule + scope|Origin|Decisions most affected|
|---|---|---|---|---|
|fittss-law.md|Target distance + size set time to hit it; movement time rises w/ distance, falls w/ target size|Targets near task focus, within easy reach, well spaced, large. Scope: touch screens have no reliable thumb-zone map; reach centre-first, edges slower (Mouse-era row in ../guides/symptom-to-fix-index.md). Size floors = standards, not Fitts's Law predictions: 24 × 24 CSS px minimum (WCAG 2.2 AA), 44 × 44 pt on iOS, 48 × 48 dp on Android. Slips onto adjacent button = mainly error prevention + spacing, not mainly Fitts's Law|1954 work measuring how much information movement control can handle|Touch target size; target spacing; placement near task focus + within reach|
|doherty-threshold.md|System answers inside 400 ms (old bar 2,000 ms) → exchange runs w/o idle time on human or machine side → steep productivity gain|Respond under 400 ms; slower work → skeleton, inline cue or real progress bar. Scope: only 400 ms limit = Doherty Threshold; direct-manipulation feedback (pressed state, echo) under 0.1 s + 1 s and 10 s limits = separate attention limits (../methods/thresholds-and-formulas.md)|1982 paper arguing for sub-second response; popular 400 ms threshold replacing 2,000 ms standard attributed to it|Response-time budget under 400 ms; loading animations + progress bars; perceived performance|
|parkinsons-law.md|Task (work) expands to fill time allotted to it|Beat expected duration w/ autofill, data reuse, short purchase + booking flows. Scope: lens from humorous essay (users judge speed against expected duration), not research finding. Steps removed via stored data → cite teslers-law.md first|Humorous 1955 essay, collected in essay book published in London 1958, drawn from British Civil Service|Autofill; flow length vs expected duration; time-saving shortcuts in checkout + booking|
|goal-gradient-effect.md|Nearer goal → stronger motivation; effort rises as goal nears|Show steps remaining; small truthful head start (endowed progress); explain each step during waits. Scope: progress display = design takeaway; human evidence shows acceleration toward real rewards → verify w/ step drop-off data|Hypothesis 1932; tested w/ rats in alley 1934; later consumer research showed purchase acceleration + illusionary progress|Progress bars + step counters; head starts in loyalty programs + onboarding; step visibility during waits|

## Expectations
Four laws: Jakob's Law, Mental Model, Aesthetic-Usability Effect, Peak-End Rule.

|Law|Core idea|Design rule + scope|Origin|Decisions most affected|
|---|---|---|---|---|
|jakobs-law.md|Your product = lesser share of anyone's usage → products people already use set their expectations of yours|Follow conventions by default; novelty only for stated purpose, researched + tested; make redesigns opt-in|Stated 2000|Platform conventions; opt-in rollout of redesigns; deliberate, tested novelty|
|mental-model.md|People act on compressed internal model predicting how system behaves|Design to users' models, not team's; narrow mismatch w/ empathy, journey maps, personas, interviews|Concept from 1943 book|Domain conventions (Hypothetical: library site's search → hold → pickup sequence); research to align models; managing discordance a redesign causes|
|aesthetic-usability-effect.md|Good-looking design judged easier to use|Polish, but measure task success apart from ratings; in tests, problems stay hidden behind polish|1995 study, 26 ATM interface variants, 252 participants|Visual-polish investment; usability test design + interpretation; tolerance of minor flaws|
|peak-end-rule.md|Experience judged not by its average but by its end + most intense moment (peak); cite both halves|Design peaks + endings deliberately; plan negative peaks (waits, errors, 404s, payment declines). Scope: peak = most intense moment of either valence, not "worst" moment. Explains remembered judgment + return, not abandonment mid-experience|1993 study|Confirmation + success screens; wait-state design; error + 404 fallbacks|

## Complexity
Three laws: Tesler's Law, Postel's Law, Paradox of the Active User.

|Law|Core idea|Design rule + scope|Origin|Decisions most affected|
|---|---|---|---|---|
|teslers-law.md (Conservation of Complexity)|Every system holds irreducible complexity that can only be moved, never removed|Let system carry complexity: defaults, suggestions, data reuse, automation, progressive disclosure|Mid-1980s|Complexity carrier (system or user); smart defaults + automation; progressive disclosure|
|postels-law.md (Robustness Principle)|Strictness for what goes out (sent/emitted), leniency for what comes in|Clear feedback + bounds; accept + normalize varied input when meaning clear|1979-80, first stated for TCP (TCP robustness principle)|Validation bounds + feedback; input parsing + normalization; accessibility across access methods|
|paradox-of-the-active-user.md|People use software straight away + leave manuals unopened|Contextual help + progressive onboarding, not front-loaded tours|1987 studies|Contextual tooltips vs tours; progressive onboarding; getting-started checklists people can revisit|

## Related
- ../guides/symptom-to-fix-index.md: from observed usability problem to law explaining it + fix.
- ../guides/law-misapplications.md: wrong uses of each law w/ correction; check before citing.
- ../methods/thresholds-and-formulas.md: measurable form of each law (response-time limits, target sizes, formulas).
- ../checklists/usability-review.md: yes/no questions by theme, each tied to a law.
- ../guides/laws-and-principles-crosswalk.md: humane principle bounding each law.
- ../ethics/using-psychology-responsibly.md: guardrails for every psychological lever laws describe.
- [Principles index](../principles/index.md): seven humane-design principles = other half of knowledge; they bound how laws get used.
- [Gestalt grouping principles overview](gestalt-principles-overview.md): background of five perception laws.
