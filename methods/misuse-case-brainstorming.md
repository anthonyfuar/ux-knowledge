# Misuse-case brainstorming

## Use when
- Before feature ships: list ways someone could use it for harm, run it against vulnerable-group prompts, then test misuse cases on real build.

## Steps
1. **Mirror each use case.** Every use case → its misuse case.
2. **Add abuser personas** w/ own goals + requirements, beside ordinary personas.
3. **Run design against vulnerable-group prompts** (table below).
4. **Run forgotten-people list** → research, quantify, set anti-goals, align mitigations.
5. **Test against working build** in dedicated misuse session.
6. **Log each successful attack** w/ finding + mitigation + owner → repeat session once mitigations land.
- Repeat whole exercise for any counter, ladder, rank / badge before shipping it.

## Vulnerable-group prompts
|Area|Ask|
|---|---|
|Depression + suicidal thinking|Could feed, notifications / comparisons worsen low mood? Distressed user after 20 min in this feed: what happens?|
|Addiction|Worst case for susceptible person facing variable rewards, streak anxiety / autoplay chains?|
|Exclusion|Groups shut out by disability, culture, education, language, device, bandwidth / age?|
|Oversharing|Could this provoke sharing people later regret, + what emotional fallout follows?|
|Abusive relationships|Could partner, parent / ex use this to stalk, monitor, blackmail, out / dominate someone?|
|Habit + progress mechanics|Most vulnerable person facing this counter? What does broken run do to them at 11 pm?|
|Health + well-being tracking|Logged number = symptom, not feedback — for whom? What does record reveal about someone's state if another person sees it?|
|Partners, affiliates, embedded kits|What could advertiser, affiliate / third-party kit inside product do that team never would? Would team detect it? What party can contractually + practically stop it?|

## Worked case: a daily streak counter
- Misuse = mechanic uses person, not other way round.
- Centre analysis on person never able to let number break; most vulnerable person facing streak: not casual lapser.

Hypothetical personas; savings app, use case = building saving habit by daily check-ins:
- Hypothetical: perfectionist-trait person (cannot let number break) makes token transfer late every night, even on days money needed for food, only to keep run alive.
- Hypothetical: person on irregular income (cannot save in lean week) reads each reset as verdict on their worth + stops opening app.
- Hypothetical: person recovering from gambling, for whom daily money tally w/ "keep it going" framing feels like chase they're trying to quit.
- Hypothetical: person keeping weekly screen-free day of rest for religious reasons, forced each week to choose between this practice + run.
- Hypothetical: adult child w/ access to elderly parent's account watches parent's check-ins + uses broken run to pressure them over spending.

Mitigations:
|Do|Avoid|
|---|---|
|Count unit other than consecutive days|consecutive-day runs as only measure|
|Keep number private + optional|public / mandatory counters|
|Let declared absence keep run intact|resetting runs for declared absence|
|Send no loss-framed reminders|"you'll lose your streak" prompts|
|Read heaviest-use segment as warning sign|celebrating heaviest users as success|

## Forgotten-people list
Groups: LGBTQ people; disabled + elderly people; people in other countries / fragile political contexts; parents; poor people; religious people; people w/ eating disorders / illness.
1. For each group ask: worst this could do to them?
2. Research how those scenarios feel to people in them.
3. Quantify how often scenarios already occur.
4. Convert into explicit anti-goals.
5. Align mitigations w/ product goals.

## Testing misuse against a real build
- Limit: written misuse case = hypothesis until somebody tries it.
- Limit: automated scanning finds broken code, not cruelty; only humans imagining harm find consequential routes to harm.

|Do|Detail|
|---|---|
|Run dedicated session before release|testers get working build; task = locate, contact, expose, impersonate, wear down / trap another participant, using only features set to ship|
|Include survivors of harassment / stalking|pay them; tell them beforehand what they'll attempt; let them stop any time|
|Add harm question to ordinary user research|w/ consent, ask participants what harm they already met through everyday tools → their accounts describe attacks nobody on team pictured|
|Log every successful attack|finding + mitigation + owner|
|Repeat session|once mitigations landed|

## Output
- Misuse case per use case; abuser personas beside ordinary ones.
- Answers to every vulnerable-group prompt.
- Anti-goals from forgotten-people list, w/ frequency + aligned mitigations.
- Attack log from build test: finding, mitigation, owner; retest result.

## Pitfalls
|Symptom|Likely cause|Fix|
|---|---|---|
|Analysis pictures casual lapser|wrong person at centre|centre on person never able to let number break|
|Misuse list never tested|treated as finished on paper|run build session|
|Only scanners run|belief tooling finds harm|humans imagining harm + lived-experience testers|
|Counter, ladder, rank / badge shipped unexamined|exercise run once for one feature|repeat per mechanic before ship|
|Mitigations land, no retest|session not repeated|rerun after mitigations|

## Related
- ../patterns/safety-and-abuse-resistance.md: patterns: misuse cases + abuser personas, blocking + reporting, vulnerable people + children.
- [Habit, progress and gamification mechanics](../patterns/habits-streaks-and-gamification.md): streaks, counters, rewards + their effect on vulnerable people = streak case's surface.
- [Progress, goals and task completion](../patterns/progress-goals-and-completion.md): usability side of progress mechanics: indicators, head starts, multi-step completion.
- ../principles/resilient.md: principle behind method; abuse taken as given, most vulnerable put first.
- [Safety and abuse evidence](../evidence/safety-and-abuse.md): harassment, stalking + intimate-partner abuse carried out via products.
- premortem.md: neighbouring foresight method; imagine failure before launch, work backwards.
- counter-metrics.md: numbers flagging harm after launch, incl. reading heaviest-use segment.
- ../ethics/ethics-review-workflow.md: misuse cases + abuser personas sit in its review before build.
