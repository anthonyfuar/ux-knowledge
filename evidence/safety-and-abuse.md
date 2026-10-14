# Safety and abuse

## Use when
- Scope: harassment, stalking, intimate-partner abuse + other harm done through products: tracking devices · moderation + enforcement · privacy overrides · missing confirmations · biased detection systems.
- Open when threat-modelling feature locating, observing, labeling / connecting people; when deciding how much safety friction to add; or when safety finding needs documented case.
- Backs principles: ../principles/resilient.md, ../principles/transparent.md, ../principles/inclusive.md.

## 1. Item trackers + location
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Apple's AirTag item tracker accurate enough to double as stalking tool|month-long 2022 technology-news test|journalistic test|Threat-model intimate partner sharing home + passcode|
|In 2022 test, AirTag located person to within ~one block, refreshing every 2-4 min|same 2022 test|journalistic test; approximate range|↑|
|Person carrying AirTag got sound alert after 17 hours; phone alert only after > 24 hours|same 2022 test|single test|Minimize time-to-detection of unwanted tracking w/o causing alert fatigue|
|Cohabiting scenario in 2022 test: no AirTag alert for two days|same 2022 test|single test|Minimize time-to-detection of unwanted tracking w/o causing alert fatigue|
|AirTag's original alert window 72 hours, later cut to 8-24 hours|product change|documented|Minimize time-to-detection of unwanted tracking w/o causing alert fatigue|
|AirTag's ~60-decibel chirp easily missed, stops before device found, useless while driving / to deaf users|product limit|approximate loudness|Distinguish tracker moving w/ you from one merely near you; give tracked person discreet way to stop tracker + report it|
|Stalkers rarely strangers; most often current / former partners|domestic-violence technology-safety advocates|advocates' report; holds most often, not always|Threat-model intimate partner sharing home + passcode|
|Tiny trackers found sewn into teddy bears + purse linings years before mainstream item tags existed|documented cases|case|Warn at tracker setup: tracking people = crime in many places; tie tracking units to accounts for accountability|
|February 2022: Apple announced anti-stalking features for AirTags: setup warnings, earlier alerts, louder tones, precision finding, on-screen alerts whenever device sounds, serial numbers courts can subpoena|company announcement|case|Warn at tracker setup: tracking people = crime in many places; tie tracking units to accounts for accountability|
|In 2022 update Apple said misuse incidents rare but each one too many|company statement|company's own view of frequency|Warn at tracker setup: tracking people = crime in many places; tie tracking units to accounts for accountability|
|Benign triggers of tracker alerts include borrowed keys|—|case|Minimize time-to-detection w/o causing alert fatigue; distinguish tracker moving w/ you from one merely near you|
|Misuse protection at level of Apple's 2022 update absent from majority of numerous rival item trackers on sale|—|majority of rivals lack it, not all|Distinguish tracker moving w/ you from one merely near you; give tracked person discreet way to stop tracker + report it|

- Mechanism: abusers reconstruct person's routines from location pings.
- Mechanism: familiar brand makes tracking feel innocuous.

## 2. Moderation + enforcement
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Game studio sent automated messages 5-10 min after ban, quoting offending chat log → three-month reoffending fell below 8%|report on studio's moderation practice|single company's practice|Enforce standards quickly + cite exact behavior triggering sanction|
|One microblogging platform suspended ~1,100 accounts tied to jihadist group but only 7 tied to white nationalism|university extremism-research study|one study; first count approximate|Audit enforcement for consistency; put safety over speech; inaction = choice|
|In extremism study, white-nationalist accounts had > 7x followers + posted ~25x more than jihadist ones|same extremism-research study|one study; ratios approximate|Audit enforcement for consistency; put safety over speech; inaction = choice|
|In 2019 workplace-chat company removed 28 hate groups w/ no violation of its policy|historical case|case|Act on stated values, not only on letter of acceptable-use policy|
|Payments company acted against hate groups only after 2017 rally + three years of flagging by civil-rights groups|↑|case|Act on stated values, not only on letter of acceptable-use policy|
|Domain registrar dropped neo-Nazi site; other companies followed|↑|case|Act on stated values, not only on letter of acceptable-use policy|

- Mechanism: fast, specific feedback changes behavior.
- Platform enforcement inconsistent across ideologies.
- Mechanism (historical cases, 2017-2019): companies react to peers; one firm acting on its values pressures others.

## 3. Visible protection cues
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Optional profile-picture guard on large social network made people 75% less likely to copy guarded pictures|—|case|Add visible protection cues; even small friction changes behavior|
|W/ profile-picture guard, screenshots of guarded pictures blocked on one mobile platform|—|case|↑|
|Women avoided uploading photos for fear of stalking|research in India|finding|↑|
|Social network's team acknowledged it should have anticipated women's fear of uploading photos|company statement|case|↑|

