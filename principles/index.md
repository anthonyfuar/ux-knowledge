# Principles index

## Use when
- Reviewing any product decision for humane design → seven principles side by side; pick principle file to read in full.
- Review any product decision against seven humane-design principles: Respectful, Finite, Empowering, Intentional, Inclusive, Resilient, Transparent. They = layer saying why + which.
- Each principle: own file w/ definition, practices, key concepts, related principles + audit-questions section (yes/no questions).

## Why these principles exist
- Framing: designers shipping these systems own their effects.
- Systems in question = products having turned to preying on known weak spots in human psychology, monetizing personal data + harvesting attention, away from extending what people can do.
- Turn came once mobile devices made attention scarce.

## The seven at a glance
|Principle|Means|Check alongside|
|---|---|---|
|respectful.md|people's well-being, attention + time borrowed by product, owed back w/ value; governed mainly by how + when product interrupts|Resilient, Transparent, Empowering|
|finite.md|experience has edges; quality of time over endless quantity|Intentional, Inclusive, Resilient|
|empowering.md|what people gain outranks what product earns from them; measured by agency, not utility|Transparent, Resilient, Finite|
|intentional.md|quick win weighed vs later + second-hand effects; friction placed deliberately where it supports habits people would endorse, keeps privacy intact + stops abuse|Finite, Inclusive, Resilient|
|inclusive.md|every variation in ability, context, culture, class, language + mental state in scope; method of working, not compliance state|Intentional, Finite, Resilient|
|resilient.md|abuse taken as given; whoever stands to get hurt most designed for first; abusability = successor to usability|Respectful, Finite, Inclusive|
|transparent.md|no deceptive patterns, honest conduct, product's aims stated openly|Respectful, Empowering, Resilient|

## Key practices per principle

### Respectful
- Urgency for person decides delivery channel.
- Notifications off by default, except an essential few.
- Notification controls per sender, per category + per channel + quiet hours.
- Adapt to context + to what people keep ignoring.
- Keep status at periphery of attention.
- No manufactured social obligation.
- No targeting of people's emotional lows.

### Finite
- "All caught up" marker, not silent backfill.
- Load More/pagination, not infinite scroll, where people search/compare.
- "Up next" + deliberate tap, not autoplay.
- Variable rewards turned into predictable, scheduled delivery.
- Visible usage + enforced limits.
- Sleep protected by default.

### Empowering
- People can inspect, tune, mute, reset + bypass ranking, e.g. via chronological/following-only view.
- Hidden options stay discoverable + unpersonalized mode exists.
- Human in loop for AI decisions; can review, correct, approve + appeal.
- Product invisible until needed.
- Leaving as easy as joining.

### Intentional
- Confirmation effort scaled to severity: inline confirmation, menu, type-to-confirm, or delay-then-undo.
- Explicit confirmation before money moves or content shared.
- Algorithmic speed bumps, e.g. rate limits, forwarding caps + delayed amplification.
- Defaults chosen for well-being; no default where active choice matters.
- Second-order thinking, futures wheel + premortem before building.

### Inclusive
- Diverse teams built + retained.
- Disability first, extended across permanent, temporary + situational limits.
- Platform's reduced-motion, text-scaling, contrast + zoom settings kept working.
- Readable copy, honest error states + undo for anxious people.
- Co-design w/ excluded people holding decision power.
- Stricter defaults for minors.

### Resilient
- Misuse case + abuser persona beside every use case.
- Threat-model intimate partner sharing home + passcode.
- Personal privacy settings always beat group, admin + automated actions.
- Block, mute, report + appeal loops fully specified.
- Graceful degradation + route to human.
- Recommenders guardrailed around signals of distress.

### Transparent
- Price, terms + data collected stated specifically before person commits.
- At point of collection: what data taken, why + how it earns money.
- Opt-in, not opt-out.
- Findable ways to view, export + permanently delete data.
- Declining carries equal weight to accepting.
- Controls do what their label says.
- "Why am I seeing this" on recommendations, ads + generated answers.

## Working rules
- Use seven as structured critique: one row each in design-review template.
- Each principle links to 3 neighbouring principles (column "Check alongside").
- Satisfying one principle often quietly violates neighbouring one → always check related set.
- If principles conflict → human rights (privacy, security, accessibility) first, then respect for time + effort, then delight.
- Name people + their goals; don't say "users", "DAUs" or "conversions". Why: vocabulary shapes what counts as success.
- Principle-file convention: practice w/ pattern entry links to file holding it (e.g. notifications + interruptions → ../patterns/notifications-and-interruptions.md); practice w/o pattern entry carries guidance inline.

## Where to go next
|Need|Open|
|---|---|
|Principle's definition, practices, key concepts + related principles|its own file: respectful.md, finite.md, empowering.md, intentional.md, inclusive.md, resilient.md, transparent.md|
|Do/avoid guidance + worked example for each practice|pattern files; start at [Pattern catalog index](../patterns/index.md)|
|Yes/no audit questions|audit-questions section of each principle file; all seven sets together → ../checklists/humane-design-audit.md|
|Principles touched by feature + where to start|surface-to-principle-map.md|
|Team + process habits serving every principle|cross-cutting-practices.md|

## Related
- surface-to-principle-map.md: principles each surface touches first + where to start.
- cross-cutting-practices.md: team + process habits serving every principle.
- ../checklists/humane-design-audit.md: yes/no questions per principle + on AI + automation.
- [Pattern catalog index](../patterns/index.md): pattern-entry format + how to pick surfaces.
- ../guides/laws-and-principles-crosswalk.md: psychological lever each principle guards + principle bounding each usability law.
- ../laws/index.md: usability half: all 30 UX laws grouped by theme.
- ../guides/core-stance.md: people over metrics; rights over effort over delight.
- ../guides/review-an-interface.md: steps for usability + humane-design review.
