# Intentional

## In one line
- Intentional = quick win weighed vs later + second-hand effects.
- Friction placed on purpose where it supports habits people would endorse, keeps privacy intact + stops abuse.
- If pause protects people (irreversible actions, data exposure, purchases, sharing) → keep/add resistance.
- If friction merely frustrates → remove it.
- Set defaults for well-being, because most people never change them.
- Anticipate product's ripple effects on people not using it.
- Open when: design/review touches confirmations, undo windows, speed bumps, defaults, step removal, or long-run + second-hand consequences.

## Core practices
Highest weight; check first.
1. Confirmation effort scaled to severity: inline confirmation, menu, type-to-confirm or delay-then-undo.
2. Explicit confirmation before money moves or content shared.
3. Algorithmic speed bumps: rate limits, forwarding caps, delayed amplification.
4. Defaults chosen for well-being; no default where active choice matters.
5. Second-order thinking, futures wheel + premortem before building.

## Commitments w/ a pattern entry
|Commitment|Do|Avoid|Entry|
|---|---|---|---|
|Graded confirmation|confirm irreversible/high-consequence actions, graded by severity up to type-to-confirm||../patterns/friction-undo-and-confirmation.md|
|Undo on sends|delay-then-undo window on sends||same|
|Algorithmic speed bumps|rate limits, delayed amplification, forwarding caps, restrictions on new accounts||same|
|Meaningful effort|meaning-building effort; friction nudge only when it benefits person||same|
|Money + sharing|explicit confirmation before purchases, money movement + sharing||same|
|Sensitive actions|step-up authentication||same|
|Defaults|honest, beneficial suggestions; withheld where active choice matters||../patterns/defaults-and-choice-architecture.md|
|Ask, do not assume|offer choice at moment it becomes meaningful|assuming|../patterns/calm-technology-and-device-etiquette.md|
|Extended use|moderation prompt after extended use||../patterns/feeds-scrolling-and-pacing.md|
|After launch|keep watching; at outset, set up what's needed on day it fails or does harm||../patterns/safety-and-abuse-resistance.md|
|Beyond the people using it|account for indirect users, externalities + fragile contexts||../patterns/inclusive-and-accessible-design.md|

## Process practices (method files)
Each has own method file; process patterns assuming them → ../methods/process-safeguards.md.

|Practice|Procedure|
|---|---|
|Pair every growth metric w/ user metric + counter-metric|../methods/counter-metrics.md|
|Gate decisions w/ three-gate check (three gates)|../methods/three-gate-check.md|
|Second-order thinking + futures wheel|../methods/second-order-thinking.md, ../methods/futures-wheel.md|
|Premortem before launch|../methods/premortem.md|
|Consequence scanning as recurring ritual, w/ anti-goals|ritual → ../lookup/organizations-and-toolkits.md; worst cases → anti-goals → ../methods/misuse-case-brainstorming.md|

## Guidance held here (no pattern entry)

### Told a product category is unstoppable?
- Do: refuse inevitability argument. Name decisions still open: what product senses + retains, when it speaks, whether it's on before anyone gets asked.
- Why: inevitability argument ends design conversation before consequences examined.
- Face-worn display hands nobody the world, only what computer left of it after filtering.

### Making an action effortless?
- Ask: does this action deserve effortlessness? Ask of one-tap actions in design, not only of steps getting removed.
- Wrong: ease = goal needing no justification → Right: physical effort carries part of act's weight.
- Hypothetical: signing paper petition = walking to town-hall desk + writing name in front of clerk → residents sign only causes they back.
- One-tap broadcast carries no such cost → product, not person, settles how much deliberation speech gets.

### Shipping a minimal first release?
- Do: schedule + fund contextual edge-case work inside release; don't let MVP become final.
- Why: minimal first release becomes product people live with, since postponed cases rarely get picked up again.

### Wants vs higher needs?
- Do: put higher needs ahead of momentary wants; let people set content they aspire to see.
- Claim: until UX reworks its founding metaphors, only passing wants find expression, not higher needs; this rework = field's next step.
- Do: use behavioural science only toward person's own goals.
- Wrong: revealed preference = well-being → Right: revealed preference does not equal well-being.
- Rule: persuasion defensible when person would endorse it knowing how it works.