## 4. Privacy overrides + observation features
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|College student outed when group admin added her to queer chorus group + group's privacy setting overrode her personal settings; she got disowned, later attempted suicide|documented case|case|Person's own privacy settings must always win over group, admin / automated actions|
|Company engineer publicly blamed group admin for outing|same case|case|Person's own privacy settings must always win over group, admin / automated actions|
|Email client's read receipts reported recipient's location, w/ no opt-out|documented case|case|Observed party controls observation features|
|Email client's CEO said team had not imagined location-tracking misuse; its product + engineering team = 83% men|same case|case; homogeneous teams miss misuse|↑|

## 5. Labeling + cataloguing people
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|One microblogging platform lets anyone put person on public list w/o asking|product behavior|case|Require consent before labeling, grouping / cataloguing another person|
|Hate groups curate public lists of people to organize targeted harassment|documented misuse|case|Require consent before labeling, grouping / cataloguing another person|
|Code-hosting platform requires approval before one account can tag another|product behavior|case|Require consent before labeling, grouping / cataloguing another person|
|People most exposed by public lists, often women, have no say over own cataloguing|historical comparison of 2 platforms|comparison of 2 platforms; often women, not only|Threat-model both additions + removals of labeling, grouping / cataloguing features|

## 6. Crisis features
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Large social network co-developed suicide-prevention tools w/ leading mental-health experts|company case|case|Bring outside experts into anything touching mental health, elections / journalism|
|Social network's proactive detection led to work w/ first responders on > 100 cases in one month|same company case|case|↑|

- Mechanism: pattern recognition spots signs of suicidal ideation on live video.
- Expert involvement beats improvised crisis features.

## 7. Safety friction: sharing, security, purchases
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|In 2018 messaging service limited forwarding in India after viral misinformation contributed to riots|historical case|case|Add speed bumps to sharing + amplification|
|In 2018 video platform tightened monetization to deter spam + extremism|↑|case|↑|
|2018 forwarding limit + monetization change = voluntary friction, accepted despite short-term engagement cost|two 2018 cases above|case|↑|
|Breach exposing data of up to 500 million hotel guests might have proved easier to contain in less seamless, more compartmentalized system|digital-security product manager's argument|argument, not finding; containment only might have proved easier|Step-up authentication + compartmentalization for sensitive actions|
|Devotion to minimizing friction = internet's weakest security link|same expert argument|argued|↑|
|2017: voice-assistant device ordered dollhouse after sentence on TV broadcast triggered it; its default setting asked no confirmation before ordering|documented incident|case|Require explicit confirmation before purchases + any money movement|

## 8. Internal + operator tools
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|January 2018: poorly designed internal screen named as cause of false statewide ballistic-missile warning sent to public|documented incident|read as design failure, not one operator's carelessness|Give operator, admin + internal tools what customer-facing flows get: confirmation graded by severity · dangerous controls separated from routine ones · realistic testing|
|Early + continuous testing w/ internal tool's actual users would have caught missile-warning flaw|argument after incident|argued|↑|

- Highest-consequence screen often one no customer sees.

## 9. Biased detection systems
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Facial recognition still struggles to recognize Black faces|—|finding|—|
|Self-driving detection systems less likely to detect darker-skinned pedestrians|2019 study|one study|—|
|Color film stock historically calibrated w/ white skin as ideal tone → degraded rendering of darker skin|historical case|case|—|

- Homogeneous teams + training data produce biased systems w/ life-or-death consequences.

## 10. Accountability + scale
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Engineer knowingly writing software to cheat emissions tests went to prison|documented case|case; software engineering has no comparable licensing / liability regime|Set your bar above compliance; law lags|
|1% of two billion accounts = twenty million people|expert argument|arithmetic|Count people, not percentages|
|At streaming company in practice, 1% test at music service reaches ~one million people|practice account|approximate reach|Never ship to test cohort what you would not leave in place permanently|

- Wrong: group = "just an edge case" → Right: label hides marginalized people in it.

## Related
- ../patterns/safety-and-abuse-resistance.md: when / do / avoid entries these cases support: misuse cases, blocking + reporting, vulnerable people, children.
- ../methods/misuse-case-brainstorming.md: steps for listing how people could use feature to harm.
- ../patterns/privacy-data-and-security.md: data minimisation, consent, access + deletion, tracking.
- ../patterns/friction-undo-and-confirmation.md: confirmation graded by consequence, undo windows + speed bumps.
- ../patterns/errors-and-input-tolerance.md: usability side: error prevention + recovery, destructive actions.
- unintended-consequences.md: item trackers as dual-use feature + platform harm in fragile contexts.
- inclusion-and-exclusion-costs.md: those left out + what it costs.
- convenience-and-friction.md: what removing / adding friction does.
- ../principles/resilient.md, ../principles/transparent.md, ../principles/inclusive.md: principles this evidence backs.
