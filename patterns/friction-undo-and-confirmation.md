# Friction, undo and confirmation

## Scope
- Confirmation graded by consequence, undo windows, step-up authentication, speed bumps, + deciding which effort to keep or remove.
- Open when designing/reviewing destructive, costly, broadcast or sensitive actions, confirmations, undo windows, step-up authentication, timeouts, any proposal to add or remove steps.

## Principles behind these patterns
|Principle|What it governs here|
|---|---|
|../principles/intentional.md|most: confirmation, type-to-confirm, graded friction, purchase confirmation, speed bumps on sharing, meaning-building effort, whose friction to remove, nudges only for person|
|../principles/resilient.md|delay-then-undo, context-aware validation, step-up authentication|
|../principles/inclusive.md|whose friction to remove|
|../principles/respectful.md|warning before timeouts + letting people extend|

## Grading friction to consequence

### Confirm this action or not?
- When: irreversible/high-consequence actions, e.g. permanent deletion, signing out everywhere, sending to many people, sharing sensitive data.
- Do: confirmation states what will happen; effort demanded scales w/ action's severity + reversibility.
- Avoid: one-tap irreversible actions; confirmations on trivial actions → train people to click through.
- Why: Intentional.
- Hypothetical: smart-home hub asks once more before factory-resetting every paired door lock + says which doors will stop responding.

### Does the action cost other people?
- When: action will interrupt, notify, expose or commit a group.
- Do: price cost to others: prompt names those affected + how many → decision made w/ cost in view.
- Why: such prompt does two jobs: stops accident + teaches norm. Person learns what their convenience costs others → then usually picks quieter route unprompted.
- Limit: confirmation naming only actor's own loss leaves everyone else's interrupted attention invisible + unpriced.
- Hypothetical: shared family calendar, before moving recurring dinner several relatives attend, says how many + names each relative whose plans get pushed + notified → change made w/ them in view.

### Catastrophic operation: what confirmation?
- When: catastrophic operations, e.g. wiping dataset, deleting organization, destroying audience list.
- Do: require typing specific word or name of thing destroyed (type-to-confirm).
- Avoid: reflexive, generic Are-you-sure prompt.
- Why: Intentional.
- Hypothetical: hospital research database asks analyst to type study's name before wiping its participant table.

### Same verb, different criticality: where does each control live?
- When: one verb (delete, toggle) applies to entities of very different criticality (grading friction by sensitivity).
- Do: harmless controls inline; moderately risky behind menu; dangerous inside detail view behind submenu, w/ explicit save + consequence message. Inline help for rare, high-impact tasks. Break interface consistency on purpose for dangerous actions.
- Avoid: uniform placement letting people act on autopilot; inline toggle for system-wide rule only because power user asked for speed.
- Why: Intentional.
- Hypothetical: retail chain's pricing console: "hide product" inline; "archive category" in row menu; "apply discount rule to all stores" in rule's detail view behind edit step, explicit save + note naming which stores change.

### Order or money transfer: what before it goes through?
- Do: show total; require explicit confirmation, gesture or biometric.
- Avoid: zero-click ordering.
- Why: Intentional.
- Case: voice assistants once placed orders in response to sentence spoken in broadcast. Single-press reorder hardware removed so much friction → people could not tell what they spent until charge appeared.
- Hypothetical: school-cafeteria top-up screen shows child's account, amount + card before press-and-hold confirm.

### Sensitive account action: is the current session enough?
- When: changing credentials, viewing stored passwords, moving funds, deleting account (step-up authentication).
- Do: require re-authentication/second factor even within active session. List active sessions + let people end them. After password change → offer to roll back recent profile edits.
- Avoid: existing session treated as authority for everything.
- Why: Resilient.
- Hypothetical: payroll portal asks fresh one-time code before changing salary-receiving bank account, even mid-session.

## Making mistakes recoverable

### Consequential send or submit: final at once?
- Do: hold action a few seconds + show cancel affordance before final (delay-then-undo window).
- Avoid: instant, unrecoverable sending.
- Why: Resilient.
- Hypothetical: job-application portal briefly holds just-submitted application w/ visible "withdraw" control before it reaches employer.

