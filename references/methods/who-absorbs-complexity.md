# Deciding who absorbs complexity (Tesler's Law applied)

## Use when
- Allocating task's irreducible complexity between system + user, as Tesler's Law requires; 10 steps, from listing irreducible core to justifying engineering cost.

## Steps
1. **List task's irreducible core.**
2. **Assign each piece explicitly**: system / user. Default = system + builders carry it.
3. **Shift complexity to system** w/ one technique below.
4. **Handle rest w/ progressive disclosure**: essentials shown by default, advanced options one layer down.
5. **Stop simplifying before it turns into abstraction**; keep meaning visible.
6. **Contextual help for active users.**
7. **Expect counterpoint**: users' overall complexity may not drop, because effort freed by simpler task goes to more ambitious work.
8. **Place product on control continuum**, from full automation to full manual. Factors: device type, activity frequency + complexity, user expertise, market positioning, intended emotional tone.
9. **Give every automated step** smart default + system-state communication + failure path (support, diagnosis, instructions).
10. **Justify moving work to engineers w/ cost estimate, not dogma**: frequency × active users × cost per encounter.

## Complexity-shifting techniques (step 3)
|Technique|Hypothetical instance|
|---|---|
|Reuse data already given|Hypothetical: home-insurance claim form fills incident address from policy address once person confirms damage at home|
|Fill in known data ahead of time|Hypothetical: IT-support ticket form enters requester's name + department from sign-in|
|Suggestions drawn from history|Hypothetical: same ticket form proposes devices this person reported before|
|Stored credentials|Hypothetical: train-booking app holds traveller's railcard + payment card → repeat booking goes through w/o retyping either|
|Automate whole step|Hypothetical: hospital supply room logs each item nurse carries out via shelf sensors + camera recognition → no scan-out step left|
|AI assistance|Hypothetical: clinic's patient-messaging tool drafts short candidate replies + offers endings for nurse's half-typed sentence|
|Intent-based natural-language interaction (feature-rich products)|Hypothetical: school district's attendance tool answers typed everyday-words question, w/o any filter setup|

## Decision rules
- If deciding carrier of core piece → start from default (system + builders carry it) + record choice explicitly.
- If simplification hides what action means → stop; abstraction, not simplicity.
- If active users get stuck mid-task → contextual help (step 6).
- If automated step has no failure path → add one: support, diagnosis + instructions.
- If objection = engineering cost → multiply frequency × active users × cost per encounter + compare; argue from number.
- If product got simpler but users' total load seems unchanged → consistent w/ counterpoint (step 7): users may have moved on to more ambitious work.

## Pitfalls
|Symptom|Likely cause|Fix|
|---|---|---|
|Users re-enter data system already has|complexity left w/ user|reuse / prefill / suggest|
|Advanced options crowd main screen|no progressive disclosure|essentials first, advanced one layer down|
|Clean screen nobody understands|simplified into abstraction|restore visible meaning|
|Automation fails silently|no state communication / failure path|step 9|
|Debate stuck on principle|no cost estimate|step 10 arithmetic|

## Hypothetical examples
- Hypothetical (irreducible core): bank transfer cannot exist w/o payee account + amount; these two pieces = its core.
- Hypothetical (one layer down): home-thermostat app shows target temperature + weekly schedule on main screen; sensor calibration + humidity offsets sit behind "Advanced" expandable section.

## Related
- ../laws/teslers-law.md: law behind method, w/ origin, pitfalls + counterpoint.
- ../patterns/complexity-management.md: patterns: complexity's bearer, progressive disclosure, settings pages, expert tools.
- [AI, assistants and automated features](../patterns/ai-and-automated-features.md): AI assistance, intent-based interaction, automation hand-over, human review.
- ../laws/paradox-of-the-active-user.md: law behind contextual help for active users (step 6).
- thresholds-and-formulas.md: measurable form of step 10 cost estimate.
- [Justifying design decisions to stakeholders](stakeholder-arguments.md): cost arithmetic as stakeholder argument.
- ../patterns/defaults-and-choice-architecture.md: humane bound on step 9 smart defaults; defaults as honest, beneficial suggestions.
- ../principles/empowering.md: humane bound on automation; augmentation, not substitution, w/ people kept in charge.
