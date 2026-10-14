# Usability heuristics mapped to UX laws

## Use when
- Finding needs its usability heuristic named beside law.
- No law explains problem → heuristic carries finding alone.

## Citing rules
- Usability finding cites both heuristic + law.
- Heuristic names what went wrong; law explains why people behave as observed.
- Many error-prevention fixes need no law (idempotent submit, undo, soft delete, constraints) → cite error-prevention heuristic alone.
- Avoid: borrowing timing / motor law to justify error-prevention fix no law explains.

## Fit test (run before citing a law)
1. State mechanism behind problem in one sentence.
2. Check law's definition predicts stated mechanism.
3. Definition does not predict it → cite heuristic only (see law misapplications guide).

|Law|Fits only when / about|
|---|---|
|../laws/hicks-law.md|problem involves choice among options|
|../laws/doherty-threshold.md|system response time|
|../laws/peak-end-rule.md|emotional peak / real end of episode exists|
|../laws/fittss-law.md|predicts movement time|

Hypothetical: utility-bill portal charges twice when Pay double-tapped. Step 1: nothing stops repeated submit. Step 2: Fitts's Law predicts movement time, not repeated submits → no fit. Step 3: cite error prevention alone; fix = idempotent submit.

## Map: ten heuristics → related laws
Ten classic usability heuristics, first published 1990, revised 1994; in their order.

|#|Heuristic|Related laws (link through)|
|---|---|---|
|1|Visibility of system status|../laws/doherty-threshold.md, ../laws/goal-gradient-effect.md, ../laws/zeigarnik-effect.md|
|2|Match between system + real world|../laws/mental-model.md, ../laws/jakobs-law.md|
|3|User control + freedom|../laws/jakobs-law.md (opt-in redesigns + way back to old version); ../laws/paradox-of-the-active-user.md (safe experimentation)|
|4|Consistency + standards|../laws/jakobs-law.md, ../laws/similarity.md|
|5|Error prevention|../laws/postels-law.md; ../laws/fittss-law.md (destructive-target spacing); ../laws/working-memory.md; many fixes = heuristic alone|
|6|Recognition rather than recall|../laws/working-memory.md, ../laws/millers-law.md, ../laws/chunking.md|
|7|Flexibility + efficiency of use|../laws/pareto-principle.md, ../laws/teslers-law.md, ../laws/parkinsons-law.md|
|8|Aesthetic + minimalist design|../laws/aesthetic-usability-effect.md, ../laws/occams-razor.md, ../laws/cognitive-load.md, ../laws/hicks-law.md|
|9|Help users recognize, diagnose + recover from errors|../laws/peak-end-rule.md, ../laws/working-memory.md|
|10|Help + documentation|../laws/paradox-of-the-active-user.md|

## Related
- [Usability review checklist](usability-review.md): yes/no questions by theme, each tied to UX law; rows w/ no fitting law cite heuristic from this map.
- ../guides/write-a-finding.md: finding's fixed shape, confidence labels + severity ranking; where heuristic + law get cited.
- ../guides/law-misapplications.md: wrong uses of each law + correction; read when fit test fails.
- ../guides/symptom-to-fix-index.md: observed usability problem → law explaining it → fix.
- ../laws/index.md: all 30 UX laws by theme w/ core idea + design rule; check law's definition here.
- ../patterns/errors-and-input-tolerance.md: error prevention + recovery, tolerant input, destructive actions.
- ../patterns/friction-undo-and-confirmation.md: humane-design side of error prevention; confirmation graded by consequence, undo windows.
- humane-design-audit.md: humane-design companion; yes/no questions per humane principle + AI and automation.
