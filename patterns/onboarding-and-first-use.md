# Onboarding and first use

## Scope + laws behind these patterns
- Use for: usability patterns for product's first session + first week: starting w/o tour · in-context guidance · progressive onboarding · safe exploration · help content · empty states · first success · sign-up timing · accessible onboarding · re-engagement nudges.
- Applies when: designing/reviewing onboarding, tours, tooltips, empty states, activation or week-one messages.
- Laws underneath: ../laws/paradox-of-the-active-user.md, ../laws/teslers-law.md, ../laws/cognitive-load.md, ../laws/zeigarnik-effect.md, ../laws/goal-gradient-effect.md, ../laws/flow.md, ../laws/jakobs-law.md.
- Scope limits:
  - ../laws/hicks-law.md applies in onboarding only to choosing among options (e.g. goal/role picker), not to informational tour screens → those belong to ../laws/cognitive-load.md lens.
  - ../laws/peak-end-rule.md applies to first real success, not to skipping/dismissing tour.

### New user arrives: tour first or work first?
- When: new user arrives (let people start immediately).
- Do: product usable at once, guidance alongside work. Design first use for impatient, goal-driven people, not idealized user reading everything.
- Avoid: front-loaded product tour = overlays pointing at UI parts before any use.
- Why: front-loaded tour = making people adapt to technology; active users find it annoying; most people take in little or nothing of it. Long run, learning first would save time, but task at hand wins anyway. Origin: 1987 observations of computer novices: launched into real use at once, pressing on through dead ends + mistakes; documentation shipped w/ machine went unread. ../laws/paradox-of-the-active-user.md.
- Hypothetical: home-insurance claim app opens straight on "photograph the damage", short hint beside camera button, not welcome carousel.

### Where does guidance live?
- When: any route first-time user takes may end at any feature → in-context help needed across product.
- Do: help on every route via tooltips shown when relevant, context-tied + lightweight. Same contextual tooltips surface new features to existing users when relevant: discovery, not announcement tour.
- Avoid: guidance only on one prescribed onboarding path or in docs nobody opens.
- Why: ../laws/paradox-of-the-active-user.md.
- Hypothetical: tax-filing site shows brief tip beside deductions field first time anyone opens it, whichever route led there.

### Product has a rich feature set?
- When: products w/ rich feature set (onboard progressively).
- Do: reveal features as each step mastered, keep rest hidden + give risk-free space w/ one core action.
- Aim: functions found once person ready for them; person sets exploring speed; small steps build confidence + familiarity.
- Avoid: short welcome carousel, then whole app opened up at once.
- Why: if each function surfaces only when it fits moment → even heavy toolset + demanding processes learned w/o overload, because each new piece of learning attaches to knowledge person already holds. ../laws/teslers-law.md, ../laws/cognitive-load.md.
- Hypothetical: small-business accounting suite first shows only "record an expense" inside sandbox company; invoicing + payroll appear once recording expenses routine.

### Flexible product whose range could swamp people?
- When: flexible product whose range of possibilities could swamp people (revisitable starter checklist or template).
- Do: checklist or get-started template, returnable any time + used at person's own pace, where real use teaches core features.
- Why: ../laws/cognitive-load.md.
- Hypothetical: website builder's starter site carries short, simple checklist (change headline, add photo, publish) owner can reopen from help menu any time.

### People learn by trial and error?
- When: trial-and-error learning (make exploration safe).
- Do: exploring causes no lost work + no irreversible damage. Short feedback loops, e.g. live previews as settings change. Teach shortcuts in place: reveal accelerators when they would help, e.g. hover tip showing faster drag-and-drop. Each operation gets obvious inverse, named as pair (e.g. drop/pick up). Undo so experiments do no lasting damage. Choose undo grain (character, command, task) deliberately.
- Avoid: long action sequences w/o visible result.
- Evidence: 1984 training-wheels studies: for beginners keep all choices visible but disable advanced/error-prone ones w/ short "not available yet" message, system state unchanged.
- Limit: in safety-critical domains trial + error alone not enough; formal training still needed.
- Hypothetical: photo-printing service previews each crop + border change live, undo per edit, + greys out poster sizes w/ "not available yet" note until first print ordered.

### Writing help content or choosing a metaphor?
- When: writing reference + help content; choosing interface metaphor.
- Do: sort reference + help by real usage frequency + goals, not alphabetically. Metaphors whose obvious matches ease starting. Make metaphor's break points clearly visible so new concept gets learned, e.g. typewriter-like editor inserting text rather than overstriking.
- Avoid: silently breaking metaphor.
- Evidence: one 1980s text editor: large share of its 140 commands used only in macros, yet manual listed all of them alphabetically. One observed user, misled by broken metaphor, spent almost one hour producing pads of folders instead of document.
- Hypothetical: digital wallet shaped like physical wallet flags plainly: user can still restore "removed" card for some time, where real wallet would not allow it.

