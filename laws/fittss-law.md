# Fitts's Law

## In one line
Acquisition time (move to + hit target) rises w/ distance, falls w/ size; both together set it. → Targets: near task focus, in easy reach, well spaced, large.

- Theme: Motor/time. Classed as effect / principle.
- Bites hardest on: target clearance from neighbours, placement (near task focus, in reach), drawn touch-target size.
- Spelling: also w/ apostrophe only (no final s).
- Form = one relation, many equations: movement time tied to distance + size = common core of every version.

## Applies when / does not apply when

|Situation|Fitts's Law?|Cite instead / also|
|---|---|---|
|Sizing, spacing, placing buttons + touch targets|Yes|Platform / accessibility floors (standards)|
|Porting mouse-era layout to touch|Yes, w/ touch limits (no persistent cursor)|Touch field evidence below|
|Comparing pointing devices / layouts|Yes, via accuracy-adjusted throughput|ISO 9241-9|
|Separating destructive controls|Yes (destructive-target spacing)|Error-prevention heuristic|
|Wrong-button slips between 2 adjacent buttons|At most supporting argument; mainly error prevention + spacing|↑|
|Never-found control (Save at end of long scroll, off-screen action)|No: assumes visible, already located target|selective-attention.md + visibility-of-system-status heuristic|
|Finding target, deciding, understanding label|No: movement time only|hicks-law.md for deciding step|
|Idempotent submit, undo, soft delete, constraints|Many such fixes need no law|Heuristic alone, not borrowed timing / motor law|
|Eye tracking|Contested (2011 analysis): eye effectively blind during saccades|Cite only as contested|
|Minimum target size|No: floors set by standards, not predicted; model has no size threshold|WCAG, iOS, Android floors|

## Decision rules

### 1. Meet the floor, then size by position + use
|Platform|Floor|
|---|---|
|Web, WCAG 2.2 level AA|24 × 24 CSS px, or equivalent spacing around smaller target|
|Web, enhanced|44 × 44 CSS px|
|iOS|44 × 44 pt|
|Android|48 × 48 dp|

- First meet platform / accessibility floor → then size each target by position + how often used.
- Positional touch figures (~7 mm centre vs ~12 mm corners) = add-on to floor, never instead.
- Beyond floors, size relatively: frequent / critical targets → larger, nearer current focus, more spacing, in easy-reach zones.
- Touch-target test: wide clear margin to next target; easy reach; sized so fingertip lands on it w/o missing.
- Set touch size by screen position, in physical units (mm); whole visible element clickable.
- If invisible padding enlarges hit area → users still slow to aim at visible shape → target must look as big as it acts.
- If target = 2D rectangle → smaller of width / height = adequate stand-in for target width; wide but very thin target stays hard to hit.

### 2. Place for the task
- Task's button near where person already works + looks.
- If touch → no reliable thumb-zone map: never design to single one; centre-first layout; treat edge targets as slower.
- Never port mouse-era edge + corner shortcuts to touch.
- Screen corners: pointing research = fastest pixels to acquire; one web-design view = least valuable pixels (usually far from cursor). Both can hold at once → weigh distance vs precision.

### 3. Decide the control, not just its size
3 decisions beyond size + distance: whether control exists, type, placement.
- Type sets affordance: slider → continuous range w/ known limits; switch → binary state.
- Hero control (most used, most important or most drastic on screen) → spatial + visual prominence, even if rarely used.

### 4. Separate danger, map sides consistently
- Irreversible 'ejector-seat' actions → away from positive actions. OK directly beside Cancel = risky.
- Simon effect → confirm + dismiss on prompt's side (or its subject's); left / right mappings consistent.

### 5. Compare devices or layouts properly
- Model: movement time linear in index of difficulty, MT = a + b × ID; constants a, b regression-fitted per device. HCI form: ID = log2(D/W + 1).
- No single formula: never quote one variant as definitive.
- Compare by accuracy-adjusted throughput (bits/s), w/ effective width (We) from actual hit-point spread.
- Count misses, else aggressive users look falsely fast.
- Fitting method for a, b contested; chosen method can create differences > real device differences.

### 6. Cite with care
- Never sole design justification; never stand-alone UX metric.

## Why it works

Mechanism:
- Farther + smaller targets need more time + precision; rushing → more misses. Slowest = small + far.
- Speed-accuracy trade-off in aimed movement: error rate climbs when movement quick + target small.
- Two-phase aimed movement: fast coarse ballistic phase (set mainly by distance) → slow corrective homing phase (set mainly by target size). Small targets stretch homing.
- Longer distance → higher peak speed → distance costs time logarithmically: twice as far takes longer, not twice as long.
- Hard stop behind target (screen edge under mouse cursor) removes most homing.
- Information-transmission view: distance (D) = signal, target width (W) = noise. ID depends only on D/W.
- Touch: capacitive screens reduce finger contact to one centroid → accuracy driven by tap scatter + sensor error (worse near edges), not finger size.
- Simon effect: responses faster + more accurate when prompt on same side as answering control, even when position irrelevant to task.

