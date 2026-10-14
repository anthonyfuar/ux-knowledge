# Three-gate check (possible → permitted → right)

## Use when
- Build/release decision.
- Forced-choice question (which group fails, which harm, whose interest loses) → still applies; trace upstream (see Forced choices).
- Scope: three gates in fixed order, legality rule, tracing dilemma to causing decision, narrowing personal-data release, worked hypothetical.

## Steps: three gates, one after another
Fixed order: 1 Able → 2 Allowed → 3 Should.

|Gate|Question|What to know|
|---|---|---|
|1 Able|Technically possible?|Takes most engineering time.|
|2 Allowed|Legal + within policy + aligned w/ strategy?|Legal review stops here; does not cover gate 3.|
|3 Should|Ought we to do it at all?|Name decision's competing motives (e.g. innovation, profit, social contribution). Weigh long-term consequences.|

## Legality = floor, not ceiling
- Legal does not settle whether to do it.
- Why: regulation follows harm; bans one manipulative trick while sibling tricks survive.
- If rules permit it → still hold stricter internal standards.

## Forced choices
- Symptom: ethical question posed as forced choice: which group system fails / which of two harms / whose interest loses.
- Read as: clue to situation's setup, not real ethical question.
- Step: find earlier decision leaving only these options. Typical:
  - capability team should never have built
  - default team could have withheld
  - step removed to save one second
  - fail-safe nobody funded
- Upstream decision usually still open → finding goes there, not at forced choice.
- Avoid: answering only forced choice as posed → ratifies setup behind it.

## Narrowing a release of personal data
Defensible answer = narrow every release dimension until benefit survives + exposure does not.
1. Aggregate → no one can pick out individuals.
2. Limit to one defined area + one defined time window.
3. Release only to named organizations under written purpose limit.
4. Delete when defined use ends.
5. Publicly state data shared.

## Hypothetical example
Hypothetical: school district asks education-app vendor for students' at-home usage logs (times, devices, places) to find those w/o home internet.
- Able: passes; logs exist.
- Allowed: passes; contract + law can read as permitting it.
- Should: same logs could find unconnected students; they also reveal household routines, who shares devices, when child home alone.
- Narrowed: per-neighbourhood counts only, one area + one term, district office named in written purpose limit, deletion when outreach ends, public note of data shared.

## Output
- Write down reasoning while time allows: next such request will leave no time.
- Should-we record sits in ethics-review workflow, before ideation.

## Pitfalls
- Treating gate 2 pass as final → legal review does not cover gate 3.
- Debating two offered harms → upstream decision unexamined.
- Full-dataset release since benefit real → narrow every dimension first.

## Related
- [Four quadrants of design responsibility](four-quadrants-of-responsibility.md): companion; crosses what gets built w/ whom it serves.
- ../ethics/ethics-review-workflow.md: where Should-we record sits, before ideation.
- ../guides/answer-an-ethics-question.md: steps for judging if product decision acceptable.
- ../principles/intentional.md: principle gating decisions w/ these gates.
- ../patterns/privacy-data-and-security.md: data minimisation, consent, access + deletion; worked example's surface.
- ../ethics/influence-vs-manipulation.md: usability-side counterpart; tests if persuasive lever serves or exploits person.
- process-safeguards.md: changing floor when competition drives harm; staged rollout w/ withdrawal condition.
- second-order-thinking.md: long view: full-adoption effects + who bears cost.
