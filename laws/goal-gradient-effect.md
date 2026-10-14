# Goal-Gradient Effect

## In one line
Nearer goal → stronger motivation to reach it; effort rises as goal nears. Use when designing progress bars, step counters, head starts, reward/loyalty programs, waits; modelling goal acceleration in analytics; checking whether Goal-Gradient (not Zeigarnik Effect) = law to cite + how far its human evidence reaches.
- Alias: goal-gradient hypothesis. Class: effect/principle.
- Theme: Motor + time. Most affects: progress bars + step counters, head starts in loyalty programs + onboarding, step visibility during waits.
- Core rule: show steps remaining; small truthful head start (endowed progress); explain each step during waits.
- Scope warning: design takeaway = progress display, but human evidence = acceleration toward real rewards → verify any progress-display claim w/ step drop-off data.

## Applies when / does not apply when
|Situation|Goal gradient?|Note / cite instead|
|---|---|---|
|visible progress toward real, reachable reward|yes|2006 field evidence covers only real, reachable rewards|
|loyalty schemes + other setups meant to keep people motivated|yes: gradient shapes consumer behavior over time there (consumer research of 2000 + 2003)|—|
|progress display alone, no real reward|not enough|customers w/ no redeemable reward slowed as card filled|
|reward too far away|no acceleration|make first steps feel meaningful|
|huge requirement dressed up as small percentage|will not fully motivate|proportional framing works only within reasonable range; absolute size still matters|
|pre-credited checklist head start|yes: via perceived nearness (endowed progress)|not Zeigarnik Effect|
|checklist started + left|—|Zeigarnik Effect (memory for interrupted tasks)|
|moment right after reward earned|effort drops sharply (postreward resetting)|highest dropout risk|
|every program member|no: ~13% of loyalty members showed no goal gradient (2006 field data)|—|

## Decision rules

### Show progress
- Show people's progress plainly → they finish more readily.
- Expect effort to accelerate near completion.
- Visible progress toward real reward speeds effort; reward drives acceleration, not habit or passage of time.
- During unavoidable waits → explain each step → progress feels steady; treat waits as potential negative experience peaks.
- Head start, even artificial, raises completion → show progress clearly + expose each step → process feels continuous; build head start honestly (next block).
- If choosing percentage framing ('70% complete') vs steps-left framing ('3 steps left') → A/B test; 2006 paper left open whether percentage or steps-left motivates more.

### Grant a head start honestly
- Build head start only from real completed steps (e.g. account created, data imported) or genuine gift toward reward.
- Never inflate total or add nonexistent steps to create head start.
- Count only real completed steps or real gift as progress; keep total effort honest.

### Set rewards + the moment after completion
- Frequent near rewards beat large distant ones (temporal discounting).
- If reward too far away → no acceleration → make first steps feel meaningful.
- Right after reward/completion → show next goal immediately; post-completion moment = churn risk.
- Use per-user acceleration to predict retention.

### Measure it
- Analytics form: goal distance d = (r − n)/r (2006 goal-distance model; r = total requirement, n = amount done).
- Model visit rate, units per session + mid-session exits against goal distance d.
- Three observable forms: rate (shorter gaps between actions), quantity (more units per session), persistence (fewer mid-session exits).
- Per-user acceleration toward first goal = early retention signal: in 2006 study, customers accelerating more toward first reward more likely to earn another + returned sooner.
- Phrase falsifiable predictions as this retention prediction, not as claim about why other users dropped out.
- Measure goal-gradient behavior w/ behavioral logs, not hypothetical surveys.

## Why it works

### Mechanism
- Motivation not constant; rises as remaining distance to goal shrinks.
- Perceived nearness counts → visible/granted progress raises effort.
- Goal-distance model (2006): formalizes goal-gradient hypothesis; effort tracks proportion of original distance still left, d = (r − n)/r, not absolute distance. Rests on relative perception + preference: 1957 psychophysics of ratio judgments + reference points of prospect theory (1979).
- Acceleration toward goal concave: main models of both 2006 reward programs had negative quadratic term → acceleration less steep right near reward.
- Postreward resetting: effort drops sharply right after reward earned + acceleration restarts from zero → moment right after completion carries highest dropout risk.
- Illusionary goal progress, also called endowed progress: head start speeds completion even when required work equal → past progress also motivates, not only remaining distance.
- Near goal, price sensitivity drops + switching costs rise (see Humane bound).

|Related construct|Year|Claim|
|---|---|---|
|control model of self-regulation|1990|feelings come from progress rate compared w/ reference rate|
|goal-looms-larger effect|1998|approach + avoidance motivation both intensify near goal|
|goals as reference points|1999|diminishing sensitivity predicts harder pushing near self-set goal|
|progress as licence|2005|felt progress can free people to act against goal|

