# Ethics review workflow

## Contents
- Use when
- Three checkpoints in the design loop
- The seven steps
- How the ethics role works
- Weighing objections
- Watch-list phrases
- Related

Feature ethics review in seven steps, kickoff → post-launch, each w/ timing, people + artifact. Also: how ethics role should work, weighing objections, phrases to watch for in discussion.

## Use when
- Planning/running pre-launch ethics review of feature.
- Setting up team review routine.
- Review depth (quick pass / standard review / full treatment) → ../guides/how-deep-to-go.md.

## Three checkpoints in the design loop
Add three ethics checkpoints to design loop:

|Checkpoint|Question it asks|
|---|---|
|Evaluate|Problem worth solving?|
|Forecast|How could someone exploit each idea?|
|Monitor|Product doing what in world?|

Baseline criteria for judging design 'good' = autonomy + transparency + safety.

## The seven steps
1. **Frame**
   - When: kickoff. Who: product lead, designer, researcher.
   - Produces: problem statement; harm-and-incentive map = physical, emotional + societal harms crossed w/ incentives of engagement, careless experimentation, scale, neutrality + speed (../principles/cross-cutting-practices.md); stated design principles.
2. **Evaluate**
   - When: before ideation. Who: whole team + one person freed from bottom-line incentives = designated ethics owner.
   - Produces: 'Should we?' record via ../methods/three-gate-check.md method; explicit anti-goals; identified indirect stakeholders.
3. **Forecast**
   - When: before build. Who: team, cross-functional partners, domain experts, people w/ lived experience.
   - Produces: ../methods/futures-wheel.md; ../methods/premortem.md risk register w/ owner per risk; [misuse cases](../methods/misuse-case-brainstorming.md) + abuser personas; walk through ../methods/four-quadrants-of-responsibility.md.
4. **Design gate**
   - When: design review. Who: reviewers using ../checklists/humane-design-audit.md checklist.
   - Produces: review vs [seven humane-design principles](../principles/index.md), one row per principle; any deceptive-patterns.md found named, each w/ honest alternative.
   - Requires: every [default](../patterns/defaults-and-choice-architecture.md) justified.
5. **Launch gate**
   - When: pre-release. Who: product, legal, PR, trust and safety.
   - Requires: threat model incl. intimate-partner threats; safety features ship day one; block, report + appeal specified (../patterns/safety-and-abuse-resistance.md); fragile-context readiness = moderation in local languages, local presence, emergency contact; age-assurance decision incl. default when user's age unknown (../principles/inclusive.md).
   - Can block release on third-party harm alone.
6. **Monitor**
   - When: post-launch + recurring. Who: named owner, support, analytics, affected communities.
   - Uses: ../methods/counter-metrics.md dashboard, each number w/ trip threshold + action when tripped; staged rollout w/ holdout group (../methods/process-safeguards.md); segmented after-testing; standing review w/ affected communities.
   - Requires: written withdrawal trigger + person empowered to pull feature.
7. **Reflect**
   - When: quarterly. Who: each practitioner.
   - Includes: personal ethical-drift check (../methods/team-and-personal-practices.md); team retrospective on workload + attention.

## How the ethics role works
|Do|Avoid|Why|
|---|---|---|
|Facilitate|Judge|Role = facilitation, not judgment|
|Put ethical question in front of real decision-makers|Owner becomes person saying no|Owner turns into outsourced conscience: team hands conscience over + stops carrying it|
|Make honest answers safe|Practice hardening into stick|Review people expect to be judged by = review they route around|
|Aim at movement toward least harm for those affected|Aim at certificate declaring team ethical|Least harm for those affected = review's aim|

## Weighing objections
- Powerful technologies attract both fear of novelty + well-founded objections. Most turn out good + bad at once, depending on deployment + governance.
- Separate fear of novelty from well-founded objection.
- Do not settle objection by classifying person raising it.
- Ask what concern predicts:
  1. Who gets harmed?
  2. Via what mechanism?
  3. How would harm show up observably?
  4. What would change our minds?
- If concern names mechanism + observable signal → earns mitigation, whether or not raiser likes technology category.
- If concern only registers discomfort → write it down + watch for signal it implies.
- Hypothetical: smart-lock remote-unlock review; engineer disliking connected locks warns former partner still holding household app login could open door, visible as unlock events after household change → mechanism + signal named → mitigation earned, regardless of engineer's view of connected locks.

## Watch-list phrases
When any of these said → pause ethics discussion:
- 'just an edge case'
- 'most of our users'
- 'only a test'
- 'it's in the terms'
- 'everyone else does it'
- 'we'll fix it after launch'
- 'nobody is forcing them to use it'

Name 'nobody is forcing them to use it' separately: sounds like freedom, works as change of subject → moves fault onto person though team built mechanics. Product engineered to make putting it down hard cannot treat putting it down as test of user's character.

## Related
- ../guides/answer-an-ethics-question.md: reasoning steps when asked if product decision acceptable.
- ../guides/how-deep-to-go.md: choose quick pass, standard review / full treatment.
- ../checklists/humane-design-audit.md: yes/no questions per humane principle + AI + automation; design-gate checklist.
- ../checklists/usability-review.md: usability side of design review; yes/no questions by theme, each tied to law.
- [Methods overview](../methods/index.md): method to use at each stage.
- ../methods/stakeholder-arguments.md: argument structures justifying usability + humane choices to stakeholders.
- ../patterns/safety-and-abuse-resistance.md: misuse cases, blocking + reporting, vulnerable people, children.
- [Responsible use of psychology](using-psychology-responsibly.md): guardrails for every psychological lever.
