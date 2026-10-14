# Inclusion and the cost of exclusion

## Use when
- Sizing accessibility audience, arguing for inclusive work / backing accessibility decision w/ evidence.
- Covers people left out by digital products (disability, low vision, small screens, slow networks, anxiety, situational limits) + what exclusion costs / inclusion returns (lawsuits, gains for everyone, team performance); each row → design consequence.
- Backs principles: Inclusive, Resilient, Respectful.
- Before quoting → check traps + limits in citation-caveats.md.

## Audience size

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|~Half of people have some disability by ~age seventy|Claim on 2019 conference panel by accessibility-consultancy executive|Approximate; panel claim; offered against objection: disabled users = only small percentage|Accessibility = for everybody; plan for aging users|
|22.9 million US adults (9.4%) had vision problems|US national disability + functioning reports, 2014-2015|—|Size assistive-technology audience honestly when prioritizing work|
|39.6 million US adults (16.3%) had movement impairment|Same reports, 2014-2015|—|Size assistive-technology audience honestly|
|32.4% of US adults had at least one basic action difficulty, rising to 60.5% for ages 65 + over|Same reports, 2014-2015|—|Plan for aging users|
|~54% of US adults w/ disabilities used internet in mid-2010s|Industry accessibility guide|Approximate|Size assistive-technology audience honestly|

## Low vision, small screens, slow networks

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|~246 million people worldwide have low vision; not everyone w/ low vision can afford, or chooses, corrective lenses|2014 global health estimate|Approximate|Do not block zoom; never override person's text scaling w/ fixed pixel sizes|
|Mobile devices = 51.3% of internet traffic in 2016; mobile interfaces often read outdoors on glossy screens|Traffic-measurement study|—|Minimum contrast: 4.5:1 for normal-size text, 3:1 for large text|
|Most common screen resolutions: 360x640 on mobile (28.86%), 1366x768 on desktop (9.87%) → far below designers' own displays|2017 survey|—|Review designs on real mid-range phones + small laptops|
|Average global connection speed ~7 Mbps in late 2016; US 16, Egypt 3|Connection-speed reports|Approximate|Heavy pages exclude slow-network users → test throttled to target region's connection speed|
|89% of users rate quick access as major requirement|—|—|Trim scripts + media to keep pages light|

## Stress and conventions

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Half of US adults found new technologies stressful|2009 survey|—|Assistive-technology compatibility reduces stress; follow interface conventions, save invention for content|

## Gains for everyone

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Accessibility work for deaf people improves usability + readability for everyone; clarity gains reach people w/ no hearing loss at all|2019 conference talk by inclusive designer|—|Solve for one, extend to many|
|In series of cases, every accessibility improvement also improved design for people w/o disabilities|2015 talk by accessibility consultant + 2019 panel|Series of cases|Treat accessibility as innovation lever, not compliance cost|

- Wrong: accessibility work inherently slow → Right: feels slow because teams still learning it.

## Legal duty and litigation

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Pop star's website sued in 2019 for failing visually impaired users|Case listed in design thesis|Documented case|Expect accessibility litigation|
|Large retailer earlier settled accessibility lawsuit for millions|—|↑|↑|
|European governments must make public websites accessible under UN disability convention|Legal duty|—|↑|

Lawsuits + legal duties = legal + financial arguments for accessibility; preferred reason = teams should do it because they can → lead w/ positive case.

## Standards and readability

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|WCAG 2.0 (W3C standard): 12 guidelines under 4 principles, 3 conformance levels|Standard|—|—|
|Fog index of ~8 = working readability threshold for general text|—|Approximate; WCAG does not require writing at eighth-grade reading level|Write general text at roughly eighth-grade reading level|

## Representation and team performance

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Women's entrepreneurship organization made previously excluded low-income, immigrant + minority women program leaders → more diverse audiences + much higher turnout|Consulting case, design-for-diversity practice|Documented case|Give excluded people decision power|
|Writers' program discovered it mostly served educated, upper-class white women|Consulting case|↑|Name excluded source|
|Surgical checklist modeled on pilots' checklists cut avoidable operating-room errors despite resistance|Book on checklists written from surgical practice|Documented case; offered as rationale for bias checklists in design|Habitually ask: who sits at the table? Worst case + on whom?|
|Teams outperform individual decision-makers 66% of time|2017 research summary in business magazine|—|Recruit people w/ lived experience onto team|
|Team performance climbs w/ diversity: all-male teams made better business decisions 58% of time, gender-diverse teams 73%, teams also diverse in age + geography 87%|Same 2017 summary|—|↑|

- Wrong: empathy exercises can stand in for representation → Right: empathy exercises = not substitute for representation.

## Motion

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Motion effects of major operating-system release caused nausea for users w/ vestibular disorders|Historical case|Documented case|Let person switch off each of: infinite scroll, autoplay, animation + parallax|
|Interface motion can trigger discomfort / seizures|—|Can|Each motion feature switchable off by person|

## Mismatch and the persona spectrum
Disability arises from mismatch between person + their environment.

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Gamer relying on voice recognition displayed dozens of two-handed controllers as physical record of mismatches between products + person|Book on inclusion|Documented case|Find + fix mismatches your own product creates|
|Exclusion can take permanent, temporary / situational form|Large software company's inclusive design toolkit|Can|Map each ability design assumes across persona spectrum (permanent, temporary, situational)|
|Mobile technology makes situational limits relevant to nearly everyone|—|Nearly|Map each assumed ability across persona spectrum|

- Hypothetical (situational): warehouse picker in thick work gloves cannot operate small touch control; nurse wearing face mask not recognized by workplace tablet's face unlock.
- Hypothetical (temporary): patient w/ one eye bandaged after minor surgery struggles w/ low-contrast text; person w/ laryngitis cannot use voice entry.

## Anxiety and ambiguity

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Person w/ generalized anxiety froze at marital-status question on medical form|2021 article on designing for anxiety|Documented case|Ask only for data you can justify + offer "prefer not to say" option|
|Another person took forgotten two-year-old insurance login as proof of own poor memory|Same 2021 article|↑|Tell people when failure not their fault|
|For anxious people, interface ambiguity becomes self-blame|—|Mechanism|Ask only for justified data; tell people when failure not their fault|

## Related
- ../principles/inclusive.md: principle backed here; definition, practices, audit questions.
- ../principles/resilient.md: principle backed here.
- ../principles/respectful.md: principle backed here.
- ../patterns/inclusive-and-accessible-design.md: patterns backed here: persona spectrum, accessibility floors, low-end devices, identity.
- ../patterns/forms-and-data-entry.md: usability side; fields, formats, validation timing, accessible errors.
- ../patterns/departing-from-convention.md: usability side; when to follow conventions + when to deviate.
- ../patterns/calls-to-action-and-touch-targets.md: usability side; target size, spacing, placement.
- ../checklists/humane-design-audit.md: yes/no questions per humane principle, incl. Inclusive.
- ../methods/stakeholder-arguments.md: argument structures justifying usability + humane choices.
- citation-caveats.md: traps + limits to check before quoting inclusion figures.