### Origin
- 1932: goal-gradient hypothesis proposed within behaviorist psychology.
- 1934: tested on rats: closer to food at end of straight alley (running from start box) → faster they ran; pace kept rising. Speed curve on 20-foot runway looked like compressed 40-foot curve → consistent w/ proportional distance.
- Human evidence came late: until mid-2000s little research on how goal distance shapes people's conduct + decisions, while animal studies abounded (1933, 1948; review in 1977) → before 2006, support almost entirely from animals.
- 2000 + 2003: consumer studies applied gradient to loyalty schemes + similar motivation setups, asking how buyers act there over time.
- 2006: consumer field studies revisited hypothesis + tied it to three outcomes: head start speeds completion even w/ equal work (illusionary progress); shoppers buy faster as reward nears; stronger acceleration goes w/ customers coming back. Overall line: 1932 hypothesis → 1934 rats → consumer research extending it to faster buying + illusionary progress.
- Support for basic claim: 1932 hypothesis, 1934 animal experiment + later consumer research.

## Evidence
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|First clear behavioral field evidence of goal gradient in humans|2006 studies|only for real, reachable rewards|tie progress to real reward|
|Inter-purchase gap shrank 0.7 days from first stamp to last = 20% speed-up; card filled in 24.6 days vs 29.4 days at customers' first-gap pace; first gap averaged 3.3 days vs 2.7-day average gap; latent-class model put 58% of customers in largest segment, which showed significant acceleration|2006 campus café field study: card offering 1 free coffee after 10 purchased; 949 redeemed cards covering ~10,000 purchases|field study analysed w/ hazard models + no-reward control|visible progress toward real reward speeds effort|
|Café study control: participants paid regardless of purchases slowed instead of accelerating. Customers w/ no redeemable reward showed opposite pattern: slowed as card filled|2006 café study control; 2006 field data|no-reward control|acceleration driven by reward, not habit or time|
|Head start: head-start group finished in 12.7 days vs 15.6 days (~20% faster); medians 10 vs 15 days; free stamps did not work as sunk cost|2006 randomized café experiment: 108 customers got 10-stamp card or 12-stamp card w/ 2 stamps pre-filled free; both required 10 purchases|randomized field experiment|head start from real steps or genuine gift|
|Endowed progress effect: 10-stamp card w/ 2 stamps pre-filled redeemed by 34% vs 19% for blank 8-stamp card; head-start group finished faster + showed shorter gaps between washes near goal|2006 car-wash study; every card required 8 paid washes|↑|same|
|Visit frequency, songs rated per visit + persistence all rose as members neared goal; of 473 ended visits, 17% ended right after reward + only 0.2% w/ 50 songs banked toward goal; effort reset after reward: 24 songs on last visit before certificate vs 16 on first visit after; biggest accelerators tended to reach second reward + return sooner|2006 online music-rating program: gift certificate for every 51 songs rated; 148 members, 14,866 ratings|secondary behavioral data|show next goal right after reward; acceleration predicts retention|
|Customers accelerating more toward first reward more likely to earn another + returned sooner|2006 study|retention finding; not claim about why people drop out|per-user acceleration = early retention signal|
|~13% of loyalty members showed no goal gradient|2006 field data|about|do not assume every user accelerates|
|Near goal, people less price-sensitive + more open to promotions: 56% of people close to goal vs 38% of others accepted weekly marketing emails for bonus miles|2006 survey|—|do not exploit near-goal window (Humane bound)|
|Wait design, three levers: goal gradient (every wait step explained), operational transparency (arrival estimate + method behind it), idleness aversion (animation during wait) → post-request cancellations fell 11%|Uber Express POOL, 2019 behavioral science work + A/B experiment|one company's A/B test; single in-house experiment, not general effect size|explain each wait step; waits = potential negative peaks|
|Contrast, Zeigarnik Effect: unfinished tasks remembered better than completed ones|1920s experimental memory study comparing recall of incomplete vs completed tasks|measured recall only; design implications listed for it (signal more content exists, show progress clearly, head start raises motivation to finish) = design takeaways only; head start = endowed progress, i.e. Goal-Gradient|cite Zeigarnik for interrupted tasks, Goal-Gradient for head starts|

