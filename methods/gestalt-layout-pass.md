# Grouping-first layout pass (Gestalt pass)

## Use when
- Laying out screen / re-checking design already looking finished.
- Goal: settle grouping cues before styling; 7 steps.

## Steps
1. **Whole before parts.** Overall configuration first; whole layout sets each element's role.
2. **List units.** Mark elements needing to read as one unit vs as separate.
3. **One cheapest cue per unit.** Cheapest working grouping cue. Order, cheapest → most expensive: spacing → likeness → shared region → connector.
4. **Make all cues agree.** All favour same partition; remove any cue arguing for another.
5. **Re-run pass late.** Aesthetic tweaks quietly erode grouping in finished-looking designs.
6. **Test hierarchy w/o content.** Grey-box / blur text, or gray-box wireframe beside live page → structure should still read. Why: layout conveys structure before any word gets read.
7. **Validate critical groupings w/ users.** No grouping law guarantees how people read layout.

## Cue choice
|Need|Cue (cost order)|Law|
|---|---|---|
|Group by nearness|spacing (cheapest)|Law of Proximity|
|Group by shared look|likeness|Law of Similarity|
|Group inside boundary|shared region|Law of Common Region|
|Group by explicit link|connector (most expensive)|Law of Uniform Connectedness|

## Decision rules
- If spacing alone makes unit read → stop; region / connector not needed.
- If two cues suggest different groupings → keep one matching intended partition, remove other.
- If design looks finished after visual polish → re-run grouping pass.
- If blurred / grey-boxed version shows no clear structure → layout not conveying hierarchy → rework it.
- If grouping critical → validate w/ users; no grouping law guarantees how people read it.

## Pitfalls
|Symptom|Likely cause|Fix|
|---|---|---|
|Elements read as wrong group|competing cues|step 4: one partition, remove dissenting cue|
|Heavy boxes + lines all over|expensive cue where spacing would do|step 3: cheapest working cue|
|Grouping fine in wireframe, muddled in final|late aesthetic tweaks|step 5 re-run|
|Structure visible only when reading text|layout not conveying hierarchy|step 6 content-free test|

## Hypothetical example
- Hypothetical: bank transfer screen must read as two units: payee details + amount/date. Extra space between units carries split; inside each, matching field styles hold it; no card borders needed. Later change gives amount field coloured fill shared w/ payee name → likeness now argues for different partition → fill removed.

## Related
- [Gestalt grouping principles](../laws/gestalt-principles-overview.md): how grouping cues combine + compete (steps 3 + 4).
- ../laws/proximity.md: step 3 spacing cue.
- ../laws/similarity.md: step 3 likeness cue.
- ../laws/common-region.md: step 3 shared-region cue.
- ../laws/uniform-connectedness.md: step 3 connector cue.
- [Content layout, grouping and visual hierarchy](../patterns/layout-grouping-and-hierarchy.md): pattern entries: grouping cues, spacing, containers, emphasis + reading order.
- [Responsible use of psychology in design](../ethics/using-psychology-responsibly.md): guardrails for every psychological lever, incl. grouping + emphasis.
