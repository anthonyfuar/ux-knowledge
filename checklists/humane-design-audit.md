# Humane-design audit

## Use when
- Auditing product, feature / flow against humane-design principles + AI and automation.
- Structure: 1 yes/no block per humane principle (Respectful, Finite, Empowering, Intentional, Inclusive, Resilient, Transparent) + 1 cross-cutting AI and automation block. Each question + what to look for ("Passes when").

## How to run
1. Answer each question yes / no.
2. "No" = finding, not failure.
3. Per "no" → log principle + screen + proposed fix.
4. Per block → also check related principles. Why: decision touching one principle touches its neighbours.

## Blocks + neighbours
|Block|Means|Also check|
|---|---|---|
|../principles/respectful.md|care for people's well-being, attention + time|Resilient, Transparent, Empowering|
|../principles/finite.md|bounded, high-quality time w/ product|Intentional, Inclusive, Resilient|
|../principles/empowering.md|people's gain over product's earnings|Transparent, Resilient, Finite|
|../principles/intentional.md|weigh long-run consequences; add friction on purpose|Finite, Inclusive, Resilient|
|../principles/inclusive.md|design for people in all their variety|Intentional, Finite, Resilient|
|../principles/resilient.md|expect abuse; shield vulnerable|Respectful, Finite, Inclusive|
|../principles/transparent.md|no deceptive patterns; honest intent|Respectful, Empowering, Resilient|
|AI and automation|cross-cutting block, not its own principle|Empowering, Transparent, Resilient, Intentional|

## Respectful
|Check|Passes when|
|---|---|
|Urgency to person, not business, picks notification channel?|sound, vibration / lock-screen only when time-sensitive; else badge, inbox / digest|
|People choose channel, time + sender of their notifications?|per-sender, per-category + per-channel toggles + quiet hours, not one global switch|
|Emails carry full message body?|no 'tap to view' teasers forcing person back to product|
|Delivery adapts to meetings, driving, sleep + focus?|deferred / softened in those contexts, not identical pings everywhere|
|Could this sit at attention's periphery, not its centre?|ambient indicators, tones, subtle badges preferred over modal alerts|
|Read receipts, presence + 'seen' indicators opt-in for observed person?|yes; red flag = these controls held only by observer|
|No rating nags, install banners + forced sign-in to view content?|none. Why: they serve business + score negatively on well-being|

## Finite
|Check|Passes when|
|---|---|
|Visible 'all caught up' state?|feed ends when new content ends; no silent recommendation backfill|
|Person triggers Load More, or continuous loading justified for this task?|infinite scroll only for aimless browsing of homogeneous content; paging for search, comparison + goal-directed lists|
|Autoplay yields to 'up next' card needing deliberate tap?|no countdown on card; autoplay off by default for minors|
|Moderation prompts after extended use?|'still watching?' check-ins, session-intent prompts, time-spent dashboards|
|Offers small amount of meaningful content, not volume?|no padding to extend sessions|
|Can people see elapsed time, pause + set enforced limits?|timers pause app when set time used up|
|Every reward predictable + scheduled, not variable payoff?|no jackpot-like pull-to-refresh; no badge counts withheld / unpredictable|

## Empowering
|Check|Passes when|
|---|---|
|Can people inspect, tune, mute, reset + bypass ranking?|chronological / following-only view 1 tap away; 'why am I seeing this' on recommendations|
|Privacy + anonymity controls clear, reachable + protective by default?|anonymous / no-account mode where feasible|
|Stays out of way until summoned?|quiet by default; no constant suggestion surfaces|
|Healthier habits supported by showing people own usage patterns?|yes; streak-only usage feedback pushing more use does not pass|
|AI decisions: can person understand, review, correct + approve before they take effect?|legible reasoning + confidence level + path to correct decision|
|When personalization narrows view, can people find hidden content?|full catalogue + unpersonalized mode stay accessible|
|Leaving as easy as joining?|cancel, unsubscribe + delete use same channel + step count as sign-up|
|Anyone asked what people gave up, not only whether task finished?|time, attention, money + privacy spent reported beside completion rates|

## Intentional
|Check|Passes when|
|---|---|
|Confirmation effort proportional to action's irreversibility + reach?|inline confirmation for harmless, menu for moderate, type-to-confirm for catastrophic; delay-then-undo for sends|
|No purchase, share, publish / send completes on one unguarded tap?|confirmation proportionate to consequence; if missing → identify beneficiary of its absence|
|Defaults favour well-being, privacy + person's intent?|opt-in for data collection + add-ons. Why: most people never change defaults|
|Consent, identity, money + relationship choices: no preselected answer?|neutral active choice; nothing pre-ticked / pre-highlighted|
|Algorithmic speed bumps (rate limits, delayed amplification, forwarding caps)?|present. Why: they slow abuse + cascading harm|
|Team weighed consequences over months + years, not only next quarter?|../methods/futures-wheel.md / ../methods/premortem.md in decision record|

