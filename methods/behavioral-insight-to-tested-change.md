# Turning a behavioral insight into a tested change

## Use when
- Observed user behaviour → hypothesis → experiment, before any rollout.

## Steps
1. **Frame problem w/ product team, from evidence in hand.** Sources: metric monitoring, usability-study readouts, field observation (e.g. ride-alongs).
2. **Review behavioral-science literature on this exact problem.** Each concept found → concrete UI idea.
   - Waiting problem → concepts = Goal-Gradient Effect, operational transparency, idleness aversion.
3. **Rank UI ideas** by estimated impact + risk.
4. **Test top-ranked ideas in controlled experiment**, analyze results, only then roll out.

## Decision rules
- If problem framed from opinion, not existing evidence → back to step 1 sources.
- If literature search generic → narrow to exact problem, then each concept → concrete UI idea.
- If ranking on impact alone → add risk; ranking uses both.
- If tempted to ship top idea directly → no; controlled test + analysis come before rollout.

## Evidence
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Step-by-step wait screen → 11% fewer cancellations after ride request|Uber Express POOL, controlled experiment|controlled experiment; single product|Literature waiting concepts can become testable screen; measure effect before rollout|

## Output
- Problem statement grounded in existing evidence.
- Literature concepts, each w/ its concrete UI idea.
- Ranking by impact + risk.
- Analyzed experiment result for top ideas = basis for rollout decision.

## Pitfalls
- Framing w/o existing evidence / w/o product team (step 1 skipped).
- Citing concept w/o turning it into concrete UI idea.
- Rolling out before controlled test analyzed.
- Not checking whether lever serves person or exploits them (humane bound, see Related).

## Hypothetical example
- Hypothetical: passport-renewal service sees in support logs + usability readout: applicants abandon while photo check runs. Wait literature → ideas: show each check stage, give estimate + how it's worked out, offer short guide to next step meanwhile. Ranked by impact + risk → top ideas to controlled test before any rollout.

## Related
- [Reading product experiments honestly](reading-experiments-honestly.md): interpreting step 4 test w/o fooling team.
- [Designing peaks and endings](peaks-and-endings.md): applies step 2's three waiting concepts.
- ../laws/goal-gradient-effect.md: law behind one step 2 waiting concept.
- [Applied product cases](../evidence/product-cases.md): step 4 wait-screen case + its evidence.
- activation-moment.md: another correlation → experiment method.
- [Influence versus manipulation](../ethics/influence-vs-manipulation.md): humane bound: does persuasive lever serve person or exploit them?
- counter-metrics.md: pair experiment's metric w/ metric for harm it could hide.
- process-safeguards.md: staged rollout w/ withdrawal condition.
