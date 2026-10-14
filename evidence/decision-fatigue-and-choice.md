# Decision fatigue and choice

## Use when
- Scope: findings on decision fatigue, choice overload, pull of defaults, loss aversion + framing, each w/ its design consequence.
- Open when setting defaults, sizing / sequencing option sets, or backing choice-architecture decision w/ evidence.
- Backs principles: ../principles/intentional.md, ../principles/empowering.md.

## 1. Decision fatigue
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|People make ~35,000 decisions/day (also quoted as > 35,000)|2022 health-news piece quoting psychology lecturer + clinical researcher|approximate figure from news piece|Automate recurring decisions · remember people's preferences · curate options, not exhaustive lists|
|Exhaustion = frequent end state: daily load of ~35,000 decisions keeps drawing down mental reserves|—|mechanism; frequently, not always|Automate recurring decisions · remember people's preferences · curate options, not exhaustive lists|
|Accumulated decision fatigue impairs judgment|—|finding|Automate recurring decisions · remember people's preferences · curate options, not exhaustive lists|

- View following from decision fatigue: no choice comes free; each spends some of person's attention + time.

- Warning signs of decision fatigue: irritability · hasty / default choices · trouble processing incoming information, e.g. notifications.

## 2. Sizing + ordering option sets
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Jam coupons redeemed more when 6 varieties offered than when 24 offered|grocery field study|classic choice-overload result|Fewer, well-explained options beat catalogs|
|Many-option attributes presented before few-option attributes → more default acceptance|2010 field experiments on product customization|consistent w/ depletion during multi-step configuration|Sequence simple binary choices before long lists|
|Choosing what to stream cost ~10.5 min per session on average|June 2023 streaming consumer survey by media-measurement firm|survey; approximate average|Offer honest shortlist + one-tap access to full, unpersonalized catalog|
|20% of people end up switching to another activity: started undecided, then found nothing|same June 2023 survey|survey|↑|
|Streaming catalogue ~1.6 million titles in early 2020 → ~2.7 million in mid-2023|2023 media-measurement report|approximate counts|↑|
|What people seek from option set = feeling sure about those shown, not more of them|business professor's observation, 2020; resurfaced in generative-search debates|observation|Build confidence via visible sourcing, not by hiding alternatives|

## 3. Defaults under load
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Tennis line-call game w/ default set to "in": harder judgment task → default accepted more often|2010 brain-imaging study|imaging study|Assume default = outcome under load; set it in person's interest|
|Rejecting default showed increased frontal-cortex activity|same 2010 study|imaging finding|Assume default = outcome under load; set it in person's interest|
|Organ-donation consent ~2x higher under opt-out than opt-in|2004 research on defaults + donation decisions; incl. online experiment w/ 161 participants in opt-in, opt-out + neutral conditions|approximate ratio|No defaults where active choice matters (consent, identity, money); elsewhere default to person's well-being|
|In states defaulting to limited-tort plan, 79% chose it; in neighboring state defaulting to full plan, 70% chose full plan|comparison of neighboring states' defaults|real-world comparison|No defaults where active choice matters (consent, identity, money); elsewhere default to person's well-being|
|Raising retirement-saving default from 0 to 3% raised participation but lowered share of people saving > 3%|retirement-saving default change|default change w/ mixed effect: participation up, higher saving down|No defaults where active choice matters (consent, identity, money); elsewhere default to person's well-being|

- Mechanism: defaults act as decisions for people w/ no formed preference.

## 4. Loss aversion + felt ownership
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Losses weigh ~2x as much as equivalent gains|1979 prospect-theory paper|approximate ratio|Never exploit loss aversion to block cancellation / opt-out|
|People told their money already in risky investment tended to keep it there|1988 status-quo research|tendency|Never preselect options for business's benefit|
|Bidders leading longest felt strongest ownership before owning anything|2004 online-auction study|single study|Never preselect options for business's benefit|

- Mechanism: leaving default feels like loss.
- Terms: investment + auction findings show status quo bias + quasi-endowment (= felt ownership before actual ownership).
- Mechanism: pre-selecting option creates felt ownership of it.

## 5. Personalized suggestion as the answer to too much choice
- Case: streaming services now tailor suggestions per viewer as their answer to too much choice.
- Case: Netflix reported > 92 billion hours viewed January to June 2023 (company engagement report for first half of 2023, cited in 2024 essay critical of recommendation algorithms).
- Mechanism: probability of given person enjoying given item, computed from same person's past behaviour, shown beside each suggestion; second stated aim = stretching tastes bit by bit. Hypothetical: public-library app shows fit score beside each book, computed from reader's own past loans; now + then offers pick from neighbouring genre to widen their range.
- Netflix hours figure offered as sign personalized suggestion works.
- Caveat: Netflix hours figure differs between summaries → check citation-caveats.md before quoting it.
- If citing hours watched → they show tailoring holds attention; still ask what this convenience costs in privacy + agency.

## 6. Tiny transaction costs
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|~half of web users expect page within 2 seconds|industry performance study|industry study; approximate share|Small frictions steer behavior → place only where protecting person|
|~40% of web users abandon pages slower than 3 seconds|same industry study|industry study; approximate share|Small frictions steer behavior → place only where protecting person|

- Mechanism: even tiny transaction costs change behavior.

## 7. Framing
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|> 80% of people judge "a bank teller active in women's rights" more likely than "a bank teller"|classic cognitive-psychology studies|classic result|Tidy personas + framed data incomplete → check framing before deciding|
|Relabeling "a box of tacks" as "a box and tacks" markedly raises solve rates in candle problem|candle problem|marked rise|Tidy personas + framed data incomplete → check framing before deciding|

- Term: conjunction fallacy = richer story beating probability: more detailed description judged more likely.

## Related
- ../patterns/defaults-and-choice-architecture.md: defaults, opt-in, equal-weight decline + symmetric exit.
- ../patterns/lists-options-and-choice.md: usability side: option counts, ordering + comparison.
- ../laws/choice-overload.md: law behind many-options findings, w/ its limits.
- ../laws/hicks-law.md: decision time as options grow.
- ../laws/cognitive-bias.md: systematic biases e.g. those in loss-aversion, status-quo + framing findings.
- ../patterns/friction-undo-and-confirmation.md: where to place small frictions so they protect.
- convenience-and-friction.md: neighbouring evidence on what removing / adding friction does.
- citation-caveats.md: traps + limits to check before quoting these figures.
- ../principles/intentional.md, ../principles/empowering.md: principles this evidence backs.
