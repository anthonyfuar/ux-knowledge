# Surface-to-principle map

## Use when
- Starting to design/review feature → pick humane-design principles + pattern files to read for its product surface.
- Per surface: principles most affected, where to start, pattern files to open.

## How to read a row
1. Find surface (aliases in brackets).
2. Principles: primary first. Files: respectful.md, finite.md, empowering.md, intentional.md, inclusive.md, resilient.md, transparent.md.
3. Start with: practices to settle first.
4. Open: files listed most specific first (→ = then).

## Map
|Surface|Principles|Start with|Open|
|---|---|---|---|
|Notifications and interruptions (alerts)|Respectful, Finite, Intentional, Inclusive|urgency matching; off by default; quiet hours; context adaptation; age-aware defaults|../patterns/notifications-and-interruptions.md → ../patterns/calm-technology-and-device-etiquette.md → ../patterns/safety-and-abuse-resistance.md|
|Feeds and infinite scroll (scrolling)|Finite, Empowering, Resilient, Inclusive|stopping cues; load-more; variable rewards; algorithm controls; feed accessibility; guardrails for distressed users|../patterns/feeds-scrolling-and-pacing.md → ../patterns/recommendations-and-personalization.md → ../patterns/inclusive-and-accessible-design.md|
|Onboarding and sign-up|Transparent, Intentional, Respectful, Inclusive|right to know; ask in context, not at setup; symmetric exit; anonymous trial; readable copy|../patterns/onboarding-and-first-use.md → ../patterns/privacy-data-and-security.md → ../patterns/defaults-and-choice-architecture.md → ../patterns/inclusive-and-accessible-design.md → ../patterns/forms-and-data-entry.md|
|Settings and controls (preferences)|Empowering, Transparent, Inclusive, Respectful|reachable privacy + notification controls; personal settings overriding group defaults; preserved platform accessibility|../patterns/complexity-management.md → ../patterns/defaults-and-choice-architecture.md → ../patterns/privacy-data-and-security.md → ../patterns/notifications-and-interruptions.md → ../patterns/inclusive-and-accessible-design.md|
|Defaults|Intentional, Transparent, Respectful, Resilient|well-being defaults; opt-in data; no default where active choice matters; safest privacy default|../patterns/defaults-and-choice-architecture.md → ../patterns/privacy-data-and-security.md → ../patterns/notifications-and-interruptions.md → ../patterns/forms-and-data-entry.md|
|Recommendations and personalization|Empowering, Transparent, Finite, Resilient|discoverable hidden options; explain why; unpersonalized view; no rabbit holes; context for contrary views|../patterns/recommendations-and-personalization.md → ../patterns/transparency-and-honesty.md → ../patterns/defaults-and-choice-architecture.md|
|News, editorial and information feeds|Empowering, Transparent, Resilient, Inclusive|context beside contrary views; news space separate from friendship metaphor; editorial curation; rabbit-hole limits; explain ranking; finite edition w/ ending|../patterns/recommendations-and-personalization.md → ../patterns/feeds-scrolling-and-pacing.md → ../patterns/transparency-and-honesty.md|
|Progress, streaks, badges and gamification|Intentional, Finite, Resilient, Inclusive|change counted unit before wording; private + optional by default; pausable runs; reward delivered value; purpose-consistency test; counter-metrics w/ trip threshold|../patterns/habits-streaks-and-gamification.md → ../patterns/progress-goals-and-completion.md → ../patterns/transparency-and-honesty.md → ../patterns/monetization-and-growth.md|
|Health, well-being and mental-health features|Resilient, Inclusive, Transparent, Finite|engagement traces treated as health data; local storage + no advertising use; every tally optional; no comparison ranking; crisis + distress guardrails; no win-back built on low mood|../patterns/safety-and-abuse-resistance.md → ../patterns/privacy-data-and-security.md → ../patterns/habits-streaks-and-gamification.md → ../patterns/recommendations-and-personalization.md → ../patterns/ai-and-automated-features.md|
|Data collection and permissions|Transparent, Respectful, Resilient, Intentional|data minimization; purpose stated at point of collection; no repurposing; threat-model misuse; friction before exposure|../patterns/privacy-data-and-security.md → ../patterns/transparency-and-honesty.md → ../patterns/defaults-and-choice-architecture.md → ../patterns/safety-and-abuse-resistance.md → ../patterns/friction-undo-and-confirmation.md|
|AI features and generated answers|Empowering, Transparent, Resilient, Intentional|human in loop; augmentation over substitution; sources + corroboration; admit limits; gate risky queries|../patterns/ai-and-automated-features.md|
|Sharing, tagging and social mechanics|Intentional, Resilient, Respectful, Transparent|speed bumps on resharing; consent for tags + lists; no manufactured reciprocity; model mechanics at scale|../patterns/friction-undo-and-confirmation.md → ../patterns/defaults-and-choice-architecture.md → ../patterns/recommendations-and-personalization.md → ../patterns/safety-and-abuse-resistance.md → ../patterns/monetization-and-growth.md|
|Purchases, subscriptions and trials|Transparent, Intentional, Empowering|total price first; unchecked add-ons; explicit confirmation; trial reminder; easy cancellation|../patterns/monetization-and-growth.md → ../patterns/transparency-and-honesty.md → ../patterns/friction-undo-and-confirmation.md → ../patterns/defaults-and-choice-architecture.md → ../patterns/forms-and-data-entry.md|
|Error states and failures (errors, failure states)|Inclusive, Resilient, Transparent|say whose fault + what comes next; graceful degradation; human backup; undo|../patterns/errors-and-input-tolerance.md → ../patterns/calm-technology-and-device-etiquette.md → ../patterns/inclusive-and-accessible-design.md → ../patterns/friction-undo-and-confirmation.md → ../patterns/memorable-moments-and-endings.md|
|Account deletion and cancellation|Transparent, Empowering, Resilient|right to be forgotten; exit as easy as entry; step-up authentication on sensitive changes; no confirm-shaming|../patterns/privacy-data-and-security.md → ../patterns/defaults-and-choice-architecture.md → ../patterns/friction-undo-and-confirmation.md|
|Tracking, location and monitoring (location tracking)|Resilient, Transparent, Respectful, Inclusive|intimate-partner threat model; observed person controls signal; cross-platform safety alerts; discreet reporting|../patterns/safety-and-abuse-resistance.md → ../patterns/privacy-data-and-security.md|
|Metrics and success criteria (success measures)|Empowering, Intentional, Finite|people's gain ahead of product's earnings; user-goal metric + counter-metric; assess w/ several signals; segment after tests|no pattern file; method files instead: ../methods/measure-what-you-value.md, ../methods/counter-metrics.md, ../methods/goals-signals-metrics.md, ../methods/reading-experiments-honestly.md, ../methods/engagement-vs-empowerment-metrics.md|
|Products for minors (products used by minors)|Inclusive, Resilient, Finite, Respectful|stricter defaults; protective default when age unknown; no persuasion tactics; sensitive inferred attributes barred from ranking; sleep protection; family controls preserving dignity|../patterns/safety-and-abuse-resistance.md → ../patterns/recommendations-and-personalization.md → ../patterns/feeds-scrolling-and-pacing.md → ../patterns/notifications-and-interruptions.md|

## Related
- [Principles index](index.md): seven principles side by side w/ key practices + neighbours.
- [Pattern catalog index](../patterns/index.md): pattern-entry format + list of all pattern files.
- ../checklists/humane-design-audit.md: yes/no questions per principle + on AI + automation.
- cross-cutting-practices.md: team + process habits for every principle.
- ../guides/design-a-screen-or-flow.md: steps bringing laws + principles into new design.
- ../guides/review-an-interface.md: steps for usability + humane-design review.
- ../guides/laws-and-principles-crosswalk.md: usability half: principle bounding each law.
- ../guides/symptom-to-fix-index.md: usability counterpart: lookup from observed problem to law + fix.
