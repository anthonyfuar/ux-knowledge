# Resilient

## In one line
- Resilient = abuse taken as given; whoever stands to get hurt most designed for first.
- Abusability = how easily one person can harm another w/ product; successor to usability.
- Rule: put people most exposed to harm first + assume someone will try to turn product against another person.
- Product can pass every usability measure + still serve as weapon.
- Open when: design/review touches misuse + abuse, blocking/muting/reporting, location/monitoring features, account takeover, failure states, vulnerable people or children.

## Core practices
Highest weight; check first.
1. Misuse case + abuser persona beside every use case.
2. Threat-model intimate partner sharing home + passcode.
3. Personal privacy settings always beat group, admin + automated actions.
4. Block, mute, report + appeal loops fully specified.
5. Graceful degradation + route to human.
6. Recommenders guardrailed around signals of distress.

## Commitments w/ a pattern or method entry
|Commitment|Do|Avoid|Entry|
|---|---|---|---|
|Community moderation|block, mute, report, comment filtering, audience restriction||../patterns/safety-and-abuse-resistance.md|
|Moderation semantics|specify exactly what block, mute + restrict do in each direction||same|
|Reporting loop|full loop incl. appeal; explanations prompt + specific||same|
|Misuse cases|misuse case + abuser persona beside every use case||same|
|Happy path|start from happy path centred on vulnerable person||same|
|Counting|count people|percentages|same|
|Intimate partner|threat-model intimate partner||same|
|Harm window|shrink harm window; safety signals reach every sense + every platform|causing alert fatigue|same|
|Stop + report|discreet way to stop + report||same|
|Doxxing surface|audit doxxing surface, incl. removed notifications + aggregate views||same|
|Expansion|assess institutional fragility before expanding||same|
|Hate|refuse to serve as platform for hate; safety over speech; act on values, not only policy||same|
|Children|protect children from persuasive design||same|
|Privacy precedence|personal privacy settings override group, admin + automated actions||../patterns/defaults-and-choice-architecture.md|
|Recommenders|guardrail around sensitive states; counter rabbit hole||../patterns/recommendations-and-personalization.md|
|Failure|work even when failing; test under sub-optimal conditions||../patterns/calm-technology-and-device-etiquette.md|
|Gates|apply three-gate check||../methods/three-gate-check.md; process patterns → ../methods/process-safeguards.md|

## Guidance held here (no pattern entry)

### Reading the numbers?
- Rule: numbers need fieldwork beside them → pair analytics w/ interviews + observation.
- Step: after every test, segment results by population.
- Step: sit w/ support staff.
- Limit: analytics show what happened; reason behind it absent from numbers.
- Limit: average creates illusion of knowledge.

### Account could be taken over?
- Do: make takeover visible + reversible: list active sessions.
- Do: challenge sensitive account changes w/ second factor.
- Do: after password reset, offer undo of recent account changes.
- Why: w/ visible sessions, second-factor challenges + post-reset undo, intruder meets resistance before doing damage.

### Growth vs known harms?
- Rule: known harm still open → pause growth work until resolved.
- Do: keep watching product after launch.
- Measure: instrument abuse alongside growth: unanswered first messages, blocks, false positives.
- Why: speed at scale magnifies damage to those least able to absorb it.

### Platform + data choices?
- Do: favour open standards: interoperability + data portability over lock-in.
- Do: validate against projected future populations + climate, not only today's logs.

### Someone on staff raises a harm?
- Do: provide retaliation-free channels for staff raising harms (protect internal dissent).
- Do: know escalation + whistleblowing routes.
- Why: punishing warnings discards earliest chance to fix problem.

## Why it matters
- Problem addressed: happy-path development at speed + scale, by definition serving least vulnerable.
- Dismissing people as edge cases marginalizes them.
- Scale: 1% of two billion accounts = twenty million people.
- Designing for most vulnerable protects everyone; reverse does not hold.

