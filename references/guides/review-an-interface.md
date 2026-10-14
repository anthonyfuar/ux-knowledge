# Review an interface

## Use when

- Asked to review, audit / critique existing interface / flow.
- One numbered 10-step sequence covers usability + humane design; each step tagged usability / humane pass + points to files to open.
- New design instead → design-a-screen-or-flow.md runs same two passes.

## Before step 1

1. Take stance + conflict-settling ranking from core-stance.md.
2. Set humane-pass depth w/ how-deep-to-go.md.

## Step map

Usability pass = steps 1, 4, 5, 6, 9; humane pass = steps 2, 3, 7, 8, 10.

|#|Pass|Step|Open|
|---|---|---|---|
|1|usability|Walk the usability checklist|../checklists/usability-review.md|
|2|humane|Audit vs checklist|../checklists/humane-design-audit.md; ../checklists/calm-technology-scorecard.md; ../checklists/interruption-decision-rules.md|
|3|humane|Name deceptive patterns|[deceptive-pattern taxonomy](../ethics/deceptive-patterns.md); ../ethics/anti-patterns-and-humane-alternatives.md|
|4|usability|Confirm the law|../laws/index.md → law's file; ../checklists/usability-heuristics-map.md|
|5|usability|Fix from the surface|surface pattern file (table in step 5); symptom-to-fix-index.md; [pattern catalog](../patterns/index.md)|
|6|usability|Misapplication check|law-misapplications.md|
|7|humane|Check neighbors|[principles index](../principles/index.md) → principle files|
|8|humane|Evidence per finding|evidence theme files (table in step 8); ../evidence/stating-evidence.md|
|9|usability|Verify, then write findings|../evidence/product-cases.md; ../evidence/citation-caveats.md; write-a-finding.md|
|10|humane|Rank + argue|core-stance.md; ../methods/stakeholder-arguments.md|

## Steps 1-10

### 1. Walk the usability checklist (usability pass)

- Walk heuristic ../checklists/usability-review.md checklist theme by theme.
- Every "no" → finding.

### 2. Audit vs checklist (humane pass)

- Answer per-principle yes/no questions in ../checklists/humane-design-audit.md.
- Each "no" → finding in fixed shape of write-a-finding.md.
- If notification-heavy / device product → also score w/ ../checklists/calm-technology-scorecard.md.
- If any behavior interrupts → check vs ../checklists/interruption-decision-rules.md.

### 3. Name deceptive patterns (humane pass)

- Compare every prompt, default, price display, consent sentence + exit path vs [deceptive-pattern taxonomy](../ethics/deceptive-patterns.md).
- If element matches → finding names pattern w/ its humane alternative beside it; quick table of both = ../ethics/anti-patterns-and-humane-alternatives.md.
- If failure has no shared name (e.g. opaque ranking, deferred edge case) → describe plainly; never invent labels.

### 4. Confirm the law (usability pass)

- For each finding: find cited law via [index of the 30 UX laws](../laws/index.md), open its file, confirm mechanism (origin-and-mechanism section, Why it works) + pitfalls (limits-and-pitfalls section, Misreadings and limits) → cited law must truly explain problem.
- If no law explains it → use classic usability heuristics mapped to laws: ../checklists/usability-heuristics-map.md.

### 5. Fix from the surface (usability pass)

Take fix from relevant surface's pattern file:

|Surface|File|
|---|---|
|Navigation + menus|../patterns/navigation-and-menus.md|
|Calls to action + touch targets|../patterns/calls-to-action-and-touch-targets.md|
|Forms + data entry|../patterns/forms-and-data-entry.md|
|Onboarding + first use|../patterns/onboarding-and-first-use.md|
|Search + results|../patterns/search-and-results.md|
|Lists, options + choice|../patterns/lists-options-and-choice.md|
|Content layout, grouping + visual hierarchy|../patterns/layout-grouping-and-hierarchy.md|
|Dashboards + data displays|../patterns/dashboards-and-data-displays.md|
|Feedback, loading + perceived performance|../patterns/feedback-loading-and-performance.md|
|Progress, goals + task completion|../patterns/progress-goals-and-completion.md|
|Errors, input tolerance + edge cases|../patterns/errors-and-input-tolerance.md|
|Complexity management|../patterns/complexity-management.md|
|First impressions + aesthetics|../patterns/first-impressions-and-aesthetics.md|
|Familiar conventions vs novelty|../patterns/departing-from-convention.md|
|Memorable moments + endings|../patterns/memorable-moments-and-endings.md|
|AI, assistants + automated features|../patterns/ai-and-automated-features.md|

- Lookup by observed problem → symptom-to-fix-index.md.
- Every surface, humane ones incl. → [pattern catalog](../patterns/index.md).

### 6. Misapplication check (usability pass)

- Check fix vs law-misapplications.md table → fix adds no new error.
- New error this catches, e.g.: capping menu / list at seven items.

### 7. Check neighbors (humane pass)

- For each finding: check principles in its "Also check" set; set for each of seven principles = [principles index](../principles/index.md).
- Then open principle files: ../principles/respectful.md, ../principles/finite.md, ../principles/empowering.md, ../principles/intentional.md, ../principles/inclusive.md, ../principles/resilient.md, ../principles/transparent.md.
- Why: fix satisfying one humane principle often violates another; confirmation added everywhere → nagging; safety alerts added as fix → alert fatigue.

### 8. Evidence per finding (humane pass)

- Attach claim + its design implication from evidence files.
- Quote numbers exactly as evidence states them.
- Flag whether evidence = expert opinion / study; rules in ../evidence/stating-evidence.md.

|Theme|File|
|---|---|
|Attention + distraction|../evidence/attention-and-distraction.md|
|Addiction + variable rewards|../evidence/addiction-and-variable-rewards.md|
|Children + adolescents|../evidence/children-and-adolescents.md|
|Decision fatigue + choice|../evidence/decision-fatigue-and-choice.md|
|Personalization + surveillance|../evidence/personalization-and-surveillance.md|
|Filter bubbles + polarization|../evidence/filter-bubbles-and-polarization.md|
|Unintended consequences in cities + societies|../evidence/unintended-consequences.md|
|Safety + abuse|../evidence/safety-and-abuse.md|
|Convenience + friction|../evidence/convenience-and-friction.md|
|Inclusion + cost of exclusion|../evidence/inclusion-and-exclusion-costs.md|
|Business consequences of deceptive design|../evidence/business-cost-of-deception.md|

### 9. Verify, then write findings (usability pass)

- Verify any number / study before quoting: Evidence section of law's file, ../evidence/product-cases.md, ../evidence/citation-caveats.md.
- Then write findings in fixed shape of write-a-finding.md, ranked by severity.

### 10. Rank + argue (humane pass)

- Order findings by severity per ranking in core-stance.md.
- Name Blocking findings plainly as must-fix before release.
- Case to stakeholders (long-term revenue, legal + PR exposure, mock headlines, precedents) → build w/ ../methods/stakeholder-arguments.md.

## Related

- core-stance.md: holding laws + ranking ordering severities.
- how-deep-to-go.md: quick pass vs standard review vs full treatment.
- write-a-finding.md: fixed shape, confidence labels, severity ranking, worked examples.
- design-a-screen-or-flow.md: same two passes on new design.
- symptom-to-fix-index.md: observed problem → explaining law → fix.
- common-mistakes.md: most damaging misuses, usability side + humane side.
- laws-and-principles-crosswalk.md: humane principle bounding each law.
- ../ethics/ethics-review-workflow.md: steps for feature ethics review before launch.
