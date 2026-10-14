# Errors and input tolerance

## Scope
- Error prevention + recovery: tolerant input, open intake into systems of work, real + extreme content, limits stated at input, stress states, context restored after failure, destructive actions, corrections, failure messages.
- Open when designing/reviewing input parsing, validation, error/outage states, deletion/irreversible actions, recovery after failure, corrections, layouts surviving real data.

## Laws and principle behind these patterns
|Law / principle|Role here|
|---|---|
|[Postel's Law (Robustness Principle)](../laws/postels-law.md)|accept liberally, emit cleanly|
|../laws/teslers-law.md|who absorbs tolerant-input complexity|
|../laws/paradox-of-the-active-user.md|errors from people reading nothing first|
|../laws/peak-end-rule.md|failure streaks + outages as negative peaks + endings|
|../laws/fittss-law.md|mis-tap prevention, target size + spacing|
|../laws/cognitive-bias.md|belief perseverance, risk compensation|
|../principles/resilient.md|humane bound on recovery, reversibility + failure states|

## Taking input in

### Accept messy input or reject it?
- When: parsing dates, phone numbers, names, addresses, free text.
- Do: accept varied input forms → convert to system format; tell user clearly what happened to it. Keep acceptable-input limits clear.
- Avoid: rejecting unambiguous input. Also accepting unclear input: leniency only if meaning clear.
- Origin: Postel's Law (Robustness Principle) began as TCP rule: receiver accepts specification-breaking input if meaning stays clear; sender follows specification fully.
- Who does the work: ../methods/who-absorbs-complexity.md splits tolerant-input work between system + user (Tesler's Law).
- Hypothetical: airline passenger form accepts birth date as words, slashes or dots, echoes it in one standard format for traveller to confirm; re-asks only when day + month could trade places.

### How open should intake into a system of work be?
- When: many channels/teams feed one system, e.g. support tickets via email, phone, apps + voice, or design-system contributions (Postel's Law for systems of work).
- Do: accept liberally, from any team + in any form (code, designs, content, criticism) → one well-defined output, e.g. single usable ticket, or clear guidelines, patterns + code fitting people's workflows.
- Why: open intake → contributors feel heard; system meets its worst real use cases; ownership spreads; organization-wide themes surface.
- Evidence: policing rigid system tends to provoke workarounds (2016 practitioner reflection on design systems).
- Hypothetical: city maintenance desk takes pothole reports by phone, web form, photo message + walk-in note → each becomes one standard work order w/ location, photo + urgency.

### When and how to state limits and validate?
- When: people read nothing first + set to work at once (Paradox of the Active User).
- Do: graceful recovery on any path. State limits (size, file count, timeout, format) at input, not after failure. Validate early. Retry paths for slow connections. Validate per finished input unit (whole phone number, whole field), not mid-entry. Report results within 2–4 s (1968 response-time research).
- Why: skipped instructions → dead ends + errors. Errors reported mid-entry break chunk person holds in mind.
- Case: one hosted form service allows one file per field, 8 MB per request + 30-second upload timeout → file under size cap can still fail.
- Hypothetical: university admissions upload field states accepted formats, size cap + time allowed next to button; stalled upload offers resume, not blank error.

## Real and extreme content

### Will the layout survive real data?
- When: planning states + scenarios (anticipating surprises).
- Do: design for almost every capability level, access method + input; any input → output stays accessible + dependable; layouts survive messy real data. Build test data from extremes of existing data: longest, shortest, ugliest items. Test over-limit headlines, missing images, odd aspect ratios, varying item counts, narrow viewports, larger default font sizes. Organization's own content → fix outliers editorially + record limits in style guide.
- Localization from first layout: allow longer strings; some teams test layouts w/ placeholder text twice source length, for languages like German; right-to-left languages as mirrored layout; capitalization in source strings, not styling.
- Avoid: ideal placeholder content (short names, studio headshots) → hides breakpoints until launch.
- Why: resilience grows w/ each case planned for. Enlarged text can trigger mobile layouts on desktop. Aim = garbage in, not bad out: messy input must not produce broken result.
- Bound: accessibility floors + low-end devices: inclusive-and-accessible-design.md.
- Case: 2018 content audit: list titles 8 to over 320 characters long, only a handful above 80; team designed for 80 characters + edited outliers → titles read better.
- Hypothetical: hotel-booking cards tested before launch w/ longest property names, rooms w/o photos, portrait-only images + Arabic translation.

## When something fails

### What does a stress state show?
- When: errors, payment failures, security alerts, medical/emergency flows (make stress states demand least memory).
- Do: problem, user's input + next step visible together; one clear recovery path, every step reversible. Interleave easier steps among hard ones → no failure streak. Let people resolve all errors in one pass.
- Avoid: disappearing messages; instructions shown once then hidden; recovery needing remembered codes/earlier screens.
- Why: stress quickly weakens working memory. Streak-end rule: failure streaks (consecutive errors/rejections), especially as final event, act like peaks in remembered experience.
- Hypothetical: home-alarm app, after failed disarm, keeps alert, code field + "call monitoring centre" on one screen, every remaining field error listed at once.

### What is restored after a crash or timeout?
- Do: after crashes, timeouts/lost connections → keep + quickly restore last query, position/model state. State recovery time at once.
- Avoid: losing people's creative work on failure.
- Bound: 1968 response-time research: restore context ≤ 15 s, else ≤ 5 minutes.
- Why: lost work felt as personal failure → users avoid system.
- Hypothetical: benefits application keeps every answered page when connection drops + reopens on same question after sign-in.

### How does a failure message read?
- When: decisions overlooking some users, bugs, missing pages, outages (turning failures into rapport).
- Do: fallbacks expressing brand's personality → softens negative peak. Say plainly what went wrong + realistic recovery time. Never blame user. Calm styling when user can do nothing about it.
- Avoid: red alarm styling + try-again-later w/o explanation/estimate → implies user must act; creates negative peak + ending at once.
- Why: bad moments leave sharper memories than good ones. Outage may end session → can become remembered ending (Peak-End Rule).
- Case: one music-streaming service's outage message: red alarm styling + try-again-later w/ no explanation or estimate.
- Hypothetical: children's library app, while catalogue server down, shows mascot stacking books in calm colours, says plainly catalogue unavailable + when team expects it back, asks nothing of reader.

## Destructive and consequential actions

### How much friction before committing?
- When: destructive, irreversible/consequential actions follow flexible input (accept liberally, commit conservatively).
- Do: routine actions fast. Friction only where mistakes expensive, proportional to risk: confirmation summaries stating consequences plainly, least-destructive default, typing resource name for rare, hard-to-reverse changes. Prefer reversibility (even simulated undo) + physically separated destructive controls over Are-you-sure dialogs. Keep remaining risk visible even when safety nets exist.
- Avoid: confirming every routine action; routine typed confirmations → both lead to mindless clicking/typing. Accepting almost anything when destructive results neither confirmed nor reversible.
- Why: vigilance cannot last → protection belongs at risky moment. Safety nets can reduce people's care (risk compensation).
- Hypothetical: warehouse inventory tool: staff adjust counts freely, but before writing off whole stock location → summary of items lost + dialog defaults to "cancel".

### How to prevent mis-taps?
- Do: enlarge + separate destructive/adjacent targets.
- Why: errors rise when small target approached fast.
- Misreading: Wrong: slip onto adjacent button = Fitts's Law problem → Right: frame it as error prevention + spacing; Fitts's Law explains movement time, not which of two neighbouring targets gets hit.
- Hypothetical: smart-thermostat app moves "turn off heating" away from "set schedule" + enlarges both targets.

### Routine deletion: undo, soft delete or confirm?
- Do: prefer undo (toast/inline Undo staying long enough, not vanishing in a few seconds) + soft delete (trash, archive, recovery window) over confirmation dialogs. Confirm only truly irreversible, rare or others-affecting actions. Deletion confirmation names object + consequence; button labelled w/ action (e.g. Delete 3 files), not OK. Destructive controls away from frequent ones, visually distinct, never default.
- Avoid: Are-you-sure prompt on every action; hard delete w/o recovery for user-created content; bulk actions w/o count + preview.
- Caveat: for undo-first handling of destructive actions, cite error-prevention usability heuristic; no timing/motor law covers it (../checklists/usability-heuristics-map.md).
- Hypothetical: recipe app deletes saved recipe at once w/ Undo bar staying until dismissed + keeps it in "recently deleted"; emptying folder asks "Permanently delete these recipes?" w/ count shown.

## Correcting what people believe

### How to correct a wrong impression?
- When: correcting wrong mental model, misleading message or content mistake.
- Do: give replacing explanation, not only retraction. Prevent wrong first impressions rather than rely on later fixes. After error, restore people's confidence in affected feature.
- Why: belief perseverance + continued influence effect → prevent, not fix later. People avoid once-bad choice even when now right.
- Evidence:

|Finding|Study|Design consequence|
|---|---|---|
|~half of induced belief survived after participants debriefed|one study|prevent wrong first impressions rather than rely on later fixes|
|No backfire effect|study of 10,100 participants across 52 issues|do not withhold corrections for fear of backfire|

- Hypothetical: bank app wrongly showed fee → says correct charge + why first figure appeared, then marks fee screen fixed → customers trust it again.

## Related
- friction-undo-and-confirmation.md: humane side: consequence-graded confirmation, undo windows, speed bumps.
- forms-and-data-entry.md: fields, formats, validation timing, payment failure, accessible errors.
- calls-to-action-and-touch-targets.md: target size, spacing + placement behind mis-tap prevention.
- memorable-moments-and-endings.md: failure moments designed as peaks + endings.
- ../checklists/usability-heuristics-map.md: error-prevention heuristic to cite where no law explains problem.
- inclusive-and-accessible-design.md: accessibility floors + low-end devices bounding design for any input, access method, capability level.
- ../principles/resilient.md: humane principle bounding recovery, reversibility, failure states.
- ../methods/who-absorbs-complexity.md: allocates tolerant-input work between system + user.
- ../laws/postels-law.md: robustness rule behind tolerant input.
