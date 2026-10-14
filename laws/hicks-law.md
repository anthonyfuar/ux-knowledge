# Hick's Law (Hick-Hyman Law)

## In one line
More choices, more complex choices → longer decision time. Measurable form: RT = a + b log2(n); reaction time grows w/ log of option count n. Use for: options per step, whether to recommend one, staging onboarding, whether Hick's Law = right law to cite.
- Alias: Hick-Hyman Law. Class: effect / principle.
- Theme: Decisions. Most affects: options per step, recommended defaults, progressive onboarding.
- How to apply: decision slows as options grow more complex + log of their count rises; if speed critical → cut n, split n across steps, add recommended default.

## Applies when / does not apply when
|Applies when|Does not apply when → cite instead|
|---|---|
|people choose among options|informational screens, nothing to choose|
|response speed critical: few choices matter most there|sequential no-choice screens (tour slides, intro carousels): cost = attention + working memory → Cognitive Load, Paradox of the Active User|
|ordered list w/ known target (alphabetical / known key): only here log benefit holds|unordered list: scan = linear search → model as linear scan; Serial Position Effect or Chunking for placement|
|onboarding: choices within single step (e.g. goal / role picker)|onboarding slides, nothing to choose|
|choices within each step of split flow|splitting data-entry form into steps → Chunking + Cognitive Load|

Assumptions behind law: options equally likely; user knows target's name; responses learned + well mapped.

Modifiers + exceptions:
- Options not equally likely → decision time tracks information (entropy H, in bits), not count: T = b·H. Law concerns information (uncertainty) → predictable options cost less time than their count suggests.
- Choice made beforehand → option count barely slows decision; finding chosen item in unordered list still costs linear scan.
- Stimulus-response compatibility shifts RT on top of option count: control moving like its effect → faster response.
- Little or no slowdown for spoken responses to familiar stimuli (1985 study).
- Saccadic eye-movement time stays flat or falls as targets multiply = "anti-Hick" effect (2002 + 2008 studies).

## Decision rules

### Number of options
- Wherever people must react quickly → few options.
- If speed critical → cut n; split n across steps; add recommended default.
- Per screen/step, low option count: spread lengthy flow, many-part task + any extended run of choices across successive steps.
- Short path for frequent case; do not burden majority for curious minority.
- At entry step → offer one goal; defer secondary options (e.g. filters) until after core action.

### Recommending
- Recommend one option: mark one you would suggest so full set does not swamp people.
- Recommended option relieves overwhelm + remedies overload but = no license to hide essentials: recommend, do not conceal.

### Onboarding
- Stage onboarding: introduce features bit by bit → newcomers carry less load.
- If newcomers must grow into heavier workflows → hold each feature back until it pays off; they then get there w/o getting swamped.
- Onboarding = high-stakes: much rides on it + much can go wrong.

### How far to reduce
- Stop reducing before interface turns abstract: keep enough so reduction never ends in abstraction.
- Pair w/ Tesler's Law: system must carry complexity removed from screen; Tesler's Law sets reduction floor.
- Move complexity into progressively disclosed layers.
- Do not over-correct into long chains of binary menus (10 or more clicks): people leave before reaching content.
- Extra steps cheap when each clearly signals path to goal (information scent, term from 1999) → measure per-step success + hesitation, not click count.

### Lists + menus
- Want log benefit → order list (alphabetical / known key) + ensure target known.
- Unordered navigation → model as linear scan; reduce, group + order items.

## Why it works

### Mechanism
- Each added stimulus brings unwanted work: reading + ruling in or out.
- Extra options = unrequested work, each weighed + made sense of → reducing options, sequencing them or progressive disclosure lowers cognitive load + working-memory demand.
- Decision time grows logarithmically, not linearly: people categorize + discard about half of remaining options per step (like binary search), not checking one by one → doubling options adds constant increment.
- Original form: T = b·log2(n + 1); +1 = uncertainty about whether to respond at all.
- Applied form: RT = a + b·log2(n); constants a + b fitted per task.
- Same information-theory form as Fitts's Law.
- Feature creep ends in button-crowded device usable only via heavy mental effort or repetition-built muscle memory. Hypothetical: office copier panel gains button w/ every release → workable only by staff stopping to puzzle it out or having run it often enough to act by rote.