### Probable mistake: warn or block?
- When: content can reveal person's intent (context-aware validation).
- Do: flag probable mistakes, e.g. meeting scheduled in past, message mentioning attachment but carrying none. Warn + allow; do not block.
- Avoid: syntax-only validation; hard blocks on legitimate exceptions.
- Why: Resilient.
- Hypothetical: pharmacy refill app notes requested quantity far above person's usual refill, asks whether intended, still lets request through.

### Session about to expire?
- Do: announce expiry in advance; let people extend before expiry; offer stay-signed-in option.
- Avoid: silent session drops discarding half-completed form.
- Why: Respectful.
- Hypothetical: housing-application portal sends on-page notice well before session ends, offers more time w/ one tap, keeps half-filled answers, asks whether to stay signed in on this device.

## Friction that protects others

### Sharing and forwarding: add speed bumps?
- When: one-tap broadcast enables misinformation/pile-ons.
- Do: prompt people to open link before resharing; cap forwards; delay wide spread of unverified/viral content; restrict replies from brand-new accounts; throttle rapid-fire actions from one account.
- Avoid: unlimited, instant resharing optimized for exponential reach.
- Why: Intentional; misuse cases behind it: safety-and-abuse-resistance.md.
- Case: messaging service capped forwards after viral rumours contributed to violence.
- Hypothetical: neighbourhood-forum app asks member to open linked article before reposting + limits how many groups member can forward one post to at once.

## Choosing which effort to keep or remove

### Is this effort load-bearing?
- When: removing steps for conversion.
- Do: keep load-bearing effort: composing, choosing, committing, assembling. Remove only-tedious effort. When removing steps, aim for middle of friction-value curve.
- Avoid: automating away step where learning/ownership happens.
- Why: Intentional (designing for meaning-building effort).
- Case: peer-to-peer service saw sign-ups surge after replacing quick survey w/ required video call.
- Hypothetical: personal-budget app keeps monthly step where people sort own transactions into categories, since sorting = where they come to understand their spending.

### Whose friction is being removed?
- Do: when deciding which effort to engineer away → look at who carries it. Rank simplifications by cost to person carrying effort, not visibility to team.
- Avoid: every removed step treated as equally valuable; a quarter spent on conveniences for comfortable people presented as easing life for everyone.
- Why: Intentional + Inclusive. Much product work smooths minor inconveniences for people whose lives already run easily. Heavy barriers stay because people meeting them not counted as market: form people cannot finish w/o bank account, service assuming car ownership, flow collapsing on cheap phone/slow connection.
- Bound: accessibility floors + low-end devices: inclusive-and-accessible-design.md.
- Hypothetical: city benefits office, choosing between faster autofill for returning online applicants + payment route for applicants w/o bank account, ranks second higher: those applicants carry heavier cost.

### May friction steer a choice?
- When: shaping healthier choice.
- Do: small added effort on less healthy option + better option visible; every option stays available.
- Avoid: friction nudge serving business rather than person → treat as deceptive pattern + remove (../ethics/deceptive-patterns.md); same friction techniques steering toward upgrades/data sharing.
- Why: Intentional (friction nudges only when they benefit person).
- Hypothetical: sleep app puts wind-down audio on late-evening home screen + moves high-energy playlists one tap deeper; both still play.

## Related
- errors-and-input-tolerance.md: usability side of error prevention + recovery, tolerant input, destructive actions.
- forms-and-data-entry.md: usability side of validation timing, checkout, payment failure.
- defaults-and-choice-architecture.md: equal-weight decline + symmetric exit, where effort must not block leaving.
- [Convenience and friction evidence](../evidence/convenience-and-friction.md): what removing/adding friction does.
- ../ethics/deceptive-patterns.md: where nudge serving business belongs.
- safety-and-abuse-resistance.md: misuse cases behind speed bumps on sharing.
- inclusive-and-accessible-design.md: accessibility floors + low-end devices, for deciding whose friction to remove.
- ../principles/intentional.md: principle most friction patterns serve.
- ../principles/resilient.md: undo windows, validation, step-up authentication.
- ai-and-automated-features.md: agent confirmation follows same consequence scale.
