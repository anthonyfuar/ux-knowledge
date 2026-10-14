# Unintended consequences in cities and societies

## Use when
- Feature could affect non-users / shared resource.
- Planning entry into new market / fragile context.
- Argument for foresight work needs documented case.
- Covers second-order effects products + built systems had on streets, housing, shared space, public safety + whole societies once adopted at scale, plus support behind two foresight methods (premortem, futures wheel).
- Backs principles: Intentional, Resilient, Inclusive.

## Navigation app reroutes residential streets

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Quiet Los Angeles residential + hillside streets designed for 15-20 mph became jammed cut-through routes due to Waze, navigation app routing by live traffic|Local investigative reporting, 2019|Documented case|Model feature's effects at full adoption, not at early adopters' delight|
|By December 2014, Waze cut-through traffic complaints reached Los Angeles council district of ~100,000 households; 60% of Los Angeles city streets non-arterial|Same case|Approximate household count|Routing system should encode road class + capacity, not only observed speed|
|As adoption grew, drivers' time savings from cut-throughs shrank to seconds|Same case|Documented case|Model effects at full adoption|
|Drivers converge on Nash equilibrium where everyone loses|Simulations by transportation researcher, made before outcome|Prediction|↑|
|Residents of diverted streets had no lever to switch diversion off|Same case|Documented case|Give affected non-users real channel to someone w/ authority to act|
|City data-sharing partnership w/ Waze, announced April 2015, not renewed two years later; officials reported getting stonewalled; council member had to use constituents' personal contacts to get company to return calls|Local investigative reporting, 2019|↑|↑|
|During wildfires, app reportedly routed drivers toward fire|Same case|Reportedly|—|

## Short-stay rentals and housing

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Airbnb (home-rental platform) in New York ignored 2010 dwelling law|2018 technology-magazine article|Documented case|Map laws + norms your product bends|
|By 2016 ~20,000 New York Airbnb listings deemed illegal, fines up to 7,500 dollars; 2018 New York law required hosts to disclose listings, fines up to 25,000 dollars per undisclosed listing|Same case|Approximate listing count|Engage regulators before launch|
|New York City held nearly 50,000 Airbnb listings; top 5 markets = only 4.3% of listings, yet shaped global perception of company|Same case|Nearly|Map laws + norms your product bends|
|Airbnb expected one-year regulatory fight in New York; still fighting eight years later|Same case|Documented case|Engage regulators before launch|
|Report blaming platform for rising rents disputed by report's own data supplier; both sides leaned on numbers other side rejected|2018 reports|Disputed|State uncertainty when claimed harm / benefit rests on contested third-party data|
|Dearer rents + scarcer housing traced in part to Airbnb: owners switch homes to visitor letting wherever it pays better than standing tenancy → locals pay more for what remains + fewer homes left for residents|2018 reporting on short-stay rentals + urban housing|In part; mechanism straightforward, magnitude contested|Ask what scarce local resource your marketplace re-prices; trace where supply moves once more profitable use for it exists; model supply shift before entering market, not after legislation arrives|

## Shared e-scooters in shared space

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Conflicts over shared e-scooters (operators e.g. Bird, Lime, Lyft) fell into 3 groups: safety; clutter / vandalism; reckless riding|2020 researcher summary of comparative study using local news from 10 cities|—|Design end state of anything left in shared space: where it goes, how long it lasts, who cleans it up|
|Appeal: low-cost way to cover short distance in traffic-choked city w/o hired ride / car|Same case|—|—|
|What followed: pedestrians obstructed, streets cluttered + uglified, case-by-case (ad hoc) lawmaking of many kinds; scooters left in rivers + over fences, lasting only months|Same case|Documented case|Design end state: where it goes, how long it lasts, who cleans it up|
|Proposed fixes: restrict scooters to bicycle infrastructure; cap speed at 25 km/h; parking every 200 m|Same case|Proposals|—|
|Car at 50 km/h needs ~70 times urban space of cyclist / pedestrian|—|Approximate|—|

## Platform entry into a fragile context

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|In Sri Lanka in 2018 false rumor of 23,000 sterilization pills, then 18-second video, led to days of anti-Muslim mob violence spread through social platform|2018 newspaper investigation|Documented case|Before entering fragile context → staff local-language moderation|
|~25 local-language moderator openings unfilled; platform had no local office|Same case|Approximate count|Before entering fragile context → staff local-language moderation + open local presence|
|Officials asked platform for emergency contact; company pressed them to use in-product reporting tool instead; reports of inciting content came back marked not violating platform's standards|Same case|Documented case|Before entering fragile context → set up emergency escalation|
|~3 million users bypassed government's block of platform via VPN|Same case|Approximate|—|
|Violence = local in origin, platform acting as wind spreading it|Framing by government adviser|Framing|—|

## Ranking experiments

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Six-country ranking experiment (October-March) moved professional media into separate tab during surge of hate|2018 reports|Documented case|Treat ranking experiments as ethical experiments; review + monitor them|
|Same company's stock fell 4.5% within hours of announcing feed changes favoring users' long-term interests|—|↑|—|

Together six-country experiment + stock drop show ranking experiments' externalities + market pressure against humane changes.

