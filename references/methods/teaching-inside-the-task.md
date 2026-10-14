# Teaching inside the task (onboarding for people who skip manuals)

## Use when
- Designing / reviewing first use, onboarding, product tours, in-product guidance.
- Aim: build first use around learning by doing; 8 steps.

## Basis
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|First-time users went straight to work, tolerating resulting stuck points + mistakes, instead of opening bundled documentation|1987 user studies|—|design for people starting to act immediately|
|Front-loaded product tours of sequential overlays skipped by most users|—|"most", not all|drop mandatory up-front tours|

## Steps
1. **Let users act immediately.** Drop mandatory product tours up front, before use.
2. **No single prescribed onboarding flow.** People take different routes + reach different stages → help at hand on every one.
3. **Well-timed, lightweight discovery** = context-tied tooltips.
4. **Progressive onboarding.** Show one core action alone, teach it w/o risk, hold every other feature back → reveal each as previous one mastered.
5. **Revisitable "get started" template or checklist** teaching via real use; also keeps open-ended possibilities from swamping new users.
6. **Design for real, often irrational behaviour**, not idealized user reading everything.
7. **Bring first real success (activation action) as early as possible.** Peak-End Rule applies here, not at tour's end.
8. **Check accessibility + ethics** (checks below).

## Cases
|Product|What it did|Step|
|---|---|---|
|Slack|onboarding bot had newcomers practise messaging w/ only message input visible|4|
|Notion|revisitable get-started template teaching by real use|5|

## Checks (step 8)
|Check|Passes when|Law / principle|
|---|---|---|
|Tours reachable|keyboard + screen reader can reach tours|accessibility floor|
|Focus returned|focus goes back when tour closes|↑|
|Motion|reduced-motion settings honored|↑|
|Value first|value delivered before sign-up|ethics|
|No confirmshaming|none anywhere in onboarding|ethics; deceptive patterns|
|Permission in context|notification permission asked in context|ethics|
|Easy exit from re-engagement|every re-engagement message has one-tap opt-out|ethics|

## Decision rules
- If people must click through tour before first use → remove requirement; let people act.
- If guidance exists only in one fixed flow → make it reachable from any path + stage.
- If many features revealed at first use → hold all but one core action back; reveal on mastery.
- If onboarding "peak" planned at tour's last screen → move effort to first real success.

## Hypothetical example
- Hypothetical: payroll tool for small shops opens on one action, "pay one employee", w/ sample employee to practise on + nothing else visible. Other features appear one by one, each once previous one mastered. Get-started checklist reachable from help menu at any point, + first real payslip produced = moment product celebrates.

## Related
- ../laws/paradox-of-the-active-user.md: law behind basis; people start work straight away + leave manuals unopened.
- ../patterns/onboarding-and-first-use.md: entries for first-run experience, tours, empty states, activation + re-engagement nudges.
- activation-moment.md: locates step 7's first real success + measures path to it.
- ../laws/peak-end-rule.md: law applied at step 7's first real success.
- ../patterns/inclusive-and-accessible-design.md: accessibility floors behind step 8 check.
- ../ethics/deceptive-patterns.md: confirmshaming + other named patterns kept out of onboarding.
- ../patterns/notifications-and-interruptions.md: asking permission in context; what interrupts, when, under whose control.
