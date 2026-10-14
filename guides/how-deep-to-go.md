# How deep to go

Sizes humane pass before design / review starts. Three tiers: quick pass, standard review, full treatment; each states scope, what to run, required answer.

## Ground rules

- Pick tier before design / review starts.
- Tier set by what feature does; never by mood / team's feelings about it.
- Naming tier = commitment to its required output; tier declared w/o all required parts counts as not run.
- Tiers size humane pass only: its steps in design-a-screen-or-flow.md (new feature) + review-an-interface.md (existing flow).
- Usability-pass steps of both guides not sized by tiers.

## Pick the tier

1. Feature can locate, record, expose / contact someone? Minors can use it? Money moves? Ranks / recommends? Acts autonomously? Reaches large population? → any yes = **Full treatment**.
2. Else: any new people-facing feature / any existing flow under audit → **Standard review**.
3. Else: internal tool / small change; nothing new collected, interrupted / exposed → **Quick pass**.
4. Any uncomfortable quick-pass answer → escalate one tier.

## Are the quick tables enough?

- If quick pass / naming deceptive pattern / product-ethics question → guides + quick tables suffice alone: [principles index](../principles/index.md) (seven humane-design principles) + ../ethics/anti-patterns-and-humane-alternatives.md.
- Product-ethics question → answer w/ answer-an-ethics-question.md.
- If feature ranks, collects data, charges money, acts on its own / reaches minors → guides + quick tables not enough: open detailed principle, pattern, method + evidence files at tier set by table below.

## Tier table

|Tier|Applies to|Run|Answer must contain|
|---|---|---|---|
|Quick pass|internal tools + small changes; nothing new collected, interrupted / exposed|5 questions, no workflow|5 answers + tier decision + reason to escalate / not|
|Standard review|any new people-facing feature; any existing flow under audit|new feature: design guide's 4 humane-pass steps; existing flow: review guide's whole humane pass|findings in fixed shape, each naming principle set + what happens to person; named pattern where one exists; every default justified; each growth metric paired w/ user-goal metric + counter-metric|
|Full treatment|can locate, record, expose / contact someone; minors can use it; money moves; ranks / recommends; acts autonomously; reaches large population|design guide's humane pass, all six steps, incl. foresight methods + launch gate|full standard-review answer + full-treatment extras|

## Quick pass: the 5 questions

|#|Question|Uncomfortable answer → open next|
|---|---|---|
|1|What is the default?|../patterns/defaults-and-choice-architecture.md|
|2|What does it interrupt?|../patterns/notifications-and-interruptions.md + ../checklists/interruption-decision-rules.md|
|3|What does it collect?|../patterns/privacy-data-and-security.md|
|4|How does someone leave?|../patterns/defaults-and-choice-architecture.md (symmetric exit) + [deceptive-pattern taxonomy](../ethics/deceptive-patterns.md)|
|5|Who is the most vulnerable person it touches?|../patterns/safety-and-abuse-resistance.md + ../principles/resilient.md|

- Any uncomfortable answer → escalate one tier; each question's next file = last column.
- Output: 5 answers + tier decision + reason to escalate / not.

## Standard review

|Route|Steps run|Where|
|---|---|---|
|New feature|Locate surface → Attention-hijack check → Pick patterns → Defaults + metrics|design guide steps 3, 4, 7, 13 = 1st, 2nd, 4th + 5th of six humane-pass steps|
|Existing flow under audit|whole humane pass|review guide steps 2, 3, 7, 8, 10|

- Both routes: surface list = ../principles/surface-to-principle-map.md; matching pattern files via [pattern catalog](../patterns/index.md).
- Existing-flow route: yes/no questions per principle from ../checklists/humane-design-audit.md.

Answer passes when:
- findings in fixed shape of write-a-finding.md;
- each finding names principle set + what happens to person;
- named pattern wherever one exists;
- every default justified;
- each growth metric has user-goal metric + counter-metric beside it.

Order findings + severities by ranking in core-stance.md.

## Full treatment

Design-guide humane pass, end to end:

|Design-guide step|Humane-pass step|Name|Standard review (new feature)|Full treatment|
|---|---|---|---|---|
|3|1st|Locate surface|yes|yes|
|4|2nd|Attention-hijack check|yes|yes|
|5|3rd|Forecast before building (foresight methods)|no|yes|
|7|4th|Pick patterns|yes|yes|
|13|5th|Defaults + metrics|yes|yes|
|15|6th|Gate the launch (launch gate)|no|yes|

Answer = full standard-review answer, plus:
1. Second-order chain / futures wheel, 3 levels out: ../methods/second-order-thinking.md, ../methods/futures-wheel.md.
2. Premortem w/ owners assigned: ../methods/premortem.md.
3. ≥3 misuse cases from recurring misuse prompts (../methods/misuse-case-brainstorming.md): low mood, compulsion, exclusion, regretted sharing, coercive control by someone close, identification + doxxing; among them one intimate-partner case + one for most vulnerable person feature touches.
4. Block, mute, report + appeal loops specified: ../patterns/safety-and-abuse-resistance.md.
5. Stated default for when user's age unknown (required by launch gate of ../ethics/ethics-review-workflow.md).
6. Staged rollout w/ holdout group + written withdrawal trigger: ../methods/process-safeguards.md.
7. Named owner watching feature after launch.

## Related

- design-a-screen-or-flow.md: steps standard review + full treatment use for new feature.
- review-an-interface.md: steps for existing flow under audit.
- write-a-finding.md: fixed shape of every standard-review answer.
- core-stance.md: ranking ordering findings + severities.
- ../ethics/ethics-review-workflow.md: defines launch gate + post-launch monitoring behind full treatment.
- [Methods index](../methods/index.md): foresight methods + what to run per stage.
- ../checklists/humane-design-audit.md: per-principle yes/no questions for standard review of existing flow.
- ../checklists/usability-review.md: usability-pass counterpart; not sized by tiers.
- answer-an-ethics-question.md: route for product-ethics question.