## Dual-use devices

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Apple supplied anti-stalking safeguards for its AirTags (precise Bluetooth item trackers) only after launch, after they had become effective tools for stalking people|2022 technology-news analysis + manufacturer's 2022 update|Documented case|Ship anti-abuse safeguards for dual-use features on day one|
|Most rival item trackers still lack these anti-stalking safeguards|—|Most|Ship anti-abuse safeguards on day one|
|Consequences went unexamined even though this maker routinely puts privacy + security first|—|—|↑|

Detailed item-tracker timeline + harassment and stalking cases → [safety and abuse evidence](safety-and-abuse.md).

## Built infrastructure embodies values

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Low New York parkway overpasses widely read as having blocked buses, excluding poorer + Black beachgoers|Historical case recounted in biography|Widely read as; intent contested + unprovable, what got built = what matters|Artifacts embody values regardless of designers' intent|
|1950s Atlanta interstate explicitly plotted as racial boundary + produced only chronic traffic|Historical case in 2019 design-ethics book|Intent behind such infrastructure contested + unprovable; what got built = what matters|Make ethics routine design-process step|

## Single assumptions and resilience

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Colorado town's water system, assumed to draw on sealed aquifer + exempt from chlorination since 1974, contaminated in 2008|Historical case, told by designer, formerly public-health emergency planner|Documented case|Resilience = breadth of situations system covers|
|In 2008 contamination ~1,300 people (>14% of residents) fell ill, one died, twenty hospitalized|Same case|Approximate count|Do not build only for best-case conditions|
|System had no tolerance for its single assumption breaking|—|Mechanism|Do not build only for best-case conditions|

## Removing what quietly regulates
Removing apparent nuisance can collapse system built on it (ecological history).

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Wolves eliminated from Yellowstone by 1926 as threat to livestock + settlement|Ecological history|Documented case|Before removing step → ask what it quietly regulated|
|No wolves → nothing checked elk herds → their browsing stripped willow, aspen + cottonwood → beavers fell, banks eroded, water warmed as cover lost, fish + songbirds declined|Same case|↑|Before removing step → ask what it quietly regulated|
|Reintroducing wolves decades later began reversing this chain|Same case|↑|—|

- What looks like friction to system's owners sometimes holds rest of system together.
- Damage from removing regulating element shows up several orders of consequence out.

## Harm to users and excluded groups

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Location-based mobile game contributed to >100,000 traffic accidents|Study estimate cited in 2018 ethics article|Estimated; cited under guideline of not putting users in harm's way|After every "how might we" question → ask "at what cost"|
|Several US cities banned cashless restaurants for discriminating against older, low-income + minority customers|Historical case, late 2010s|Documented case; convenience marketed to one group excluded others|Before setting strategy → ask: worst case + on whom?|
|Adapter dongles = one computer maker's top-selling product at major retailer, 2016-2018 → top-selling dongles = symptom of fragile, non-interoperable system|Retail sales reports|Documented case|Favor open standards + interoperability as form of resilience|

## Verify the parables you use

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Legend of New College, Oxford, planting oaks centuries ahead to replace its dining hall's ceiling beams = myth|Historical correction|Documented correction|Verify the parables you use|
|College acquired relevant estate in 1441, seventy years after hall's construction; real beam replacement 1863-1865|Same correction|Documented|Keep stewardship lesson; drop false anecdote|
|College archivist called legend myth in 2008|↑|Documented|Verify the parables you use|
|Senior politician repeated legend publicly in 2013 + got corrected in press same day|↑|Documented|↑|

Legend as told (false), as timeline:

|When (per legend)|What happens|
|---|---|
|1379|College founded; oak grove planted as future timber for hall beams|
|Next 500 years|Each forester passes on single standing order: leave grove uncut until beams need it|
|1859|Replacement of beetle-ridden beams falls due. Junior fellow guesses land college owns in various parts of country may have big-enough trees, though nobody knows of any|
|Then|College forester reveals grove + says his predecessors had long waited for someone to ask|

## Support for foresight methods

|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Imagining outcome as having already occurred improves cause identification by ~30% = basis of premortem|Research cited in project-management guidance|Approximate|Run premortem before project kickoff; start w/ silent individual brainstorming|
|Futures wheel used in futures research since early 1970s to map first-, second- + third-order consequences; foundational references from 1972 + 1993|Method history|—|Score futures wheel's outer-ring consequences for likelihood + impact|
|Implications-wheel study of abrupt climate change found many effects rated both likely + strongly negative|Implications-wheel study|—|Monitor worst futures-wheel consequences as early-warning signals|

Premortem bounds: 30-60 minutes; targets ~10 prioritized risks; works even as 15-minute kickoff.

## Related
- ../principles/intentional.md: principle backed here.
- ../principles/resilient.md: principle backed here.
- ../principles/inclusive.md: principle backed here.
- ../methods/second-order-thinking.md: asks what happens at full adoption + on whom cost falls.
- ../methods/futures-wheel.md: steps for mapping change's consequences in rings.
- ../methods/premortem.md: steps for imagining failure before launch + working backwards.
- ../methods/four-quadrants-of-responsibility.md: grid of what gets built (pixel, product, ecosystem) vs whom it serves (one person, community, society).
- ../methods/cutting-to-essentials.md: usability side; simplifying design w/o losing function; pair w/ check on what removed step regulated.
- safety-and-abuse.md: detailed item-tracker timeline + harassment and stalking cases.
- filter-bubbles-and-polarization.md: ranking effects on belief + discourse.
- convenience-and-friction.md: what removing / adding friction does.
