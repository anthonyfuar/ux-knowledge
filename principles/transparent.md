# Transparent

## In one line
- Transparent = no deceptive patterns, honest conduct, product's aims stated openly.
- Nothing in interface built to mislead; product behaves as it claims; its purpose legible.
- Someone signing up owed clear account of commitment: why recommendation/ad appeared, how to leave, how to inspect + erase their data, what data taken + for what.
- Open when: design/review touches sign-up + consent, pricing, data collection, access, export/deletion, ads, explanations of recommendations/generated answers, cancellation, or any suspected deceptive pattern.

## Core practices
Highest weight; check first.
1. Price, terms + data collected stated specifically, before person commits.
2. At point of collection: what data taken, why + how it earns money.
3. Opt-in, not opt-out.
4. Findable ways to view, export + permanently delete own data.
5. Declining carries same weight as accepting.
6. Controls do what their label says.
7. "Why am I seeing this" on recommendations, ads + generated answers.

## Commitments w/ a pattern entry
|Commitment|Do|Avoid|Entry|
|---|---|---|---|
|Right to know before commitment|total price on first screen||../patterns/privacy-data-and-security.md; total price = hidden-costs row of ../ethics/deceptive-patterns.md|
|Minimal asks|ask only for what task needs + say why||../patterns/privacy-data-and-security.md|
|Purpose binding||repurposing data behind person's back|same|
|Access, export, delete|deletion removes data|deletion only deactivating account|same|
|Two-layer terms + privacy policy|surface relevant fragment at moment of decision||same|
|Own trackers|audit own trackers||same|
|Data, purpose + revenue|explain all three together at point of collection||../patterns/transparency-and-honesty.md|
|Ads|unmistakably ads||same|
|True cost|shown before click||same|
|"If they knew" test|run "if they knew" test||same|
|Consent|opt-in; withdrawal as easy as giving consent|opt-out|../patterns/defaults-and-choice-architecture.md|
|Symmetric exit|symmetric exit + reminder before trial converts||../patterns/defaults-and-choice-architecture.md; trial reminder → ../patterns/monetization-and-growth.md|
|Tags + lists|consent before others attach tags, lists or content to someone's identity||../patterns/defaults-and-choice-architecture.md|
|Deceptive patterns|name + eliminate deceptive patterns||../ethics/deceptive-patterns.md|
|Urgency + activity||manufactured urgency; fabricated activity|same|
|Honest controls|controls do exactly what their label says; decline = same weight as accept||../patterns/transparency-and-honesty.md + ../patterns/defaults-and-choice-architecture.md|
|Explaining ranking|explain recommendations; let interface explain algorithm||../patterns/recommendations-and-personalization.md + ../patterns/transparency-and-honesty.md|
|Generated answers|show sources, admit limits, gate risky queries||../patterns/ai-and-automated-features.md|

## Guidance held here (no pattern entry)

### Delight vs legibility?
- Rule: transparency over delight; legible, honest experience ranks above surprise + flourish.
- Why: charm distracts from what product does w/ people's data.

### Helping people understand their data?
- Do: teach data literacy inside product: explain via settings themselves, as used.
- Do: report people's usage honestly.
- Wrong: privacy policy = education about data → Right: privacy policy does not educate about data.

### Using personal data for tailoring?
- Rule: personal data used for tailoring stays person's own property, held by company only on trust.

## Why it matters
- Product scandals share one root: organizations knowing far more about people than they disclose.
- Term for deceptive patterns coined in 2010.
- Deceptive patterns = precise, deliberate exploitations of cognitive weaknesses.
- Deceptive patterns usually demanded by someone accountable for one metric.
- Deceptive patterns work short-term, then backfire: lawsuits, nine-figure fines, refund spikes + lost trust.

## Key concepts
|Term|Meaning|
|---|---|
|Deceptive patterns|interface tricks leading people to buy, subscribe, share or stay against their intent; engineered, not accidental; identifiable by their density in interface|
|Named deceptive patterns|roach motel; forced continuity; sneak into basket; hidden costs; misdirection; trick questions; disguised ads; bait and switch; friend spam; price-comparison prevention; hidden "no". How each works + its honest alternative → ../ethics/deceptive-patterns.md|
|Persuasion vs manipulation vs coercion|influence w/o duress vs covert behaviour change vs removal of real choice; = white hat, grey, black hat respectively|
|Personalization paradox|people ask for tailoring yet balk at giving up data behind it|
|Creepiness ditch|point where system's accuracy about person stops feeling helpful + starts feeling like surveillance. Tipped by how much got inferred vs given + how far inference goes unexplained, not by result's usefulness. Same recommendation can land on either side depending on whether its provenance visible|
|Data literacy|active transparency enabling people to decide proactively about sharing|
|Surveillance capitalism|economic logic claiming human behaviour as raw material for prediction + modification|
|Luxury surveillance|consumer devices sold under this label extend surveillance capitalism voluntarily|

## Audit questions
Scope: no deceptive patterns + honest intent. All principles' questions → ../checklists/humane-design-audit.md.

|Check|Passes when|
|---|---|
|Ahead of sign-up, every item person agrees to spelled out to them?|plain-language summary beside full terms|
|For each data request, purpose stated + collection opt-in?|permission prompts explain feature needing them|
|Can people find, view, export + erase data for good?|delete means delete, not deactivate|
|Full price, incl. mandatory fees, shown where price first appears?|no surprises at last step|
|Consent sentences short, positive, unchecked by default + consistent in on/off meaning?|no double negatives; no pre-ticked boxes|
|Ads unmistakably distinct from content, navigation + generated answers?|labelled ads in separate slots|
|Do controls do exactly what their label says?|close closes; decline as visible as accept|
|Own site scanned for trackers you cannot justify?|scan looked for third-party cookies, fingerprinting, session recording + platform pixels|

## Neighbours to check
- Check alongside: respectful.md, empowering.md, resilient.md.
- Working w/ neighbours → [Principles index](index.md).

## Related
- ../patterns/transparency-and-honesty.md: entries on honest controls, true cost, explaining algorithm + honesty tests.
- ../patterns/privacy-data-and-security.md: entries on data minimisation, consent, access + deletion, tracking.
- ../patterns/defaults-and-choice-architecture.md: entries on opt-in, equal-weight decline + symmetric exit.
- ../ethics/deceptive-patterns.md: names each deceptive pattern, how it works + its honest alternative.
- ../ethics/influence-vs-manipulation.md: tests: does persuasive lever serve person or exploit them?
- [Business cost of deceptive design](../evidence/business-cost-of-deception.md): evidence on fines, refunds, churn + trust loss.
- ../laws/cognitive-bias.md: usability-side law: status quo bias + loss aversion lie behind pre-checked add-ons, self-serving opt-outs + subscription traps.
- ../guides/laws-and-principles-crosswalk.md: psychological lever each principle guards + principle bounding each law.
- ../checklists/humane-design-audit.md: audit questions for all seven principles together.
- [Principles index](index.md): seven principles side by side + how to work w/ neighbours.
- Pattern files tagged Transparent: ../patterns/ai-and-automated-features.md, ../patterns/recommendations-and-personalization.md, ../patterns/feeds-scrolling-and-pacing.md, ../patterns/defaults-and-choice-architecture.md, ../patterns/privacy-data-and-security.md, ../patterns/safety-and-abuse-resistance.md, ../patterns/transparency-and-honesty.md, ../patterns/monetization-and-growth.md.