### Origin
- Precursors: choice RT work, 1868 + 1885.
- Two psychologists' separate studies (1952 + 1953) measured reaction speed to one stimulus as count of possible stimuli changed; larger set slowed choice.
- Logarithmic benefit for ordered lists w/ known target shown by later extension in menu research (1985), not by original lamp experiments.

## Evidence
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Larger set of possible stimuli → slower choice|original experiments (1951–52): 10 lamps in circle, Morse key for each finger, pre-punched tape lit random lamp every 5 seconds; stimulus + response pen-logged as 4-bit codes (16 states possible, 10 used); later blocks gave accuracy-vs-speed instructions|1952 data from two participants; evidence = RT to stimuli in lab|fewer options where speed matters|
|RT rose linearly w/ information transmitted, not w/ option count per se|1953 study: 6x6 light matrix w/ eight named lights + varied frequency|lab experiment|predictable options cost less time than their count suggests|
|Log-time benefit only in ordered lists (alphabetical / known key)|1985 menu research: alphabetic + numeric menu trees on touch screen|—|do not cite Hick's Law for unordered menus|
|Little or no slowdown|1985 study, spoken responses to familiar stimuli|exception to law|—|
|Eye-movement time flat or falling as targets multiply ("anti-Hick")|2002 + 2008 saccade studies|↑|—|
|Too many options can multiply time on task (feature creep)|not stated|hedged (can)|cut + layer options|
|Pour normally under 10 seconds took some people over one minute (over 500% increase); queues formed. One bystander: families w/ children + older people stalled machine most|2015 observation, touchscreen soda fountains: 100+ flavor combinations in multi-level menus|observational, no controlled comparison; one bystander|short path for frequent case|

### Case: Google Search
- Landing page: filtering held back until results exist; before then, only search option = query box, centred + already focused on load; suggestions recompute on every keystroke → person can choose query before fully typing it.
- Results flow: query kept visible, retrieval time shown, results in spaced chunks, borders around videos + featured snippets.
- Landing page changed little since 1998 launch; evidence strength = longevity + adoption, no study.
- Lesson: Hick's Law, working memory, Doherty Threshold, chunking, proximity + connectedness combined in one flow.