### List, inbox, workspace or dashboard is empty?
- When: list, inbox, workspace or dashboard empty (empty state = first step).
- Do: say what will appear + why it matters. One primary action filling it. Deletable starter sample or template.
- Avoid: blank panels, zero-value charts + generic illustrations w/o action.
- Evidence: starter samples rest on worked-example effect (1993 studies) + ../laws/paradox-of-the-active-user.md (1987).
- Hypothetical: household-budget app's empty overview says "Your monthly spending by category shows here", offers "Connect an account" + loads removable sample month.

### What should the first outcome be?
- When: first run, first transaction or first key-feature use.
- Do: first outcome clearly positive, core value first. Set time-to-first-value targets from own baseline data + treat as hypotheses.
- Avoid: first session ending in error, empty state or paywall.
- Why: early outcomes frame later judgment (outcome primacy, order effects). First real success, not tour, = true Peak-End lever in onboarding (../laws/peak-end-rule.md).
- Limit: no research figure recorded for how fast first result must arrive; locate + measure it w/ ../methods/activation-moment.md.
- Hypothetical: meal-kit service's first session ends on confirmed first delivery + preview of its recipes, not paywall for full menu.

### Multi-step setup or profile completion?
- When: multi-step setup + profile completion (incompleteness + head start).
- Do: clear progress. Small head start. Signal more remains. When justifying progress device, cite mechanism genuinely at work:
  - Endowed progress = pre-credited checklist step, instance of ../laws/goal-gradient-effect.md; perceived nearness to goal raises effort.
  - ../laws/zeigarnik-effect.md = memory for interrupted task; fits checklist started + then left, easy to recall + resume.
  - Cite both only when both present.
- Avoid: misleading false progress (../ethics/using-psychology-responsibly.md).
- Hypothetical: volunteer-matching site credits already-verified email as setup step one + shows remaining steps; half-filled skills profile reopens where left.

### Some users struggle on the first task while others coast?
- When: tuning first-task difficulty; some users struggle while others coast (match challenge to skill).
- Do: challenge > skill → build skill: coaching, hints, progressive disclosure. Skill > challenge → add depth: shortcuts, advanced modes, stretch goals. Plan first 15 minutes, then how product grows w/ user.
- Avoid: making product harder for everyone. Added challenge fits only once skill > current challenge.
- Why: task asking too little → boredom, too much → frustration → balance challenge against skill. ../laws/flow.md.
- Hypothetical: spreadsheet course: learners finishing first exercise quickly get advanced-formula stretch task, while those stalling get inline hints on next step.

### Value possible before an account exists?
- When: value possible before account exists (invest before registering).
- Do: let visitors start working (choose template, edit draft) before having account. Deliver value before asking for account. Ask for sign-up when visitors want to keep/export their work.
- Avoid: forced sign-up before value. Holding work hostage or using invested effort coercively.
- Why: after investing effort, creating account feels like protecting what person owns. Guardrails for invested-effort levers in ../ethics/using-psychology-responsibly.md.
- Hypothetical: floor-plan tool lets homeowner sketch rooms at once + asks for account only when they choose to save/print plan.

### Are tours, skips and consent steps accessible and honest?
- When: building any tour, tooltip, coach mark, celebration, skip or consent step.
- Do: tours, tooltips + coach marks reachable by keyboard + screen reader. Focus into tour/tooltip when it opens + back to its trigger when it closes. Visible, labelled skip. Honor reduced-motion preferences in onboarding animations + celebrations.
- Avoid: confirmshaming = skip/decline option worded to shame, e.g. "No thanks, I like wasting time". Pre-checked marketing consent. Tooltips trapping focus or vanishing on timer.
- Why: accessibility floors in inclusive-and-accessible-design.md; named patterns in ../ethics/deceptive-patterns.md.
- Hypothetical: museum app's welcome walkthrough has labelled "Skip" button reachable by keyboard; decline reads plainly "Not now".

### Week one: re-engagement nudges and permission asks?
- When: re-engagement + permission asks in week one.
- Do: base nudges on what user did or left unfinished (half-built project, invited teammate now joined), not calendar. Each nudge → one loop-closing next action. Prefer in-product messages + email over push until person has seen value. Ask push permission in context, after moment showing its usefulness. Cap frequency + stop when person returns or completes task. One-tap opt-out + frequency setting on each message.
- Avoid: fixed daily drip messages ignoring progress. Guilt or streak-loss copy. Asking notification permission at first launch.
- Why: humane bounds on nudges + permission asks in notifications-and-interruptions.md.
- Hypothetical: online-course platform emails "Your draft quiz is saved, add the last question?" only after teacher left one unfinished + stops once published.

## Related
- ../methods/teaching-inside-the-task.md: step method for designing first use around learning by doing.
- ../methods/activation-moment.md: locating first real success + measuring path to it (time to value).
- ../laws/paradox-of-the-active-user.md: law behind starting immediately + in-context guidance.
- progress-goals-and-completion.md: progress indicators, head starts, multi-step completion.
- notifications-and-interruptions.md: humane bounds on re-engagement nudges + permission asks.
- ../ethics/deceptive-patterns.md: named deceptive patterns + honest alternatives for sign-up, skip/decline + consent steps.
- ../ethics/using-psychology-responsibly.md: guardrails for progress, incompleteness + invested-effort levers.
- inclusive-and-accessible-design.md: accessibility floors tours, tooltips + celebrations must meet.