## Misreadings and limits
- Wrong: citing Zeigarnik Effect for pre-credited checklist head start → Right: head start works via perceived nearness (endowed progress, Goal-Gradient); Zeigarnik = memory for interrupted tasks + fits checklist started + left.
- Wrong: presenting time-to-value target (e.g. first result within 2 minutes) as established (Parkinson's Law, Goal-Gradient) → Right: no research figure supports universal target; derive from own cohort data + label as hypothesis.
- Wrong: treating goal gradient as animal-only → Right: controlled human field evidence exists (2006: café stamp cards + online rating program), but for real rewards; no-reward control slowed; customers accelerating more likelier to return.
- Wrong: only remaining distance matters → Right: oversimplifies; endowed progress shows past progress also motivates.
- Wrong: restating 2006 link between stronger acceleration + higher chance of continuing to second reward as reason people drop out → Right: retention finding.
- Limit: goal gradient needs real, reachable reward; progress display alone not enough.
- Limit: proportional framing of goal distance works only within reasonable range; absolute size still matters.
- Limit: hypothetical surveys (imagine you had X points) capture beliefs, not motivation over time → use behavioral data instead.
- Limit: illusory progress motivates → raises honesty questions (see Humane bound).

### Overstated evidence to avoid
- Parkinson's Law comes from humorous essay.
- Pareto Principle's 80/20 split = approximate.
- 1982 Doherty Threshold figures = vendor-authored.
- Goal-Gradient Effect rests on animal studies + 2006 human field study of real rewards (customers accelerating more toward first reward more likely to earn another + returned sooner) → never restate it as finding about why people drop out.
- Complexity bias: 1989 study illustrates it well (most participants proposed rules more elaborate than hidden rule = any three ascending numbers), but study's own conclusion concerns reasoning strategies shifting w/ task. Three-number rule-discovery task itself dates from 1960.

## Check questions
- [A] (Doherty Threshold, Goal-Gradient Effect) Every progress bar driven by real work? Look for: bars filled by timer; spinners w/o estimate where estimate possible.
- [A] (Goal-Gradient Effect) Progress visible, + user starts w/ some progress already made? Look for: multi-step flows w/o step count or progress bar.
- [A] (Goal-Gradient Effect, Zeigarnik Effect) Next goal shown right after completion? Look for: dead-end success screens where users drop off.
- Before citing: real, reachable reward? If not → progress display alone not enough.

## Symptoms → fixes
|Symptom|Likely cause (laws)|Fix|
|---|---|---|
|Multi-step flow abandoned midway|Goal-Gradient, Zeigarnik Effect as design takeaways; confirm w/ per-step drop-off rather than assuming cause|step counter or progress bar + small truthful head start|
|People drop off right after reward or success screen|Goal-Gradient Effect: postreward resetting; dead-end success screen|show next goal immediately; watch per-user acceleration as retention signal|
|Unavoidable wait feels stalled|Goal-Gradient Effect: wait steps not explained|explain each step so progress feels steady|

## Hypothetical examples
- Hypothetical (temporal discounting): city recycling scheme credits small voucher after every few drop-offs instead of one prize at year end → near reward pulls effort sooner than distant one.
- Hypothetical (reward program): pharmacy loyalty card fills one slot per prescription pickup toward real discount, + shows slots left.
- Hypothetical (honest head start): tax-return form opens w/ income section marked done, because employer data genuinely imported; no extra steps invented to pad total.
- Hypothetical (progress indicator): passport-renewal flow shows steps remaining atop every screen.
- Hypothetical (explaining each step of a wait): mortgage-approval screen names each stage as it truly happens (documents received, valuation ordered, underwriter reviewing).

## Humane bound
- Turned against people: illusory progress pushing people toward outcomes they did not choose.
- Forms of misused progress: fake progress; inflated totals; reward threshold quietly raised by bonus size; finish lines moved to serve business, not user's goals; targets ratcheting upward so nobody ever finishes.
- Turned against people: using near-goal window to extract consent, raise prices or lock people in. Near goal, price sensitivity drops + switching costs rise → exploitative lock-in possible.
- Pulling finish lines closer exploits users when goal serves business more than users.
- Artificial/illusionary progress motivates but raises honesty concerns.
- Bounded by Intentional.
- Bounded by Finite: against never-closing loops + moved finish lines.
- Bounded by Transparent: progress shown must come from real completed steps or genuine gift.
- Further reading for this bound: habit, progress + gamification mechanics; progress, goals + task completion (entry on granting head start honestly); influence versus manipulation; using psychology responsibly.

## Related
- zeigarnik-effect.md: memory for interrupted tasks (fits checklist started + left), while head start = endowed progress; shares next-goal question + midway-abandonment fix.
- doherty-threshold.md: progress shown during waits; shared question: progress bars driven by real work?
- peak-end-rule.md: waits = potential negative peaks.
- parkinsons-law.md: misapplied together w/ Goal-Gradient to time-to-value targets.
- ../checklists/usability-heuristics-map.md: links Goal-Gradient to heuristic visibility of system status (related laws: Doherty Threshold, Goal-Gradient, Zeigarnik); classic usability heuristics date from 1990, revised 1994.
- ../principles/intentional.md: humane principle bounding Goal-Gradient Effect.
- ../principles/finite.md: humane principle bounding it against never-closing loops + moved finish lines.
- ../principles/transparent.md: humane principle bounding it; progress shown must stay real.
- ../patterns/habits-streaks-and-gamification.md: humane bounds on streaks, counters + rewards + their effect on vulnerable people; applies Goal-Gradient.
- ../ethics/influence-vs-manipulation.md: tests whether head start/progress display serves person or exploits them (illusory progress, lock-in near goal).
- ../ethics/using-psychology-responsibly.md: guardrails for artificial progress + artificial head starts; flags inflated/fake progress as ethically sensitive.
- ../guides/laws-and-principles-crosswalk.md: shows humane principle bounding Goal-Gradient Effect.
- ../patterns/onboarding-and-first-use.md: applies Goal-Gradient.
- ../patterns/feedback-loading-and-performance.md: applies Goal-Gradient.
- ../patterns/progress-goals-and-completion.md: entry on granting head start honestly; applies Goal-Gradient.
- ../patterns/memorable-moments-and-endings.md: applies Goal-Gradient.