## Misreadings and limits
- Wrong: simplifying until controls become abstract (Hick's Law, Tesler's Law) → Right: keep meaning; complexity must go somewhere. Over-reducing options → abstract, meaningless interfaces w/ lost meaning.
- Wrong: cutting clicks as goal, e.g. fixed click budget (Cognitive Load, Hick's Law) → Right: extra steps cheap when each clearly signals path to goal (information scent, 1999); measure per-step success + hesitation, not click count.
- Wrong: citing Hick's Law to set/size unordered menu length → Right: unordered lists scanned linearly; law applies only to ordered lists w/ known target. Citing it for menu length usually misapplication.
- Wrong: citing Hick's Law for navigation w/o checking order + target knowledge (e.g. 14 unordered nav items) → Right: model as linear scan; reduce, group + order items; cite Serial Position Effect or Chunking for placement.
- Wrong: citing Hick's Law for sequential no-choice informational screens (tour slides, intro carousels) → Right: law = decision time among options, silent on no-choice screens; cite Cognitive Load (attention spent before value arrives) + Paradox of the Active User.
- Wrong: Hick's Law justifies splitting data-entry form into steps → Right: Chunking + Cognitive Load justify splitting.
- Wrong: recommended option licenses hiding essentials → Right: recommend, do not conceal.
- Wrong: fewer options always yield better product → Right: law does not say so.
- Limit: over-correcting into long chains of binary menus (10 or more clicks) → people leave before reaching content.
- Limit: evidence behind law = RT to stimuli in 1952 + 1953 lab experiments.

## Check questions
[A] = answerable from artifact itself (screen, prototype, spec).
- [A] (Hick's Law) Options minimal where speed matters? Look for: crowded entry screens; long menus; extra options before core action.
- [A] (Chunking, Cognitive Load; Hick's Law only for choices within each step) Option count small at every step + any extended or many-part flow run as sequence? Look for: one huge form or settings page.
- [A] (Hick's Law, Choice Overload) Recommended / featured option present? Look for: equal weight on all choices.
- [A] (Tesler's Law, Hick's Law) Simplification stops short of abstraction? Look for: controls reduced until their meaning lost.
- Before citing: list ordered + target known? If not → linear scan, not Hick's Law.
- Before citing: any choice at all? If not → Cognitive Load + Paradox of the Active User.

## Symptoms → fixes
|Symptom|Likely cause (laws)|Fix|
|---|---|---|
|People stall on crowded entry screen|Hick's Law, Choice Overload|one focused entry action; filters + secondary options after it|
|Pricing/plan choice paralyzing|Choice Overload, Hick's Law|side-by-side tiers w/ one recommended|
|People leave before reaching content|over-correction into long chains of binary menus (10 or more clicks)|fewer chained steps, each clearly signalling path; measure per-step success + hesitation|
|Controls no longer say what they do|over-reduction into abstraction (Hick's Law, Tesler's Law)|restore meaning; move complexity into progressively disclosed layers carried by system|
|Frequent task slowed by rare options|majority burdened for curious minority|short path for frequent case|

## Hypothetical examples
- Hypothetical: people simplify it themselves → family member moves every app on older relative's tablet into one folder except calls, photos + messages → sign: device shows more options than person's frequent tasks need.
- Hypothetical: essentials up front, complexity in layers → parking-meter kiosk shows only "Pay for parking" + "Extend"; permits, receipts + fines open step by step behind "More" → person holds little in mind at kiosk.
- Hypothetical: staged onboarding → freelancer invoicing tool first shows only "Create invoice"; sample client → person sends risk-free practice invoice to self; expenses, taxes + reports appear once first skill in place.
- Hypothetical: contrast → person installs library-loans app, swipes through intro slides + meets every catalogue, hold, fine + event feature on first real screen; nothing introduced step by step.
- Hypothetical: high-stakes control panel → hospital infusion-pump screen gathered settings over releases; every change costly: affects how nurses dose at bedside.
- Hypothetical: arguing for simplification → pump team proposes bedside mode w/ a few large essential options + cites Hick's Law as rationale when making case to device maker's engineering + product teams.

## Humane bound
- Bounded by Empowering: audit omissions; keep full catalog one tap away.
- Bounded by Intentional: default should be recommendation you would defend aloud.
- Turned against people: recommended option used as license to hide essentials.
- Turned against people: menu control; whoever writes options frames question → choice feels free while alternatives never appear.
- Turned against people: recommendation/default picked for business, not what most people would choose if fully informed.
- Further reading: defaults + choice architecture patterns (opt-in, equal-weight decline); attention hijacks + their counters; decision fatigue + choice evidence (defaults, choice overload, decision quality).

## Related
- ../principles/empowering.md: humane principle bounding Hick's Law; audit omissions.
- ../principles/intentional.md: humane principle bounding Hick's Law; defaults you would defend aloud.
- ../patterns/defaults-and-choice-architecture.md: humane bounds on recommended option/default (opt-in, equal-weight decline).
- ../ethics/attention-hijacks.md: further reading on humane bound.
- ../evidence/decision-fatigue-and-choice.md: evidence on defaults, choice overload + decision quality.
- choice-overload.md: shares recommended-option question + crowded-entry and pricing/plan fixes.
- cognitive-load.md: what cutting + sequencing options lowers; law to cite for no-choice screens + split data-entry forms.
- paradox-of-the-active-user.md: cite for no-choice tour screens.
- teslers-law.md: sets reduction floor; system must carry removed complexity.
- fittss-law.md: same information-theory form.
- serial-position-effect.md: cite for placement in unordered navigation.
- chunking.md: cite for placement + splitting forms into steps.
- ../checklists/usability-heuristics-map.md: heuristic "Aesthetic and minimalist design" (related laws: Aesthetic-Usability, Occam's Razor, Cognitive Load, Hick's Law); classic usability heuristics date from 1990, revised 1994.
- ../guides/laws-and-principles-crosswalk.md: names humane principle bounding Hick's Law.
- ../patterns/navigation-and-menus.md: applies Hick's Law.
- ../patterns/calls-to-action-and-touch-targets.md: applies Hick's Law.
- ../patterns/forms-and-data-entry.md: applies Hick's Law.
- ../patterns/onboarding-and-first-use.md: applies Hick's Law.
- ../patterns/search-and-results.md: applies Hick's Law.
- ../patterns/lists-options-and-choice.md: applies Hick's Law.
- ../patterns/complexity-management.md: applies Hick's Law.
- ../patterns/ai-and-automated-features.md: applies Hick's Law.
