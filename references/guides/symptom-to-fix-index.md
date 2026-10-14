# Symptom-to-fix index

## Use when
- Usability symptom known but not law explaining it or remedy.
- Rows list candidate laws; finding still cites one primary law (two at most) = one whose mechanism matches problem.
- Before citing candidate law → check it not stretched (law-misapplications.md).
- Heuristics among candidates (error prevention, error recovery, visibility of system status, user control) → described in ../checklists/usability-heuristics-map.md.
- Row → finding: fixed shape, confidence labels + severity in write-a-finding.md.
- Symptom groups: choosing, comparing + deciding · seeing, finding + scanning · memory, forms + input · errors, failures + recovery · touch, speed + waiting · flows, onboarding, change + endings · testing, real content + team judgment.

## Choosing, comparing + deciding
|Symptom|Candidate laws|Fix|
|---|---|---|
|Users stall on crowded entry screen|Hick's Law, Choice Overload|one focused entry action; filters + secondary options after it|
|Pricing / plan choice paralyzes users|Choice Overload, Hick's Law|tiers side by side, one recommended|
|Pricing / plan page steers users to tier they do not need|Choice Overload (decoy), Cognitive Bias (anchoring)|compare tiers to user's stated criteria; drop dominated tiers; show honest first reference price|
|Users stay stuck w/ defaults / trapped in subscriptions|Cognitive Bias (status quo, loss aversion)|default = informed user's pick; cancelling as easy as signing up; no guilt copy|
|Checkout quietly adds cost / consent|Cognitive Bias (defaults, status quo)|add-ons + save-card unchecked by default; all fees visible before review step; apply ../ethics/influence-vs-manipulation.md test|
|Grid of look-alike cards hard to compare|Cognitive Load, Working Memory (comparing across cards); not Similarity (uniform cards correctly read as one content type), not Selective Attention|deciding attributes (price, rating, key spec) shown consistently; add sorting + filters|

Law files: ../laws/hicks-law.md, ../laws/choice-overload.md, ../laws/cognitive-bias.md, ../laws/cognitive-load.md, ../laws/working-memory.md, ../laws/similarity.md, ../laws/selective-attention.md.

## Seeing, finding + scanning
|Symptom|Candidate laws|Fix|
|---|---|---|
|Links / buttons missed|Similarity, Von Restorff Effect|interactive elements look unlike text; one standout primary action|
|Labels seem to belong to wrong field|Proximity|each label nearer own field than neighbours; larger gaps between groups|
|Layout = undifferentiated clutter|Chunking, Common Region, Prägnanz|evident hierarchy, dividers, modules w/ backgrounds / borders|
|Charts misread / data series confused|Similarity, Von Restorff Effect|one colour per metric across all charts; colour-blind-safe categorical palette; direct labels, not legends; one accent colour for key series|
|Icons confuse users|Cognitive Load|label each icon in words unless nearly everyone reads it alike: close, print + play/pause may stand alone; share + reply sometimes counted universal, but meaning varies by product → label them too|
|Important update, prominent element / new control goes unseen|Selective Attention (tunnel vision, change blindness)|strong cue in reading path / beside control in use; one change at a time|
|Promotions, emphasized items / real content skipped as ads|Selective Attention (banner blindness), Von Restorff Effect|styling consistent w/ surroundings; no ad styling + no ad slots; test on mobile|
|Key control below fold / off screen never found (e.g. Save at end of long page)|Selective Attention (tunnel vision) + visibility-of-system-status heuristic; not Fitts's Law (assumes visible target)|sticky save bar appearing once something changes, or auto-save w/ visible saved state; warn when leaving w/ unsaved changes|
|Long filter / facet list slow to use|Cognitive Load; not Choice Overload (multi-select facets not one pick among alternatives)|type-ahead inside facet; grouped facets; recent / popular values pinned at top|
|Settings page w/ dozens of toggles hard to scan|Cognitive Load, Chunking, Common Region, Tesler's Law (progressive disclosure), Pareto Principle (verify actual usage w/ analytics); not Choice Overload|task-based labelled groups; search over setting names, synonyms + descriptions; advanced settings behind disclosure|

- Facet ordering: alphabetical facet values help only users knowing exact label; ordered list's search benefit (1985 study) applies only to users knowing exact label they seek.

Law files: ../laws/similarity.md, ../laws/von-restorff-effect.md, ../laws/proximity.md, ../laws/chunking.md, ../laws/common-region.md, [Prägnanz](../laws/pragnanz.md), ../laws/cognitive-load.md, ../laws/selective-attention.md, ../laws/fittss-law.md, ../laws/choice-overload.md, ../laws/teslers-law.md, ../laws/pareto-principle.md.

## Memory, forms + input
|Symptom|Candidate laws|Fix|
|---|---|---|
|Users forget query / selections on next screen|Working Memory|keep inputs visible; comparison tables; visited states + breadcrumbs|
|Filters, query / scroll position lost on Back|Working Memory, Tesler's Law (system carries state); also user-control heuristic|keep state in URL; restore scroll position + filters on return|
|Codes / IDs copied from elsewhere get mistyped|Chunking, Working Memory|show in delimited groups of 3–5; accept paste; keep code visible where entered|
|Forms take too long|Tesler's Law (system carries stored data), Parkinson's Law (expected-duration lens)|autofill; reuse data already held; sensible editable defaults|
|Strict input format rejects valid entries|Postel's Law|within bounds + w/ explanation, accept varied formats + normalize them|
|Field errors fire while user types, or valid fields get noisy checkmarks|Selective Attention (interruption), Cognitive Load; also error-prevention heuristic|validate when user leaves field / submits; once error shown, recheck field live → error clears as soon as fixed; valid fields stay quiet; focus first error / linked error summary|

