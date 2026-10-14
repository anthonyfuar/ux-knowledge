# Write a finding

## Use when

- Writing up any problem found in review.
- Fixed shape, two formats: law-based (usability) + principle-based (humane design).

## Pick the shape

|Situation|Shape|
|---|---|
|Usability pass of review (review-an-interface.md); law / usability heuristic explains behavior|Law-based|
|Humane pass (in design, review / product-ethics question); humane principle at stake|Principle-based|

## Law-based finding

- Fill every field; Confidence label mandatory.

|Field|Contains|Rules|
|---|---|---|
|Law|one primary law (two at most) + mechanism in one clause; pick in [index of the 30 UX laws](../laws/index.md)|Must explain observed behavior. May add year first described, if it strengthens case. No law explains it → cite usability heuristic (../checklists/usability-heuristics-map.md); never stretch law to fit.|
|Observation|what shows on screen / in flow, located concretely||
|Impact on the person|what user experiences: slower, misses something, forgets, makes errors, abandons||
|Recommended change|specific + buildable|not restated principle|
|Confidence|Observed / Inferred / Needs testing|mandatory|
|Verify by|confirming metric / test, e.g. task success, time on step, drop-off at step||
|Severity|Critical / High / Medium / Low||

When no law fits:
- Double-submit protection, idempotency, undo: no law explains these → finding cites usability heuristic.
- Then citable heuristics, e.g. error prevention, visibility of system status (../checklists/usability-heuristics-map.md).

## Confidence labels

|Label|Use when|Rule|
|---|---|---|
|Observed|problem visible in artifact|observation can carry Observed; impact prediction (e.g. "most will leave") never|
|Inferred|problem likely, judged from mechanism||
|Needs testing|problem depends on user behavior / data|label any usage / behavior claim w/o data Needs testing, even if it seems obvious|

- Hypothetical: "most riders only ever buy single tickets", said of transit app w/ no usage data → Needs testing.

## Law-based severity

|Severity|When|
|---|---|
|Critical|blocks task / causes irreversible errors|
|High|frequent failure / abandonment risk|
|Medium|friction / slowdown|
|Low|polish|

- Within one level → rank by affected-user count + frequency.
- Origin: 1994 usability severity-rating scheme weighs frequency, impact + persistence.

## Hypothetical law-based finding

Hypothetical: annual household-benefit renewal on public-services portal.
- Law: Tesler's Law; portal could carry details it already holds, yet hands this work back to applicant.
- Observation: household-members step asks every member + income from scratch, though last year's application on file has them.
- Impact on the person: re-enters what office already knows → task longer than expected; every re-entered field = another entry-error chance.
- Recommended change: prefill step from last year's file, every field editable, w/ single "still correct?" confirmation.
- Confidence: Observed.
- Verify by: household-step time + household-field correction rate.
- Severity: High (abandonment risk).

## Principle-based finding

- One shape for any workflow → two reviewers of same flow give comparable output.

Parts, in order:
1. Surface / screen.
2. Principle + its "Also check" set ([principles index](../principles/index.md), seven humane-design principles).
3. Pattern name, where one exists ([deceptive-pattern taxonomy](../ethics/deceptive-patterns.md)).
4. What happens to the person.
5. Severity.
6. Fix.
7. Evidence: add when fix will face dispute.

Rules:
- "What happens to the person" = the one part never dropped, in prose / table.
- Why: w/o it, finding reads as policy → stakeholders discount it; concrete human consequence → severity arguable + fix worth funding.
- Finding needs shortening → cut evidence clause first.

## Principle-based severity

Ranking order: Blocking → Serious → Minor.

|Severity|When|Consequence|
|---|---|---|
|Blocking|breaks any right: privacy, security, accessibility / safety; ships named deceptive pattern; adds capability to locate, expose / contact someone w/ no misuse mitigation|holds launch gate of ../ethics/ethics-review-workflow.md: nothing ships past it|
|Serious|costs people time, attention / agency; sets default against person's interest||
|Minor|delight, polish / wording||

## Hypothetical principle-based finding 1: a feature end to end

Hypothetical: card-protection add-on offered while customer activates new debit card in banking app.
- Surface: add-on offer during card activation + add-on removal.
- Principle: Transparent; also check Respectful, Empowering, Resilient.
- Pattern: roach motel + forced continuity. Add-on (free for introductory period) accepted in one tap on own activation screen; switch-off needs signed letter to postal address; when free period ends, monthly fee starts w/o any message. Skip button = "No, leave my card unprotected" → confirmshaming.
- What happens: customer never meaning to buy cover pays every month w/o noticing, or must find printer, stamp + postal address to stop it.
- Severity: Blocking, two named deceptive patterns stacked in one flow.
- Fix: switch-off via same in-app toggle as switch-on; message w/ fee + first charge date before free period ends; plainly worded skip button; switch-off confirmed once, w/o screen pleading to keep add-on.
- Evidence: settlement + refund cases reversing revenue held by exit friction. Quote settlement figures as reported range, not single number.

## Hypothetical principle-based finding 2: a ranked surface reaching minors

Hypothetical: school-library audiobook app, on minor pupils' accounts.
- Surface: "Next for you" shelf + self-starting next title.
- Principle: Resilient; also check Respectful, Finite, Inclusive.
- Pattern: bottomless feed (shelf never ends) + autoplay chain (each title rolls into next); shelf ranking uses listening signals, incl. inferred mental-health interest.
- What happens: pupil searching for stories about feeling alone → shelf narrows to ever bleaker titles, next one self-starting long after bedtime. Pupil cannot see what drives shelf, no way to switch it off; inferred interest stays on reading profile through later school years.
- Severity: Blocking, recommender acts on minor's distress signal w/ no mitigation.
- Fix: inferred traits (e.g. mental health, body image, sexuality, politics) kept out of ranking; limit how far shelf can narrow on any one sensitive theme; no auto-start + no endless loading on pupil accounts; visibly ending shelf; break + bedtime defaults on; pupil-facing control clears reading profile; release to a few schools first, comparison group on old shelf + written withdrawal condition.
- Evidence: 2023 human-rights report: feeds steer young people signalling mental-health interest toward self-harm material. Carry as report, not controlled study; no time figure attached.

## Related

- review-an-interface.md: review steps producing findings in these shapes.
- symptom-to-fix-index.md: candidate laws + fix for observed usability problem.
- ../laws/index.md: where law-based finding's primary law gets picked (30 UX laws).
- ../checklists/usability-heuristics-map.md: heuristic to cite when no law explains behavior.
- [Principles index](../principles/index.md): each of seven principles w/ its "Also check" set.
- [Deceptive-pattern taxonomy](../ethics/deceptive-patterns.md): pattern names; shipping any named one = Blocking.
- ../evidence/stating-evidence.md: quoting studies + numbers accurately, in Law field / evidence clause.
- common-mistakes.md: laws attached to behavior they do not explain; loose statistics.
- ../ethics/ethics-review-workflow.md: launch gate held by any Blocking finding.
