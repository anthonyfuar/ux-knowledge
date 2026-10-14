# Influence versus manipulation

## Contents
- Use when
- Why the line matters
- Process
- Line-drawing test
- Lever by lever
- Better success signals
- Further levers
- Check questions
- Hypothetical examples
- Related

Tests whether persuasive lever serves person or exploits them: process, line-drawing test, lever-by-lever table, success signals + further levers.

## Use when
- Design leans on psychological law to raise engagement/conversion.
- Judging whether lever crosses line.

## Why the line matters
- Compulsive products can arise when knowledge behind intuitive products turns to preying on minds.
- Documented harms of attention-capturing products: weakened relationships, anxiety, lost sleep.
- Once product begins shifting people's self-image + ways of relating to others → harms count as serious.

## Process
1. Admit possibility of exploiting minds.
2. Ask whether to build feature at all. If its goals conflict w/ users' goals → do not build.
3. Talk w/ users; qualitative findings steer design, not usage metrics alone: action log records what people did, silent on product's effects on their lives + on their motives.

## Line-drawing test
- Influence = serves goal user already holds.
- Manipulation = serves goal user would reject if they saw it.

## Lever by lever
|Lever|Legitimate use|Crosses line when|Note|
|---|---|---|---|
|../laws/doherty-threshold.md|Fast response keeps people productive + focused|Speed tuned for compulsion|Apps responding in under 400 ms once described as 'addicting' → speed-driven engagement deserves scrutiny|
|Artificial delay|Signal real effort; build warranted trust|Inflates perceived value of trivial work|—|
|Progress bars|Make waits bearable|Deliberately misrepresent progress|Help even when inaccurate → keeping them honest = designer's choice|
|Head start (../laws/goal-gradient-effect.md / ../laws/zeigarnik-effect.md)|Motivate completing tasks people want done|Illusory progress pushes people toward outcomes they did not choose|—|
|Open loops (../laws/zeigarnik-effect.md)|Remind people of tasks they started, w/ way to finish/dismiss|Cliffhangers, autoplay + ellipsis teasers drive compulsive return|—|
|Emphasis (../laws/von-restorff-effect.md)|Highlight what matters to user; help users spot option fitting their goal|Salience pushes business's preferred option over user's, especially in quick decisions w/ weak preference|2012 study: visual salience outweighed preference when choices made at fast speeds|
|../laws/flow.md + gamification|Absorption in user's own goal, w/ natural stopping points|Mechanics turn play into unpaid work or trap users in hyperfocus|2021 work claims flow mechanics can turn play into unpaid work + trap users in hyperfocus|
|Emotional arousal|Reassure people at high-stakes moments|Fear-based urgency/ominous warnings exploit threat detection|Anxious users amplify ambiguous signals into worst-case readings|
|../laws/aesthetic-usability-effect.md|Earn goodwill|Polish hides problems users pay for later|—|
|../laws/peak-end-rule.md|Make real value memorable|Endings manufactured to cover bad experience|—|
|[Cognitive biases](../laws/cognitive-bias.md)|Design around them to protect users|Exploited for conversion|—|

## Better success signals
- Measure meaningful value delivered, not time spent.
- Aim: virtual rewards never stand in for real experience; tech should enrich experience.
- Incentive analysis: predict feature's effects by asking what business model pays it to optimize.
- If feature's target = raw time/raw taps → expect attention harvesting: red badges, infinite scroll, intermittent reinforcement.
- Surrogation: engagement + conversion metrics = proxies; teams drift into treating proxy as goal.

Cases:
- Facebook prioritized posts from friends + family even at some cost in time on site, as success measure shifted from time on site to meaningful interactions.
- Even redefined 'meaningful interactions' measure of 2018 feed-ranking change computed from predicted comments, shares + reactions → could reward provocation.
- Same 2018 feed-ranking announcement paired change w/ continued demotion of 'engagement bait' + pointed to existing user control for pinning favorite pages atop feed.
- Google shipped well-being features in Family Link + its Digital Wellbeing tools, incl. parental rules, finer notification control, usage dashboards.

## Further levers
|Lever|What happens|Rule|
|---|---|---|
|Illusion of control|When outcomes random/uncontrollable, people invent rituals. Supported by yoked-noise study + pigeon experiments (random outcomes → invented rituals)|In variable-outcome systems → make causality visible. Unexplained randomness → superstition; randomness as variable reward → compulsive use|
|Unit bias|Default episode lengths + autoplay chunks set norm for how much people consume|Ethical if producing real value; manipulative if purely for lock-in|
|Denomination effects|Credits + in-app currencies loosen spending|Ethical if producing real value; manipulative if purely for lock-in|
|IKEA effect|People overvalue what they partly built themselves; shown in 2011 study|Ethical if producing real value; manipulative if purely for lock-in|

## Check questions
- Lever serves goal user already holds, or one they would reject if they saw it?
- Feature's goals conflict w/ users' goals? If yes → do not build.
- What did talking to users show, beyond usage metrics?
- What does business model pay this feature to optimize?
- Team treating proxy metric as goal?
- In variable-outcome system, causality visible?

## Hypothetical examples
- Hypothetical: language-learning app pre-fills progress on course learner enrolled in → serves learner's goal (influence); same pre-filled progress on auto-renewing premium upsell learner never asked for → crosses line.
- Hypothetical: home-security app uses red alarm styling + countdown for routine firmware update → fear-based urgency exploiting threat detection (crosses line); reassurance kept for high-stakes moments, e.g. real break-in alert (legitimate).
- Hypothetical: transit card prepaid credits riders spend on real trips → real value (ethical); same credits set to expire unless topped up, purely to lock riders in → manipulative.

## Related
- [Responsible use of psychology](using-psychology-responsibly.md): guardrails for every psychological lever + well-being examples.
- deceptive-patterns.md: humane-design side; named deceptive patterns + humane alternative each.
- attention-hijacks.md: humane-design side; ten attention levers + counter each.
- [Persuasion asymmetries](persuasion-advantages-of-systems.md): six advantages system holds over human persuader + counterweight each.
- ../guides/laws-and-principles-crosswalk.md: humane principle bounding each law.
- ../methods/engagement-vs-empowerment-metrics.md: tell capture metrics from benefit metrics.
- ../patterns/habits-streaks-and-gamification.md: streaks, counters, rewards + effect on vulnerable people.
- ethics-review-workflow.md: steps for feature ethics review before launch.