Origin, dated:
|When|What|
|---|---|
|1899|Two-component aimed-movement model (ballistic + homing) underlying law|
|1954|Lab experiment: aimed movements of varying length analysed in information terms = law's origin|
|1956, 1964|Effective-width idea; later codified in ISO 9241-9|
|1978|Pointing-device comparison = law's first HCI application|
|1992|HCI index of difficulty ID = log2(D/W + 1), by analogy w/ Shannon-Hartley theorem; became HCI standard, later adopted in ISO 9241|
|1992|Extension to 2D rectangular targets|
|2002|Crossing-based interfaces, alongside steering law|
|2016|Temporal pointing|
|2017, 2022|Touch field research → positional touch-target sizing + centre-first touch hierarchy|

Neighbouring pointing concepts:
- Steering law: movement time through constrained paths, e.g. cascading menus.
- Crossing-based interfaces: pointing concept from 2002 work alongside steering law.
- Temporal pointing (2016): error rates for targets available only within time window.

## Evidence

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Farther target → longer; larger target → less time|1954 experiment|Origin study; original task 1D|Frequent targets closer + larger|
|Mouse beat rate-controlled isometric joystick, step keys + text keys for text selection, by law's index of performance|1978 lab pointing-device comparison|First HCI application; credited as major factor in Xerox's commercial mouse introduction|Compare input methods by throughput|
|Smaller of width + height = adequate stand-in for target width on 2D rectangles|1992 extension of law to 2D|"Adequate" stand-in|Never rely on width alone|
|Law applied to eye tracking|2011 analysis|Contested: eye effectively blind during saccades|Gaze targets: cite only as contested|
|Touchscreen edge targets slower, not faster|2015 HCI conference experiment|Likely bc finger overshoots physical edge, unlike cursor|No edge / corner shortcuts on touch|
|More than 1,300 phone users watched in public, several countries, + 651 further observations|2017 large observational field study + literature review|Field observation|Basis for next row's grip figures|
|75% touched screen w/ one thumb only; < 50% held phone one-handed; 36% cradled (one hand holds, other reaches); 10% held in one hand + tapped w/ finger of other|Same 2017 field study|Grips vary between people + shift constantly; people cannot reliably self-report grip|Do not design to one grip / one thumb-zone map; observe grip, not self-report|
|Taps most accurate at screen centre; targets ~7 mm at centre vs ~12 mm in corners cover 95% of taps|Field observation reported 2017 (scrolling-screen centre)|"About" figures; positional, not floor|Size by position, on top of floors|
|Touch field data repeatable but fit no formula neatly|Touch field research|Guidance by screen position, not as slope|Touch guidance per position|
|Touch field research revised own 2013 findings after more research|Touch field research, self-revision|Older columns: never cite|Cite revised figures, not 2013 ones|
|34% sales lift from moving add-to-cart control (2010), often repeated|Single-vendor anecdote, testing-tool company|Weak evidence|Never cite as proof|
|Constants a, b differ by fitting method|Methodological debate|Contested; method can create differences > real device differences|Device difference may come from fitting method, not devices|

