# Second-order thinking

## Use when
- Asking of any feature: what happens at full adoption + cost borne by whom?

## Engine
- One repeated prompt: "and then what happens?"
- Each answer feeds back in as next question → round two, round three, further.
- Contrast, first-order thinking: working feature = end of matter; need met, problem at hand answered, no follow-up question asked.

## The orders
|Order|Question|
|---|---|
|First|What does feature do for person using it?|
|Second|What happens when everyone uses it at once?|
|Third|Cost borne by whom, + what recourse do they have?|

## Steps
1. State feature's first-order effect for person using it (happy path).
2. Ask "and then what happens?" → feed answer back in; repeat to third order + beyond.
3. Model feature at full adoption, not at early-adopter stage where it delights.
4. Ask same questions for indirect users = affected people never opening product yet bearing its effects.
5. Draw happy path + shadow path side by side: customer's journey beside journey of people affected but not using product.
6. Name cost bearer at third order + their recourse.

## Decision rules
- If analysis stops once feature works → first-order thinking; ask again.
- If model assumes a few early adopters → rerun w/ everyone using feature at once.
- If each user's best choice looks good → check for equilibrium where everyone loses; individually optimal choices can converge on one.
- If only direct users appear in journey → add shadow path for indirect users.
- If feature seems too simple to need this → still run it; expect uncomplicated feature to change character at full adoption.

## Output
- Consequence chain to third order + beyond, for direct + indirect users.
- Happy path + shadow path drawn side by side.
- Cost bearer + their recourse.

## Hypothetical examples
- Hypothetical (three orders): app auto-grabbing any freed clinic slot for its users.
  - First order: user seen sooner.
  - Second order: once every patient runs it, freed slots vanish instantly, advantage shrinks toward nothing + users keep checking anxiously.
  - Third order: cost lands on patients w/o app (no smartphone, less digital confidence) = indirect users: can no longer get cancelled slot by phone; they have no channel to object.
- Hypothetical (character change at full adoption): running app's "share my location w/ friends" toggle, launched for solo-run safety, at full adoption becomes map showing when people's homes stand empty.

## Related
- futures-wheel.md: change's consequences mapped in rings, w/ scoring + mitigation.
- premortem.md: imagines failure before launch + works backwards.
- misuse-case-brainstorming.md: how someone could use feature to harm.
- [Four quadrants of design responsibility](four-quadrants-of-responsibility.md): grid: what gets built (pixel, product, ecosystem) vs whom it serves (one person, community, society).
- ../principles/intentional.md: principle served; quick win set against later + second-hand effects.
- [Unintended consequences in cities and societies](../evidence/unintended-consequences.md): second-order effects of products at scale.
- ../ethics/ethics-review-workflow.md: its Forecast step runs neighbouring foresight methods.
- [Responsible use of psychology in design](../ethics/using-psychology-responsibly.md): usability side; guardrails for every psychological lever, incl. whether feature should exist.
