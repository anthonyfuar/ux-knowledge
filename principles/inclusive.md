# Inclusive

## In one line
- Inclusive = every variation in people's ability, context, culture, class, language + mental state in scope.
- Leaves nobody out across any difference: serves people in all their differences + takes its material from them too.
- Inclusion = method of working, not compliance state.
- Open when: design/review touches accessibility, assumptions about ability, context, device, language or emotional state, minors, or team + room composition when decisions made.

## Core practices
Highest weight; check first.
1. Build diverse teams + retain them.
2. Start from disability → extend across permanent, temporary + situational limits.
3. Keep platform's reduced-motion, text-scaling, contrast + zoom settings working.
4. Readable copy, honest error states + undo for anxious people.
5. Co-design w/ excluded people holding decision power.
6. Stricter defaults for minors.

## Commitments w/ a pattern entry
|Commitment|Do|Avoid|Entry|
|---|---|---|---|
|Persona spectrum|map one problem across permanent, temporary + situational limitation||../patterns/inclusive-and-accessible-design.md|
|Disability as starting point|take disabled people's needs as opening constraint → widen solution to everyone||same|
|Platform controls|preserve platform's accessibility controls||same|
|Motion + feeds|let people switch off motion + endless feeds||same|
|Structure|native semantics + keyboard-first structure||same|
|Type + colour|legible type + generous contrast|meaning carried by colour alone|same|
|Text|readable text as default||same|
|Devices + networks|design for commonest device + slowest connection||same|
|Emotional state|account for anxiety + emotional state||same|
|Essential tasks|two channels for every essential task||same|
|Co-design|w/ excluded people, compensated + holding decision power||same|
|Indirect users|design for indirect users + fragile contexts||same|
|Quiet signals|communicate w/o speaking; show minimum||../patterns/calm-technology-and-device-etiquette.md|
|Minors|age-aware defaults; protect minors from persuasive design||../patterns/safety-and-abuse-resistance.md|

## Guidance held here (no pattern entry)

### Staffing the team?
- Do: staff for varied abilities, backgrounds, ages + lived experience.
- Step: at kickoff, audit room composition.
- Do: retain + promote diverse staff, not only hire them.
- Team representation does more than empathy exercise.

### Offering content in one form?
- Rule: person decides how to consume content. Provide text alternatives, captions, transcripts, adjustable playback, layout + input preferences.
- Rule: alternative paths equivalent to main one, not merely compliant.
- Limit: automatic captions can meet legal bar + still stay unreadable for bilingual deaf viewers.

### Looking for worst cases + who is left out?
1. Ask "what is the worst case, and on whom?" → brainstorm worst outcomes w/ mixed group before strategy fixed.
2. Write "all people can..." statements about product → find people for whom each fails.
3. Keep standing worst-case review loop w/ named owner.
- Rule: intent does not cancel impact.

### Product may be used by minors?
- Identify minors w/ least data possible, from signals already held: age given at sign-up, account created as child's, parent-linked/family plan, school deployment.
- Treat result as approximate.
- If age unknown/doubtful → protective default, not permissive one.
- Avoid: demanding identity document, face scan or payment card as price of weaker (less protective) setting. Why: demanding age proof trades everyone's privacy for one product's certainty about a few people.
- Make protected experience good enough to live in → nobody pushed into lying about age.
- Bind age signal to its single purpose; keep it out of ranking + advertising.
- Adults placed in protected state can correct it w/o proving anything more.

### Verifying accessibility?
1. Test in real assistive contexts: screen reader, keyboard-only use, 200 percent zoom + contrast checks belong in release checklist.
2. Run automated accessibility checks on every commit.
3. Run trials under poor conditions.
- Rule: good intentions don't verify accessibility.

## Why it matters
- Disability arises from mismatch between person + design.
- Disability = mismatch → every product decision either excludes or includes; designers can remove mismatches they created.
- Same constraint one person has permanently recurs temporarily + situationally for others.
- Hypothetical: voice-only banking assistant shuts out customer w/o speech (permanent), one w/ laryngitis (temporary) + one in silent library (situational).
- Everyone tends to end up using solutions built from permanent limitation.
- Problem addressed: self-referential design: teams w/ big screens, fast connections + calm minds build for people like themselves.

## Key concepts
|Term|Meaning|
|---|---|
|Mismatch|exclusion = design assumptions not fitting person; mismatches = units designers can remedy|
|Persona spectrum|one design problem viewed across permanent, temporary + situational limitation|
|Solve for one, extend to many|broad benefit from constraints solved for strongest case|
|POUR|perceivable, operable, understandable, robust: four principles of web accessibility standard|
|Intent vs impact|what team hoped for vs how real communities experience work|
|Target source vs excluded source|intended audience vs communities affected by product but never considered|
|Stress cases|replaces term "edge cases" so extremes get tested, not ignored|

## Audit questions
Scope: people in all their variety. All principles' questions → ../checklists/humane-design-audit.md.

|Check|Passes when|
|---|---|
|Team reflects diversity of abilities, backgrounds + lived experience?|actual representation, not empathy exercises|
|Disability taken as starting constraint + assistive contexts tested?|keyboard-only use, screen reader, 200% zoom + visible focus|
|Platform accessibility preserved?|text-size scaling, contrast settings + pinch-zoom all left working|
|Can people switch off motion, parallax + endless feeds?|reduced-motion + paginated alternatives|
|Product works for permanent, temporary + situational limitations?|works one-handed, in glare, in noise, in second language, w/ anxiety + on low bandwidth|
|Errors honest about whose fault + give next step?|no generic "something went wrong" reading as person's own failure|
|Defaults stricter for minors?|no late-night push notifications, autoplay off, break reminders on|

## Neighbours to check
- Check alongside: intentional.md, finite.md, resilient.md.
- Working w/ neighbours → [Principles index](index.md).

## Related
- ../patterns/inclusive-and-accessible-design.md: when/do/avoid entries for most Inclusive practices: persona spectrum, accessibility floors, low-end devices, identity.
- ../patterns/safety-and-abuse-resistance.md: entries on children, vulnerable people + misuse cases.
- ../patterns/calm-technology-and-device-etiquette.md: entry on communicating w/o speaking + quiet signalling.
- ../evidence/inclusion-and-exclusion-costs.md: evidence on people left out + exclusion's cost.
- ../evidence/children-and-adolescents.md: evidence on effects on minors + age-appropriate design.
- ../patterns/forms-and-data-entry.md: usability side: validation timing + accessible errors.
- ../methods/testing-touch-layouts.md: usability side: touch targets tested under real grip + context.
- ../guides/laws-and-principles-crosswalk.md: psychological lever each principle guards + principle bounding each law.
- ../checklists/humane-design-audit.md: audit questions for all seven principles together.
- [Principles index](index.md): seven principles side by side + how to work w/ neighbours.
- Pattern files tagged Inclusive: ../patterns/ai-and-automated-features.md, ../patterns/notifications-and-interruptions.md, ../patterns/friction-undo-and-confirmation.md, ../patterns/calm-technology-and-device-etiquette.md, ../patterns/inclusive-and-accessible-design.md, ../patterns/safety-and-abuse-resistance.md, ../patterns/habits-streaks-and-gamification.md.
