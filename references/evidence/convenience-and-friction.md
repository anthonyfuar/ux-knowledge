# Convenience and friction

## Use when
- Scope: what removing / adding friction does: effort creating value · frictionless sharing · cost of convenience · waiting + perceived thoroughness · step order · effort-based nudges · continuous loading · failure + real-world conditions · softened transitions.
- Open when deciding whether to remove step, add pause / delay, or justify deliberate effort; or when friction finding needs documented case.
- Backs principles: ../principles/intentional.md, ../principles/empowering.md, ../principles/finite.md.

## 1. Effort that creates value
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|People value self-assembled objects more than identical prebuilt ones|2012 consumer-psychology study using storage box|holds only when assembly succeeds: labor → love only w/ successful completion|Keep load-bearing effort (composing, choosing, committing); remove only tedious effort|
|Pencil fastened to brick made handwriting slower, larger + tiring|1962 research report on using computers to extend human intellectual capability|single research report|In creation tool, per-operation cost limits ambition; not polish matter|
|Culture limited to brick-pencil would form different concepts altogether|same 1962 report|argued|In creation tool, per-operation cost limits ambition; not polish matter|
|1962 report's wider claim: effort of setting out careful argument suppresses how often anyone attempts one|same 1962 report|claim|In creation tool, per-operation cost limits ambition; not polish matter|

- Mechanism: effort pays off only w/ successful completion → friction plotted vs value forms bell curve.
- Mechanism: tool's vocabulary + notation bound what ideas can form in it.
- Mechanism: where representation awkward, ambitious work not done badly; not started at all.

## 2. Removing a step: who benefits
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Automatic "frictionless sharing" of app activity to social feed launched 2011, withdrawn by 2012; people said it stripped their sense of control + ownership over what they shared; backlash overwhelming|documented product case|case|Never act / share on person's behalf w/o deliberate per-item decision|
|Frictionless sharing served post volume + ad targeting|same case|case|Never act / share on person's behalf w/o deliberate per-item decision|
|At largest tech companies friction removal reached near-dogma status; industry-wide = fixation|2018 practitioner interviews w/ over a dozen designers, product leads + executives|interviews|When removing step → identify beneficiary; treat ease as trade-off weighed per feature|
|Former platform designers called minimal-effort apps damaging to mental health|same 2018 interviews|practitioners' view|When removing step → identify beneficiary; treat ease as trade-off weighed per feature|
|Convenience overrides stated preferences + makes alternatives seem irrational|2018 legal-scholar essay|argued|Count convenience's costs: skill, reflection, choice + resilience|
|Through habit + scale, convenience breeds monopoly|same 2018 essay|argument|↑|
|Average self-reported life satisfaction across many countries barely moved from 2005 to 2017|global poll data|self-report poll data|Don't equate frictionlessness w/ well-being|
|Growing share of US 8th, 10th + 12th graders report lives lacking purpose|survey findings in book on post-millennial generation|survey|Don't equate frictionlessness w/ well-being|
|Flat life satisfaction + growing lack of purpose came despite boom in smartphones, social media + on-demand services|poll + survey rows above|reading of both trends|Don't equate frictionlessness w/ well-being|

## 3. Waiting + perceived thoroughness
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Airport ended baggage-claim complaints by lengthening walk to carousel → seven-minute carousel wait shrank; before, passengers walked one minute, then waited seven|widely discussed queueing case|case|Cut perceived waiting by occupying people, not by faking speed|
|Coin-counting machine + eye-scan login distrusted when instant, trusted once delay added|practitioner anecdotes|practitioner anecdotes|Visible pause may convey real work; never fake progress for work not happening|
|Social network reportedly added fake progress bar to security check-up|report|reported only; fake progress bar edges into deception|Visible pause may convey real work; never fake progress for work not happening|

- Mechanism: occupied time feels shorter than empty waiting time.
- Mechanism (coin-counter + eye-scan anecdotes): added delay raised trust via perceived thoroughness.

## 4. Step order + effort-based nudges
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Cash machines returning card before dispensing money stopped people leaving cards behind|widely adopted ATM change|case|Reorder steps so payoff comes after whatever people must not forget|
|Sweets in opaque jars + fruit in clear containers shifted employees toward healthier snacks|reported in book on workplace practices at large tech company|case; nudge serving person nudged|Effort-based nudges only when benefiting person; otherwise = dark patterns|
|Clothing-sharing startup got one response to short sign-up survey; after requiring video call to join, filled interview calendar weeks ahead|founder's account|case|Onboarding friction can filter for commitment; stay honest about whom it excludes|

- Mechanism (ATM): step sequencing prevents forgetting; forgetting sets in once person's goal reached.
- Mechanism (startup): required video call signaled exclusivity + worth.

## 5. Continuous loading
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Short interruptions e.g. clicking "Next" can cause task switching on social-commerce platform|2019 information-systems study|one study; shows interruptions can cause switching; not proof they always do|Continuous loading only for goal-free browsing; pagination for finding + comparing|
|Task switching caused by "Next" clicks = main usability argument for infinite scroll on entertainment + news sites|—|argument|Continuous loading only for goal-free browsing; pagination for finding + comparing|

## 6. Failure + real-world conditions
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Connected pet feeder left animals unfed when its servers failed; offline behavior never built|historical case cited in calm-technology guidance|case; graceful degradation matters more as product gets closer to life|Design for product's whole lifespan, incl. dead battery, server down, slow network + user error|
|Head-mounted display, beautifully designed as object, under-tested for social disapproval in everyday settings|↑|canonical case for testing under sub-optimal + social conditions|Test in noise, glare, motion, low battery + socially awkward contexts|

## 7. Softened transitions
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Harsh color divisions draw attention to colors, not data|expert argument citing information-design scholarship|expert argument|Fade, ramp + blend interface transitions instead of jumping abruptly|
|Gradient-softened maps understood faster than maps w/ harsh color divisions|—|finding, source not given|↑|

- Origin: colorful statistical graphics date to 1786.
- Term: gradient softening = applying softened-gradient idea from statistical maps to interface transitions.

## Related
- ../patterns/friction-undo-and-confirmation.md: when / do / avoid entries these cases support: confirmation graded by consequence, undo windows, speed bumps, effort building meaning, nudging w/ friction only when benefiting person.
- ../patterns/feeds-scrolling-and-pacing.md: stopping points, infinite scroll vs pagination + autoplay.
- ../patterns/feedback-loading-and-performance.md: usability side: response-time budgets, indicators + waits.
- ../laws/doherty-threshold.md: usability-side law behind response-time limits; these cases bound when speed alone = goal.
- ../patterns/calm-technology-and-device-etiquette.md: peripheral attention, quiet signalling + failing gracefully.
- ../patterns/defaults-and-choice-architecture.md: defaults, opt-in + never acting on person's behalf w/o deliberate share.
- safety-and-abuse.md: safety cases on friction: forwarding limits added after viral misinformation, order placed w/o confirmation, breach argued harder to contain in seamless system.
- unintended-consequences.md: what removed step quietly regulated + second-order effects at scale in cities + societies.
- ../principles/intentional.md, ../principles/empowering.md, ../principles/finite.md: principles this evidence backs.