## Key concepts
|Term|Meaning|
|---|---|
|Abusability|evaluate w/ same rigour as usability|
|Happy path vs path of most resilience|frictionless scenario vs scenario written around most vulnerable person|
|Technical vs contextual edge cases|flow failures QA can test vs harmful behavioural deviations, e.g. non-consensual content|
|Harm window|time from harmful action starting to affected person getting told|
|Harm taxonomy|physical (sleep loss, financial strain, exposed location); emotional (betrayed trust, self-image); societal (polarization, exclusion, reinforced bias)|
|Five harmful incentives|engagement; careless experimentation; automation + scale; neutrality; reckless speed|
|Graceful degradation|baseline usability retained when power, connectivity, servers or person fail|

## Tracking + monitoring features
- Amplified coercive control: tracking, monitoring or location capability almost never first act of abuse.
- Tracking capability arrives inside existing pattern of control + raises its accuracy, reach + endurance.
- Wrong question: could this feature create stalkers?
- Right questions: how much capability does feature hand someone already watching their partner? How much of other person's routine can be reconstructed? How long until they find out?
- Trusted mainstream brand lowers abuser's own sense of doing wrong → warning at setup matters as much as alert later.

## Audit questions
Scope: abuse expected, vulnerable shielded. All principles' questions → ../checklists/humane-design-audit.md.

|Check|Passes when|
|---|---|
|Every use case has written misuse case + mitigation at launch?|misuse case not deferred to never-arriving "later"|
|Audience for person's information theirs to set, w/ safest default?|personal settings always override group + admin actions|
|Block, mute, report + appeal specified in each direction?|acknowledgement, decision + recourse; abusers cannot weaponize reporting tool itself|
|Safeguards survive attacker sharing home, passcode or account?|intimate-partner threat model, not stranger-only one|
|Doxxing surface audited so no combination of fields locates or identifies anyone?|aggregation checked across profile, activity + metadata; fields w/o justification dropped|
|Product degrades gracefully when battery, network or servers fail?|offline mode, low-speed mode + route to human|
|Abuse instrumented beside growth?|unreplied first messages, block-after-message rates + moderation false positives measured|
|Quantitative findings checked against interviews, observed sessions + support tickets?|results segmented after every experiment; product staff have sat w/ support queue. Why: why behind behaviour comes from people alone; numbers only record their actions|

## Neighbours to check
- Check alongside: respectful.md, finite.md, inclusive.md.
- Working w/ neighbours → [Principles index](index.md).

## Related
- ../patterns/safety-and-abuse-resistance.md: when/do/avoid entries for most Resilient practices: misuse cases, blocking + reporting, vulnerable people, children.
- ../methods/misuse-case-brainstorming.md: lists how people could misuse feature to harm.
- ../evidence/safety-and-abuse.md: evidence on harassment, stalking + intimate-partner abuse through products.
- ../patterns/calm-technology-and-device-etiquette.md: entries on working even when failing + testing under sub-optimal conditions.
- ../patterns/recommendations-and-personalization.md: entries on rabbit holes + sensitive states.
- ../patterns/privacy-data-and-security.md: data minimisation, consent, access + deletion, tracking.
- ../patterns/errors-and-input-tolerance.md: usability side: error recovery + edge cases.
- ../guides/laws-and-principles-crosswalk.md: psychological lever each principle guards + principle bounding each law.
- ../checklists/humane-design-audit.md: audit questions for all seven principles together.
- [Principles index](index.md): seven principles side by side + how to work w/ neighbours.
- Pattern files tagged Resilient: ../patterns/ai-and-automated-features.md, ../patterns/recommendations-and-personalization.md, ../patterns/feeds-scrolling-and-pacing.md, ../patterns/defaults-and-choice-architecture.md, ../patterns/friction-undo-and-confirmation.md, ../patterns/privacy-data-and-security.md, ../patterns/calm-technology-and-device-etiquette.md, ../patterns/inclusive-and-accessible-design.md, ../patterns/safety-and-abuse-resistance.md, ../patterns/monetization-and-growth.md, ../patterns/habits-streaks-and-gamification.md.