Law files: ../laws/working-memory.md, ../laws/teslers-law.md, ../laws/chunking.md, ../laws/parkinsons-law.md, ../laws/postels-law.md, ../laws/selective-attention.md, ../laws/cognitive-load.md.

## Errors, failures + recovery
|Symptom|Candidate laws|Fix|
|---|---|---|
|Errors / payment failures spiral into abandonment|Working Memory, Cognitive Load|keep problem, user's input + next step visible together. Why: stress cuts working capacity → recovery flows need most simplification|
|Card declined / payment times out|Working Memory, Peak-End Rule (negative peak); also error-recovery heuristic|declined card → keep all fields filled + clear only security code; give reason in plain words; offer another payment method. Timeout → check order status before allowing retry|
|Double charges / duplicate submissions|error-prevention heuristic, not law|idempotent submit w/ request key; pending state on button; safe retry never double-charging|
|Users regret destructive action|error-prevention heuristic, Fitts's Law (separation)|undo / soft delete first; confirm only irreversible, rare actions + name consequence; keep dangerous controls apart from others|
|Automated feature fails + users lost|Tesler's Law|communicate system state; failure + handover path w/ diagnosis + support|

Law files: ../laws/working-memory.md, ../laws/cognitive-load.md, ../laws/peak-end-rule.md, ../laws/fittss-law.md, ../laws/teslers-law.md.

## Touch, speed + waiting
|Symptom|Candidate laws|Fix|
|---|---|---|
|Users mis-tap on mobile|Fitts's Law|target size floors 44 pt / 48 dp / 24 px (standards); spacing between targets; centre-first placement over thumb-zone maps; separate destructive neighbours (error prevention)|
|Mouse-era layout ported to touch|Fitts's Law|centre-first placement; size targets by position, in mm; no edge / corner shortcuts on touch|
|App feels sluggish|Doherty Threshold|acknowledge input within 400 ms; animation / progress bar for longer work|
|Long operation holds users hostage|↑|put waits after completion points; past ~15 s move work to background + notify; drive progress bars from real work|
|Content jumps while loading + causes mis-clicks|Doherty Threshold, Fitts's Law|reserve space for late content; never move target under pointer; include layout stability in performance budget|
|Refreshing data blanks screen / gives no sign of what changed|Doherty Threshold, visibility-of-system-status heuristic (what changed + when), Working Memory|skeleton on first load only; on later refreshes keep stale data visible w/ inline cue + 'last updated' time|
|Payment / other processing makes users wait at checkout|response-time levels set budget (../methods/thresholds-and-formulas.md)|acknowledge at once; show processing state; block resubmission (error prevention); past ~15 s explain current activity|

- If response > 400 ms → speed it up / mitigate; spinner mitigates wait but does not meet Doherty Threshold.
- Response-time levels from 1968 work: acknowledge routine request within 2 s; ~15 s = hard break.
- Doherty Threshold's 400 ms usually out of reach for payment processing → mitigate wait instead.

Law files: ../laws/fittss-law.md, ../laws/doherty-threshold.md, ../laws/working-memory.md.

## Flows, onboarding, change + endings
|Symptom|Candidate laws|Fix|
|---|---|---|
|Multi-step flow abandoned midway|Goal-Gradient Effect, Zeigarnik Effect|step counter / progress bar + small, truthful head start. Caveat: both laws = design takeaways here → confirm w/ per-step drop-off rather than assuming they cause it|
|New users ignore tour|Paradox of the Active User|contextual tooltips, progressive reveal + get-started checklist people can return to|
|Redesign triggers backlash|Jakob's Law, Mental Model|temporary opt-in w/ preview, feedback + way back|
|Team wants novel pattern users find slow|↑|deviate only if pattern much better once learned + users stay long enough to learn it + team can scaffold learning; judge by comparing learning curves, not first use|
|Experience remembered badly despite good average|Peak-End Rule|fix worst moment + ending; add positive confirmation screen|
|Good session soured at last step|↑|no exit pop-ups / upsells; errors + outages communicated calmly, w/o blame + w/ time estimate; progress bars accelerating at end|

Law files: ../laws/goal-gradient-effect.md, ../laws/zeigarnik-effect.md, ../laws/paradox-of-the-active-user.md, ../laws/jakobs-law.md, ../laws/mental-model.md, ../laws/peak-end-rule.md.

## Testing, real content + team judgment
|Symptom|Candidate laws|Fix|
|---|---|---|
|Polished prototype tests well but real use fails|Aesthetic-Usability Effect|measure task success separately from ratings|
|Layout breaks w/ real content|Aesthetic-Usability Effect, Postel's Law|design + review w/ longest, shortest + missing real values, larger fonts + long translations|
|Team reads small test result as decisive|Cognitive Bias (framing, bias blind spot)|flip frame; report counts w/ confidence intervals; get outside review|

Law files: ../laws/aesthetic-usability-effect.md, ../laws/postels-law.md, ../laws/cognitive-bias.md.

## Related
- write-a-finding.md: fixed shape, confidence labels + severity for finding once its law picked.
- law-misapplications.md: check candidate law not stretched before citing it.
- ../laws/index.md: all 30 UX laws by theme w/ core idea, design rule + decision matrix.
- ../checklists/usability-review.md: yes/no questions by theme, each tied to law; every 'no' = finding.
- ../checklists/usability-heuristics-map.md: classic heuristics mapped to laws, used when no law explains problem.
- ../methods/thresholds-and-formulas.md: response-time limits, target sizes + formulas behind fixes.
- ../ethics/anti-patterns-and-humane-alternatives.md: humane-design counterpart lookup: common harmful patterns + what to ship instead.
- ../ethics/influence-vs-manipulation.md: tests whether persuasive lever serves person or exploits them.
