# Common mistakes in applying UX laws and humane design

## Use when
- Before delivering review / rationale / recommendation → check against both lists below.
- Two lists, most damaging misuses: (1) usability mistakes = laws stretched past what they explain + overstated evidence; (2) humane-design mistakes.
- Full table, wrong uses of each law w/ correction → law-misapplications.md.

## Usability mistakes: law attached to a behaviour it does not explain
Rule: identify mechanism first → then pick matching law; if none fits → cite usability heuristic (../checklists/usability-heuristics-map.md).

|Wrong|Why it fails|Cite / do instead|
|---|---|---|
|Cap menu at seven items citing ../laws/millers-law.md|seven = reason to chunk, not option limit; underlying memory capacity may sit nearer four items than seven|chunk|
|Size unordered menu w/ ../laws/hicks-law.md|unordered lists scanned linearly; logarithmic benefit needs ordered list + user knowing target|—|
|Cite Hick's Law for screens w/ no choice to make (tour slides, sequential information)|says nothing about them|../laws/cognitive-load.md|
|Cite ../laws/doherty-threshold.md for 0.1 s pressed state of control|concerns system response time; does not cover pressed state|—|
|Cite Doherty Threshold for double-charge prevention|does not cover it|error prevention + idempotency|
|Cite ../laws/peak-end-rule.md for Skip tap mid-journey|covers emotional peak + episode's real end|always name both halves, peak + end; never ending alone|
|Cite ../laws/fittss-law.md for control users never find (e.g. Save button at bottom of long scroll, off-screen action)|assumes visible target at already-known location + predicts movement time only|../laws/selective-attention.md + visibility-of-system-status heuristic|
|Frame slips between adjacent buttons mainly via Fitts's Law|—|main frame = error prevention + spacing; Fitts's Law only supporting argument|
|Cite ../laws/choice-overload.md for many independent settings|needs single choice among close substitutes; sixty separate toggles → scanning + finding load|Cognitive Load, Selective Attention, ../laws/chunking.md, progressive disclosure, ../laws/teslers-law.md (relocate complexity)|

## Usability mistakes: protective-interface evidence misdescribed
Law: ../laws/paradox-of-the-active-user.md.
- Wrong: 1984 training-wheels study = hiding features / tooltip support.
- Right: every menu choice stayed visible; advanced, error-prone choices disabled; selecting one → message + no change. Learners lost less time on errors.
- Caveat: evidence = one study of word processor.
- Caveat: early results from 1985 suggested some protective interfaces hurt later learning.

## Usability mistakes: judging, simplifying + reviewing in ideal conditions
|Wrong|Why it fails → do instead|
|---|---|
|Judge design difficulty by how easy team finds it|designers + developers have above-average working memory (../laws/working-memory.md); real users often tired, stressed, older / distracted|
|Simplify until controls turn abstract|per Tesler's Law, complexity must live somewhere → clarity beats minimalism (Cognitive Load)|
|Read good ratings of polished prototype as usability proof; trust ideal-content demo|→ review designs w/ messy real content, sparse data + low-end devices|

## Usability mistakes: overstated evidence
Overstated evidence = common usability mistake. State each law / claim at real strength:

|Law / claim|Honest label|
|---|---|
|../laws/parkinsons-law.md|from humorous essay, not research|
|../laws/pareto-principle.md|80/20 split approximate|
|Doherty Threshold|1982 figures behind it vendor-authored|
|../laws/goal-gradient-effect.md|rests on animal studies + 2006 human field study w/ real rewards: customers accelerating more toward first reward more likely to earn another reward + returned sooner. Never restate this evidence as finding on why people drop out|
|Complexity bias|1989 study illustrates it well: most participants proposed rules more elaborate than hidden one (simply any three ascending numbers); study's own conclusion = reasoning strategies shift w/ task, not complexity bias. Three-number rule-discovery task: 1960 work|

## Humane-design mistakes
|Mistake|Why it harms → what to do|
|---|---|
|Treat seven humane-design principles as checklist to pass, not critique to run|→ each 'no' = finding to fix; check neighbouring principles for each fix ([principles index](../principles/index.md))|
|Remove all friction to raise conversion|wrong when it removes load-bearing effort carrying deliberation, ownership / learning (../patterns/friction-undo-and-confirmation.md)|
|Confirm trivial actions (reverse mistake)|trains people to click through confirmations on autopilot|
|Add 'diverse viewpoints' to feed w/o context|abrupt contradiction w/o context hardens beliefs rather than opening them|
|Optimize one growth metric w/o user-goal metric / counter-metric beside it|cultures built around single metric breed deceptive patterns (../methods/counter-metrics.md)|
|Treat legal review as last ethical checkpoint|law lags harm by years; legal ban removes one trick, leaves sibling tricks in place|
|Threat-model only strangers as attackers + only additions to product|→ feature removals + attackers living w/ victim need same threat review as additions + strangers (../patterns/safety-and-abuse-resistance.md)|
|Hold one ethics workshop, record it, never revisit it|foresight work not changing roadmap = theater|
|Test only in quiet, well-lit, connected rooms on designer hardware|most common screen small, typical connection slow|
|Fix harmful mechanic w/ copy|wrong when mechanic's unit itself = problem|
|Decline growth mechanic w/o offering retention path to replace it|room then rejects objection, even when sound|
|Apply adult engagement settings to minors|→ age-aware defaults, now industry baseline: no late pushes, autoplay off, breaks on, private by default|
|Turn every notification on at sign-up|—|
|Send likes + promotions on same buzzing channel as urgent messages|trains people to ignore alerts; each disruption reportedly costs ~25–45 min refocusing|
|Reuse data collected for one purpose (security, health, learning) for another by default|breaks trust even if original collection consented → keep data bound to its purpose; announce any new use first; leave new uses off by default|
|Loose statistics: rounding, combining rows, presenting expert opinion as study, repeating debunked parables e.g. oak-beam legend|→ carry hedge w/ number wherever it travels (../evidence/citation-caveats.md)|
|Assume homogeneous team can imagine misuse / exclusion|→ representation + co-design w/ people w/ lived experience beat empathy exercises + simulations|
|Put delight over rights|charming onboarding animation layered on opaque data practices = not good design|

- Caveat on two figures: interruption-recovery time + phone-check-frequency ranges both reported figures, from expert article / method-dependent study set; neither = settled measurement.

## Hypothetical examples
- Hypothetical (removal needing threat review): family banking app drops second-device confirmation of new payee → household member w/ phone access can add self as payee unnoticed; removal serves attacker living w/ victim.
- Hypothetical (copy fix, harmful unit kept): workplace chat tool ranks staff by reply speed; softer wording on 'slowest responder' badge → speed ranking still does damage.

## Related
- law-misapplications.md: full table, wrong uses of each law w/ correction.
- core-stance.md: laws = heuristics, people over metrics, rights rank over effort over delight.
- ../evidence/citation-caveats.md: contested numbers, misattributions + limits of each evidence body; check before quoting any figure.
- [Principles index](../principles/index.md): seven humane-design principles as review lens, w/ neighbours to check for each fix.
- ../checklists/humane-design-audit.md: yes/no questions per principle; each 'no' = finding to fix.
- ../methods/counter-metrics.md: pairs each growth metric w/ harm it could hide.
- ../patterns/friction-undo-and-confirmation.md: grades confirmation by consequence, between removing all friction + confirming trivial actions.
- ../patterns/safety-and-abuse-resistance.md: misuse cases, vulnerable people + children.
- ../checklists/usability-heuristics-map.md: heuristic to cite when no law fits.