Step-removal note:
- Per step design removes → record: load-bearing (created deliberation, ownership / commitment) or mere tedium.
- Load-bearing step removed → finding in itself.
- Tedium-only step removed → no finding.

## Inclusive
|Check|Passes when|
|---|---|
|Team reflects diverse abilities, backgrounds + lived experience?|actual representation on team, not empathy exercises|
|Disability = starting constraint, + assistive contexts tested?|tested w/ keyboard only, screen reader, 200% zoom + visible focus|
|Platform's own accessibility preserved?|text-size scaling, contrast settings + pinch-zoom all still work|
|Can people switch off motion, parallax + endless feeds?|reduced-motion + paginated alternatives exist|
|Works for permanent, temporary + situational limitations?|one-handed, in glare, noise, second language, w/ anxiety + low bandwidth|
|Error messages honest about whose fault, + give next step?|no generic 'something went wrong' reading as person's own failure|
|Defaults stricter for minors?|no late-night pushes, autoplay off, break reminders on|

## Resilient
|Check|Passes when|
|---|---|
|Every use case has written misuse case + mitigation at launch?|misuse work not deferred to never-arriving 'later'|
|Person sets audience for own information; safest option = default?|personal settings always override group + admin actions|
|Block, mute, report + appeal specified in each direction?|report gets acknowledgement, decision + recourse; reporting tool itself not weaponizable|
|Safeguards still hold when attacker shares person's home, passcode / account?|intimate-partner threat model exists, not only stranger one|
|Doxxing surface audited so no field combination locates / identifies person?|aggregation across profile, activity + metadata considered; fields team cannot justify → dropped|
|Degrades gracefully when battery, network / servers fail?|offline mode, low-speed mode + route to human|
|Abuse instrumented beside growth?|tracked: unreplied first messages, block rate after messaging, moderation false positives|
|Quantitative findings checked against interviews, observed sessions + support tickets?|results segmented after every experiment; product staff sat w/ support queue. Why: numbers record only what people did; reasons why come from people alone|

## Transparent
|Check|Passes when|
|---|---|
|Before sign-up, every item person agrees to spelled out?|plain-language summary beside full terms|
|Per data request: purpose stated + collection opt-in?|permission prompts explain feature needing it|
|Can people find, view, export + permanently erase their data?|delete = delete, not deactivate|
|Full price, incl. mandatory fees, shown where price first appears?|no surprises added at last step|
|Consent sentences short, positively phrased, unchecked by default + consistent in what on / off mean?|no double negatives; no pre-ticked consent boxes|
|Ads unmistakably distinct from content, navigation + generated answers?|ads labelled + in separate slots|
|Every control does exactly what its label says?|close closes; decline as visible as accept|
|Team scanned own site for trackers it cannot justify?|scan covered third-party cookies, fingerprinting, session recording, platform pixels|

## AI and automation (cross-cutting)
|Check|Passes when|
|---|---|
|Always clear person deals w/ machine, not human?|machine disclosed at first turn + in transcript; no synthetic persona inviting trust owed to humans|
|When system acts on someone's behalf: proportionate confirmation + undo?|draft-and-approve for anything sending, spending, publishing / changing relationships; delay-then-undo where asking approval too costly|
|Reasoning visible enough so reviewer could disagree w/ it?|inputs, intermediate steps, confidence + sources exposed. Rubber-stamp review queue w/ nothing to inspect = not human oversight|
|Consequential decisions have named appeal route + stated timeframe?|human decision-maker handles appeal; specific explanation of what triggered outcome; answer by promised date|
|People's writing, uploads + speech excluded from model training unless they opt in?|training opt-in w/ stated purpose; no silent repurposing of data collected for something else|
|New AI capability off by default for existing accounts + removable?|capability offered, not switched on; way back to previous behaviour|
|Accuracy measured separately for each population system touches?|error rates segmented by language, skin tone, age, disability, dialect + device. Why: aggregate accuracy hides groups bearing failures|
|System safe when meeting distress, crisis / harm signals?|tested crisis paths w/ escalation to human; no cheerful continuation of harmful thread; guardrails on self-harm, medical, legal + financial queries|

## Related
- [Principles index](../principles/index.md): seven humane-design principles side by side + how to use them as review lens.
- ../guides/review-an-interface.md: steps for usability + humane-design review.
- ../guides/write-a-finding.md: fixed shape, confidence labels + severity ranking for logging each "no".
- [Usability review checklist](usability-review.md): usability-side yes/no questions, each tied to UX law.
- ../ethics/deceptive-patterns.md: deceptive-pattern taxonomy + honest alternative to each; backs Transparent block.
- ../patterns/ai-and-automated-features.md: patterns behind AI and automation block.
- calm-technology-scorecard.md: scores attention, notifications, privacy, well-being + failure states.
- ../ethics/ethics-review-workflow.md: steps for feature ethics review before launch.
- ../methods/futures-wheel.md + ../methods/premortem.md: methods whose record answers long-run consequences check.