## Misreadings and limits
- Wrong: enlarge target, ignore spacing + reach. → Right: size, spacing + placement all matter; size alone not enough.
- Wrong: keep making buttons larger. → Right: sharply diminishing returns once target reasonably sized; oversized buttons stop reading as buttons, people aim at inner icon / label, eroding size gain.
- Wrong: corners + edges = fast targets on touch. → Right: edge targets slower on touch; edge / corner shortcut holds only for mouse-like pointing devices.
- Wrong: cite law as proof layout usable. → Right: predicts movement time only, not search, decision or comprehension.
- Wrong: cite law for never-found control (Save at bottom of long scroll, off-screen action). → Right: law assumes visible, already located target; cite selective-attention.md + visibility-of-system-status heuristic.
- Wrong: hide unavailable controls (Fitts's Law, jakobs-law.md). → Right: disable w/ explanation; hidden controls break learned positions.
- Wrong: blame adjacent-button slips on movement time. → Right: mainly error prevention + spacing; law = at most supporting argument for larger, separated targets.
- Wrong: quote one formula as law. → Right: no single formula; variants share one core relation.
- Wrong: treat floors as law predictions. → Right: standards set minimum sizes; model has no size threshold.

Limits:
- Uniform scaling: ID depends only on D/W → model implies uniformly scaled whole layout keeps movement time unchanged; physically impossible.
- Original task one-dimensional (1D).
- Touch reverses pointer shortcuts: no persistent cursor, hand position unknown, finger lifts after each tap → no screen region reliably 'closer'.
- Practitioner shortcuts assume hand rests on mouse; often false (while typing, writing, using phone).

## Check questions
Tag [A] = answerable from artifact itself (see ../checklists/usability-review.md).

|Check|Look for|Law / principle|Tag|
|---|---|---|---|
|Touch targets in easy reach, spaced + large?|Small tap targets, cramped adjacent buttons, actions far from attention|Fitts's Law|[A]|
|Targets sized by position in physical units, whole visible element clickable?|Glyph-only hit areas, tiny corner targets, pixel-only specs|Fitts's Law|[A]|
|Every target ≥ its platform floor (24 × 24 CSS px or equivalent spacing on web, 44 × 44 pt iOS, 48 × 48 dp Android)?|Icon buttons + inline links below floor, adjacent targets w/ no gap|Fitts's Law as accessibility floor|[A]|
|Dangerous / unavailable controls disabled w/ reason (not hidden) + apart from positive actions?|OK beside Delete, controls vanishing by state, soft keys changing meaning|Fitts's Law, Jakob's Law|[A]|
|Every action reachable + operable by keyboard, in logical order, w/ visible focus indicator?|Hover-only menus, focus traps, invisible focus|postels-law.md for any access method, Fitts's Law|[A]|

## Symptoms → fixes

|Symptom|Likely cause|Fix|
|---|---|---|
|Mis-taps on mobile|Fitts's Law; error prevention for destructive neighbours|Meet 44 pt / 48 dp / 24 px floors; add spacing; place centre-first, not by thumb-zone maps; separate destructive neighbours|
|Mouse-era layout ported to touch|Fitts's Law|Centre-first layout; targets sized by position in mm; no edge / corner shortcuts on touch|
|Content jumps while loading → mis-clicks|doherty-threshold.md, Fitts's Law|Reserve space for late content; never move target under pointer; layout stability in performance budget|
|Destructive action regretted|Error-prevention heuristic; Fitts's Law for separation|Undo / soft delete first; confirm only irreversible, rare actions + name consequence; dangerous controls apart|
|Key control below fold / off-screen never found (Save at end of long page)|Selective Attention (tunnel vision) + visibility-of-system-status heuristic, not Fitts's Law (assumes visible target)|Sticky save bar once something changes, or auto-save w/ visible saved state; warn on leaving w/ unsaved changes|

## Hypothetical examples
- Hypothetical: e-scooter rental app's End ride button = hero control: biggest, most prominent spot on ride screen, though used only at ride's end.
- Hypothetical: pharmacy refill app: Refill right beside each prescription line (where eye already rests), not in distant toolbar; finger-sized on phones.
- Hypothetical: bank app's date-range handle = long strip, only hairline tall → hard to grab despite length; short side = stand-in for target width.

## Humane bound
- No abuse case recorded. Risk: irreversible action directly beside positive one.
- Same size + position lever used deliberately against people = 'hidden No': decline option shrunk, greyed or missing, e.g. tiny grey no beside bright accept → see ../ethics/deceptive-patterns.md.

|Principle|Bound on Fitts's Law|Read|
|---|---|---|
|../principles/empowering.md|Decline + skip get same size, contrast + position as accept|../patterns/defaults-and-choice-architecture.md (Equal-weight No)|
|../principles/inclusive.md|Size floors + keyboard access = accessibility floors|../patterns/inclusive-and-accessible-design.md|
|../principles/intentional.md|Destructive / irreversible actions: confirmation graded by consequence|../patterns/friction-undo-and-confirmation.md (graded confirmation, undo windows)|

## Related
- hicks-law.md: deciding step this law leaves out (it covers movement time only).
- selective-attention.md: cite for never-found controls, w/ visibility of system status.
- proximity.md: check w/ target spacing + task buttons near task.
- serial-position-effect.md: check w/ key-action placement.
- jakobs-law.md: learned positions break when controls hidden.
- postels-law.md: every access method, incl keyboard.
- doherty-threshold.md: layout shifts while loading.
- ../checklists/usability-heuristics-map.md: links law to Error prevention (classic heuristics 1990, revised 1994); related laws there: Postel's Law, Fitts's Law (destructive-target spacing), Working Memory.
- ../checklists/usability-review.md: meaning of [A] tag.
- ../methods/testing-touch-layouts.md: test targets under real grip + context.
- ../guides/laws-and-principles-crosswalk.md: humane principle bounding law.
- ../patterns/navigation-and-menus.md: applies law.
- ../patterns/calls-to-action-and-touch-targets.md: applies law.
- ../patterns/errors-and-input-tolerance.md: applies law.
- ../patterns/defaults-and-choice-architecture.md: equal-weight decline.
- ../patterns/inclusive-and-accessible-design.md: size floors + keyboard access.
- ../patterns/friction-undo-and-confirmation.md: graded confirmation, undo windows.
- ../ethics/deceptive-patterns.md: misuse side ('hidden No').
- ../principles/empowering.md, ../principles/inclusive.md, ../principles/intentional.md: principles bounding it.
