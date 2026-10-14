# Premortem

## Use when
- Before launching plan/feature: imagine it already failed → reason back to causes.
- Kickoff = blind spot of look-back reviews (postmortem, retrospective): at kickoff they surface no project threats + none of its downstream effects.

## Why it works
- Prospective hindsight = imagining outcome already occurred, then looking back. Improves identifying outcome's causes by about 30%.
- Disarms overconfidence suppressing concerns about plan.
- Premortem = postmortem run in reverse, on failure still only supposed.
- Postmortem, by contrast: lessons for next collaboration + process round, from what slowed/sank finished work.

## Steps (7)
1. **Brief**: share plan w/ participants. If executive sponsors' presence would chill honesty → leave them out.
2. **Frame**: tell group: one year from now, feature failed or made news for wrong reasons. Ask what happened.
3. **Silent brainstorm**: each person alone writes concrete failure reasons, 5–10 min.
   - Each reason names scenario + actor + mechanism. Reject vague reasons lacking them.
   - Hypothetical: accept → caller posing as bank support talks older customer into reading out one-time code, then adds new payee from customer's account.
   - Hypothetical: reject → "adoption could be low."
4. **Round-robin**: one reason per person per turn until all exhausted. Record all in one visible place.
5. **Prioritize**: place reasons on likelihood × severity matrix; keep about 10.
6. **Assign**: each kept risk gets owner + candidate mitigation.
7. **Fold back**: update roadmap + risk register. Then revisit risks at milestones.

## Timing + tone
|Format|Length|Fits|
|---|---|---|
|Full premortem|30–60 min|Before launch of plan/feature|
|Short version|15-min|Sprint kickoff|

- Tone: practical, not venting.

## Output
- Visible list of all reasons; ~10 prioritized risks on likelihood × severity; owner + candidate mitigation per risk; updated roadmap + risk register; milestone check-ins.

## Pitfalls
- Sponsors in room chilling honesty → leave them out of briefing.
- Vague reasons → require scenario, actor, mechanism.
- Session turns into venting → keep it practical.
- Risks listed but plan unchanged → fold back into roadmap + risk register.

## Related
- second-order-thinking.md: what happens at full adoption + who bears cost.
- futures-wheel.md: mapping change consequences in rings.
- misuse-case-brainstorming.md: listing how someone could use feature to harm.
- debiasing.md: usability side; pre-mortem among debiasing tools for reviews + team judgment.
- ../laws/cognitive-bias.md: usability-side law: systematic judgment departures from rational choice.
- ../principles/intentional.md: principle this method serves; quick win vs later + second-hand effects.
- ../ethics/ethics-review-workflow.md: its Forecast step keeps premortem risk register w/ owners.
- ../patterns/safety-and-abuse-resistance.md: misuse cases, blocking + reporting, vulnerable people.