### Building a habit loop?
- Do: build habits people endorse on reflection; aim for people returning by choice, not hooked into compulsive use.
- Measure: returns driven by help, not compulsion.
- Why: variable rewards + streak anxiety manufacture dependence.

### Showing that work takes time?
- Do: perceived effort only when real; visible pause can honestly convey thoroughness.
- Avoid: animating progress for work not happening.

## Why it matters
- Origin of problem: by 2018 industry treated, almost without question, any removed friction as good in itself.
- Second problem: happy-path development: MVP ships + deferred edge cases never return.
- Convenience quietly overrides people's stated preferences.
- Pursued relentlessly, convenience hollows out effort underpinning reflection + agency.

## Key concepts
|Term|Meaning|
|---|---|
|Friction|whatever adds to time/effort of using product = what "frictionless" doctrine aims to strip away|
|Friction-value curve|bell curve: both zero friction + excessive friction destroy value|
|Manual vs algorithmic speed bumps|visible confirmations vs system-level pacing + limits|
|Default effect|inertia, loss aversion + status quo bias make preselected option likely outcome|
|First-, second- + third-order consequences|direct effects; effects of those effects; ring beyond them, where harms usually live|
|Prospective hindsight|picturing not-yet-happened outcome in past tense; premortem rests on it|
|Direct vs indirect users|those using product vs those affected w/o using it|
|Three-gate check|technical possibility, legal permission + moral justification = three separate gates|

## Audit questions
Scope: long-run consequences + friction on purpose. All principles' questions → ../checklists/humane-design-audit.md.

|Check|Passes when|
|---|---|
|Confirmation effort proportional to irreversibility + reach?|inline confirmation for harmless actions, menu for moderate ones, type-to-confirm for catastrophic ones, delay-then-undo for sends|
|No purchase, share, publish or send completes on one unguarded tap?|confirmation proportionate to consequence; if confirmation missing → ask whom its absence benefits|
|Defaults favour well-being, privacy + intent?|defaults set knowing most people never change them; opt-in for data + add-ons|
|Questions about consent, identity, money + relationships have no preselected answer?|neutral active choice; nothing pre-ticked/pre-highlighted|
|Algorithmic speed bumps present, e.g. rate limits, delayed amplification + forwarding caps?|mechanisms slowing abuse + cascading harm|
|Did team weigh consequences over months + years, not only next quarter?|futures wheel/premortem on record|

### Step-removal note
1. For each removed step, record: load-bearing (created deliberation, ownership or commitment) or mere tedium?
2. Removed load-bearing step = finding in itself. Removed tedium = no finding.

## Neighbours to check
- Check alongside: finite.md, inclusive.md, resilient.md.
- Working w/ neighbours → [Principles index](index.md).

## Related
- ../patterns/friction-undo-and-confirmation.md: when/do/avoid entries for confirmation graded by consequence, undo windows + speed bumps.
- ../patterns/defaults-and-choice-architecture.md: entries on defaults, opt-in + where to withhold defaults.
- ../methods/second-order-thinking.md: what happens at full adoption + where costs fall.
- ../methods/premortem.md: imagine failure before launch + work backwards.
- ../methods/counter-metrics.md: pairs each growth metric w/ harm it could hide.
- ../evidence/convenience-and-friction.md: evidence on what removing/adding friction does.
- ../patterns/errors-and-input-tolerance.md: usability side: error prevention + recovery, destructive actions.
- ../guides/laws-and-principles-crosswalk.md: psychological lever each principle guards + principle bounding each law.
- ../checklists/humane-design-audit.md: audit questions for all seven principles together.
- [Principles index](index.md): seven principles side by side + how to work w/ neighbours.
- Pattern files tagged Intentional: ../patterns/ai-and-automated-features.md, ../patterns/recommendations-and-personalization.md, ../patterns/notifications-and-interruptions.md, ../patterns/feeds-scrolling-and-pacing.md, ../patterns/defaults-and-choice-architecture.md, ../patterns/friction-undo-and-confirmation.md, ../patterns/privacy-data-and-security.md, ../patterns/calm-technology-and-device-etiquette.md, ../patterns/safety-and-abuse-resistance.md, ../patterns/transparency-and-honesty.md, ../patterns/monetization-and-growth.md, ../patterns/habits-streaks-and-gamification.md.
