# Memorable moments and endings

## Scope + laws behind these patterns
- Use for: emotional-journey mapping · designing positive peak · ending well · ordering mixed feedback · matching investment to offer price · neutralizing negative peaks · evidence on why endings outweigh duration.
- Applies when: designing/reviewing confirmation + success screens, exits, waits or failure moments, or prioritizing fixes across journey.
- Laws underneath: ../laws/peak-end-rule.md, ../laws/serial-position-effect.md (recency part), ../laws/cognitive-bias.md (memory bias), ../laws/goal-gradient-effect.md, ../laws/von-restorff-effect.md.

### Where are the peaks? Map the journey first
- When: planning/auditing journey.
- Steps: three-zone journey map.
  1. Lens = whose view: research-grounded persona, one specific scenario, persona's expectations.
  2. Experience = phase + action timeline, mindset layer (motivations, questions, pain points, thoughts), emotion line where peaks show.
  3. Insights = internal owners, metrics, opportunities.
- Do: draw emotion layer as one unbroken curve across every phase; its highs + lows = candidate peaks. Let map sections bend to project aims. Product not yet launched → still map it; lens scenario may describe actual or merely expected use.
- Why: three-zone map → stakeholders share one journey model. Journey mapping = qualitative exercise. Procedure in ../methods/peaks-and-endings.md.
- Hypothetical: library-card signup map: lens = newly arrived resident w/o utility bill in own name, expecting to borrow books same day; emotion curve dips at proof-of-address step = candidate negative peak; insights zone names branch-services team as owner.

### Moment of greatest value or high-stakes commitment?
- When: moment of greatest value, help or fun, or of high-stakes commitment (design positive peak).
- Do: stressful step w/o undo needs calming, newcomers most of all → in brand's own voice: drawing, light joke, gentle motion. Where product genuinely useful/enjoyable, enlarge high point there.
- Avoid: artificial delight in moments not already valuable.
- Why: ../laws/peak-end-rule.md; guardrails for memory levers in ../ethics/using-psychology-responsibly.md.
- Hypothetical: first-time home buyer at final mortgage e-signature sees short warm line ("Big step. Here is what happens next") + quiet front-door illustration, not bare wall of legal text.

### What goes on the final screen of a flow?
- When: final screen of any flow (end well).
- Do: confirm success. Show relevant details. State next steps. Acknowledge person's effort. Ideally small celebratory touch. Prefer inline confirmation keeping context over redirect. Design in-place failure state as carefully as success state. Informative completion feedback, e.g. after autofill say how many fields filled + highlight them.
- Avoid: generic, off-brand success pages. Blocking alert dialogs at flow end. Celebratory motion ignoring reduced-motion preferences.
- Why: ../laws/peak-end-rule.md, ../laws/serial-position-effect.md (recency); carrying people to end in progress-goals-and-completion.md.
- Hypothetical: moving-company booking's done screen lists date, address + crew arrival window, thanks person for long inventory form + plays brief confetti burst staying still under reduced-motion setting.
- Hypothetical: expense-report tool confirms submission inline on same report (status → "Submitted", approver named, next step stated), not redirect to generic dashboard.

### Person is leaving: cancel, log out, exit?
- When: cancellation, logout, leaving.
- Do: exit cleanly.
- Avoid: exit-intent please-don't-go pop-ups, discounts, upsells or any other hook at exit.
- Why: hook at exit becomes remembered ending. Humane rule behind it = symmetric exit (leaving as easy as joining) in defaults-and-choice-architecture.md; ../principles/finite.md: experience has edges + natural stopping points, other side of clean ending; named exit hooks in ../ethics/deceptive-patterns.md.
- Hypothetical: gym membership cancelled online ends on last-billing-date confirmation + how to rejoin, no retention offer.

### Mixed feedback: which item goes last?
- When: reviews, reports, grades, audits.
- Do: end mixed feedback on its most positive/acceptable item.
- Avoid: ending on harshest item.
- Bound: do not invent positives to soften feedback.
- Evidence: 2017 study: appending one moderately negative rating to negative assessment, or one moderately positive rating to positive one → longer version remembered as more pleasant.
- Why: ../laws/peak-end-rule.md, ../laws/serial-position-effect.md (recency).
- Hypothetical: code-review tool summary lists blocking issues first, closes on genuinely passed checks.

### Premium or low-cost offer: invest early or late?
- When: matching investment to offer price.
- Do: premium offer → front-load quality. Low-cost offer → strong ending pays more. Set expectations early so ending does not disappoint.
- Why: premium → high expectations → early mismatch dominates judgment.
- Evidence: pizza-buffet field study: diners paying $4 based taste judgments on peak + last slice; diners paying $8 based them on first slice.
- Hypothetical: premium wealth-advice service puts most polished session first; free budgeting app saves warmest moment for month-end summary.

### Wait, failure or confusion, and a limited fix budget?
- When: waits, failures, confusing moments; prioritizing fixes on limited budget (neutralize negative peaks).
- Do: treat negative peaks as most memorable moments. Soften most intense negative spikes (data loss, surprise fee, hostile cancellation step) before adding delight. Hunt confusion + friction in testing as negative peaks. Waits → wait patterns in feedback-loading-and-performance.md. Failures → fallbacks in errors-and-input-tolerance.md.
- Why: bad experiences leave sharper memory.
- Hypothetical: photo-backup service w/ budget for one fix stops silent deletion of unsynced photos instead of adding confetti animation to uploads.

## Why endings outweigh duration
|Study|Setup|Finding|
|---|---|---|
|1993 experiment|two cold-water immersions, one per hand; both incl. 60 seconds in 14°C water; one ran 30 seconds longer while water rose to 15°C|more participants chose to repeat longer trial, because remembered less unfavorably → contradicts temporal monotonicity|
|1996 study|colonoscopy + lithotripsy patients|whatever duration, discomfort ratings followed worst point + end|
|2003 study|colonoscopy extended by three minutes, scope tip held still (no inflation, no suction)|remembered as less unpleasant; patients given extended ending had higher odds of returning for later procedures|

- Mechanism: whether people return/recommend follows rough mean, formed in memory, of feeling at peak + at end.

## Related
- ../methods/peaks-and-endings.md: procedure: map emotional journey, shape its peak + end.
- feedback-loading-and-performance.md: wait patterns for delay-caused negative peaks.
- errors-and-input-tolerance.md: fallbacks + recovery for failure moments.
- progress-goals-and-completion.md: carrying people to end of multi-step task.
- defaults-and-choice-architecture.md: symmetric-exit rule (leaving as easy as joining), behind exiting cleanly.
- ../ethics/deceptive-patterns.md: named deceptive patterns + honest alternatives; relevant to exit hooks.
- ../ethics/using-psychology-responsibly.md: guardrails for peak-end + other memory levers.
- ../principles/finite.md: experience has edges + natural stopping points; other side of clean ending.
