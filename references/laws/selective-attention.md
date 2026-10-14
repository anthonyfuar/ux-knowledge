# Selective Attention

## In one line
Attention = scarce resource; cannot cover whole scene → goal relevance rations it: attention usually holds whatever bears on current aim; lets only part through, screens out rest. Matters whenever people must see something: critical info, alerts, state changes, real content near ads.
- Alias: Selective Attention Theory (umbrella name for classic models). Class: construct. Theme: Attention.
- Reaches furthest into: telling content from ads, signalling state changes, avoiding simultaneous changes.
- Design job = steering (people discard what seems off-task): needed content/control easy to reach by eye; spare people overload + stray pulls on focus.

## Applies when / does not apply when
|Cite Selective Attention when|Cite something else when|
|---|---|
|content looking like ad / sitting in ad zone skipped (banner blindness)|grid of look-alike cards hard to compare → Cognitive Load + Working Memory (not Selective Attention)|
|weakly cued / simultaneous changes unnoticed (change blindness)|user slips onto adjacent button → main frame = error prevention + spacing; Fitts's Law only supports it|
|information outside region user reads/acts in (tunnel vision)||
|control never found → Selective Attention + visibility-of-system-status heuristic; not Fitts's Law (assumes visible target)||
|screen holds many independent settings → Cognitive Load + Selective Attention + Chunking + progressive disclosure (per Tesler's Law, relocates complexity); not Choice Overload||

## Decision rules

### Keep real content out of the ad filter
- Real content: never ad-like styling, never in ad zones.
- Never give content ad dimensions.
- Separate content from ad regions; test anything important in top banners / right rails.
- Banner-blindness triggers to avoid:
  - Location: top banners + right rails on desktop; article top / screen bottom on mobile.
  - Ad-like styling: animation, boxed rectangles, colored backgrounds, heavy formatting, text inside image.
  - Nearness to real ads: proximity groups content w/ ads.
- One weak item can poison whole region → audit key content's neighbours.

### Place what must be seen
- Critical information → current task's focal area; avoid making users watch whole dashboard when one region holds answer.
- Key fact → inside reading path, next to related text.
- Critical alerts → current task's attention path.
- Escape actions → near task.
- Peripheral content only weakly processed → never depend on it for critical messages.
- If alert must reach users from periphery → their own name, own data / goal words.
- If users must notice alert outside their focus → change physical property (sound, motion onset, position, color), not only wording.
- Relevant items physically distinct → pass early filter; indicators distinct in shape.
- Where selection happens unresolved (early vs late; 1963 model) → design for both physical + semantic salience.
- Targets look as users expect (same label, icon, color); styling consistent.
- Critical negative information → hard to miss but not alarming; say what user can do about it; never assume shown = read. Overly strong warnings → avoidance, not action.

### Signal changes
- Important changes → strong cues, shown one at a time.
- Collision = simultaneous updates stealing notice from each other → trace every one across design.
- Page loads + transitions act like flicker-experiment blank → each change where user acted, strongly signalled, one at a time.
- Stagger sounds, notifications + animations; relevant one nearest task; limit how many run at once.
- Long monitoring tasks need strong, well-timed cues (lesson of 1950 vigilance research).

### Control load + clutter
- Simple screen → clutter costs attention → remove it. High-load screen → essentials in periphery not seen.
- Never make users hold codes / earlier choices in mind while ignoring on-screen noise.
- Avoid giving users several deliberate monitoring tasks at once.
- Remove irrelevant attention-grabbing motion, badges + alarm colours from task-critical screens.
- Competing elements draw from one attention pool (1973 capacity model) → remove competitors.

### Expect filtering + test for it
- People follow one voice + tune out others (1953 experimental study) → expect users to lock onto goal-relevant signals, filter out rest.
- Test attention-dependent designs w/ both novices + experts.
- Judge salience w/ real users, not from designer's own view.

### Emphasis in quick decisions
- Emphasis in quick decisions effectively acts as default → use for user's goal.

## Why it works

### Core mechanism
- Attention = bottleneck / limited resource; filtering possibly early, attenuated or late; what passes mostly goal-relevant.
- Attention limited in both duration + capacity.
- Learned expectations (e.g. "that area is ads") drive what gets filtered.
- Noticing depends on person's goal as much as on prominence.
- Expertise changes filtering: novices filter more rigidly than practiced users.
- Inhibition-deficit hypothesis: older adults filter out irrelevant input less well → clutter fills their working memory; distractors cost them more.

### Models at a glance
|Model (year)|Claim|Design use|
|---|---|---|
|Spotlight view (1890)|attention = spotlight: sharp focus, visible but unclear fringe, unattended margin|critical info in focus, not fringe|
|Filter Theory (1958)|early selection: physical properties decide what passes, meaning extracted only afterwards; narrow passage → small throughput; historically first complete model|relevant items physically distinct|
|Attenuation Model (1960)|revision of Filter Theory: part of ignored input still processed: filter dims it rather than cutting it off; personally / biologically important words (own name, "fire") need little signal strength to break through; context primes related words → easier breakthrough|personal + goal words reach periphery|
|Late Selection Theory (1963)|selection last, after every input's meaning worked out; pertinence = importance to current goal|design for semantic as well as physical salience|
|Capacity model (1973)|tasks draw on one finite attention supply that can be split among them|remove competing elements|
|Zoom-lens model (1986)|focus widens/narrows; wider focus spreads same resources thinner → slower processing|avoid making users watch whole screen|
|Perceptual load theory (1995)|filter's locus depends on main-task demand; easy task → spare capacity spills automatically onto nearby distractors, processed for meaning; demanding task → all capacity used, side content never registers; load = task-relevant demand, not visual busyness|declutter simple screens; keep essentials out of periphery on demanding ones|
|Memory-selection models|attended + unattended input both pass initial filter, sorted by meaning at second stage → explains why own name breaks through||
|Working-memory bottleneck account|real bottleneck = deliberate steering of attention, one action at a time|avoid several deliberate monitoring tasks at once|
|Three-level working-memory framework (2003–2018)|working memory = attention directed to memory; focus holds ~one item + shifts in ~300 ms; bottleneck = controlling attention, not attending||
|Ecological view|attention = orienting toward person's goals in environment, not symptom of brain limits||

Selection gets harder when: source distant (nearby easier); streams separated only by channel + fully overlapping in time; each extra competing stream added. Distinct pitch helps stream get selected.

### Named failure modes
|Failure|What happens|Why|
|---|---|---|
|Banner blindness|content unread when placed where ads usually sit, near ad, or looking like ad, on mobile + desktop|learned "that area is ads" expectation|
|Hot-potato pattern (2018)|after one irrelevant fixation users write off fixated region on page, whole site + even other sites|one bad look poisons region|
|Change blindness|w/ faint cue even major change slips past|faint change cues + attention limits; worse when several changes at once; weakly cued changes fall outside attended subset of scene|
|Lost motion cue|real-world change usually comes w/ motion; peripheral vision catches it + steers eyes to it; change during flicker, page load, blink or rapid eye movement loses this cue → finding it needs item-by-item before-and-after comparison from poor memory||
|Masking|two simultaneous changes hide each other: first captures eye, eye movement masks second||
|Tunnel vision|users lock onto region they work in / believe holds answer, rarely scan outside it; large type or prominent corner position does not pull eye out|designers misjudge it: they already know item's location|
|Inattentional blindness|focused attention can blind people to conspicuous stimuli + leave them unaware they missed them||
|Ostrich effect|people skip information they would rather not see (account balances, security warnings)||

### Origin
- Selective attention theory built from mid-20th century, driven by both theory + applied problems (e.g. operator vigilance); neuroscience + cognitive psychology still build on those early models.
- 1953: dichotic listening studies on how listener shuts out all other sound sources, stays w/ one; named cocktail party phenomenon.
- 1950: World War II unease about how well radar operators did their job → vigilance research.
- 1950s to 1970s: listening tasks, once dominant attention-study method, gave way to mostly sight-based tasks.
- Perceptual load theory recast early-vs-late selection debate as question of load: distractors processed only if main task leaves spare capacity.

## Evidence

### Listening studies
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Listeners repeating message in one ear could report almost nothing of other ear's content|1953 dichotic listening experiments|later word-list + melody studies agreed|expect goal-locked filtering|
|Few noticed when ignored message switched from English to German or to backward speech; all noticed switch from male to female voice or to 400-Hz tone|1953 dichotic listening experiments|physical changes break through ignored input, meaning changes do not|change physical property to get noticed|
|Bottleneck passes only limited information|Filter Theory, 1958|theoretical model|physically distinct relevant items|
|Own name noticed in unattended ear on ~33% of trials|1959 dichotic listening experiment||own name / own data in alerts|
|87% target detection in attended ear vs 8% in ignored ear|1967 dichotic listening experiment||do not rely on unattended channels|
|76% detection in attended ear vs 33% in ignored ear, when told to stop at any target|1969 dichotic listening experiment|||
|Highly practiced shadowers detected 67% of digits in ignored channel vs 8% for naive listeners|1974 dichotic listening experiments|expertise changes filtering|test w/ novices + experts|

### Load + search
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Peripheral distractor slowed letter search when other positions empty (low load), not when they held non-target letters (high load)|1995 lab experiment||load decides what distracts|
|Even personally interesting distractors (cartoon characters) stopped distracting under high perceptual load|2007 experiment|||
|Visual cortex responded less to distractors under high load|2005 imaging study|||
|Two kinds of load pull opposite ways: full working memory → more distractible; full perceptual load → less distractible|2016 review of two decades of research|review|never load memory while users must ignore noise|
|People search w/ mental template of target; template matches capture attention even when harmful|2008 research||targets look as users expect|
|When targets + distractors stay consistent, attention guidance moves into long-term memory + becomes automatic|1977 research||keep styling consistent|

### Banner blindness
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Content in ad slot ignored whether placed there on purpose or not|first documented in 1997 usability testing; replicated by large 2007 eyetracking study; still common in 2018 eyetracking study (eyetracking studies 1997–2018)|long-running replication|separate content from ad regions|
|User looking up hikes made 148 fixations: 132 on content area, 1 on right rail → rail got 0.8% of attention while taking 25% of content area (~33 times less than size predicts), though holding relevant content|2018 eyetracking study|one user's session|test anything important in right rails|
|26 participants skipped in-text promotion styled as formatted blue rectangle|2018 eyetracking study||no ad-like boxes for content|

### Change blindness
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Scene shown ~half a second, brief blank, scene w/ one detail altered; many people needed 20 or 40 alternations to find change, even when warned|mid-1990s flicker experiments||page loads act like flicker blank|
|In flicker paradigm, changes w/o motion cue missed even w/ warning|2002 + 2005 reviews|reviews|signal changes strongly, one at a time|

### Field observations
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Case: participant searching company-history timeline missed year in large type at top left of each pop-up + found it only in last line of body text she read|2012 usability test|one observed participant: illustration, not effect size|key fact in reading path|
|Optional Skip link far from main actions missed → users believed sign-in required|mobile usability session|qualitative; no sample size|escape actions near task|
|Hint about detail view in far corner missed → users thought episode list unreachable|TV app usability session|qualitative; no sample size|hints near trigger|
|Several participants missed how-to video sized like surrounding display ads|instructional-video study|qualitative; no sample size|never give content ad dimensions|
|Distinct list-indicator shapes → faster, more accurate finding; near-identical shapes slowed scanning|earlier research on list indicators||indicators distinct in shape|

### Choice
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|At fast decision speeds visual salience swayed choice more than preference, most of all when brand preference weak|2012 consumer choice experiment||in fast choices salience = default|

## Misreadings and limits
- Wrong: add working-memory demands to make users "focus" (Selective Attention, Cognitive Load) → Right: loaded working memory increases distraction.
- Wrong: bigger, bolder or differently styled element gets noticed (Selective Attention, Von Restorff Effect) → Right: outside user's focus region / w/ ad-like styling often ignored; put it in reading path.
- Wrong: judge salience from designer's own view → Right: designers already know where to look + what changes; test w/ real users.
- Wrong: ship several changes at once → Right: they compete + go unnoticed.
- Wrong: cite Fitts's Law for control never found (Save at bottom of long scroll, off-screen action) → Right: it assumes visible, located target + predicts movement time only; cite Selective Attention + visibility-of-system-status heuristic.
- Wrong: frame slips onto adjacent button as Fitts's Law → Right: main frame = error prevention + spacing; Fitts's Law only supports it.
- Wrong: cite Choice Overload for screen of many independent settings → Right: it needs one choice among close substitutes; sixty separate toggles = scanning + finding load.
- Wrong: present one attention model as settled → Right: models disagree on where filtering happens (early on physical features, attenuated, or late on meaning); no single model explains all of attention; cite each for part it explains.
- Wrong: treat resource (capacity) theories as precise → Right: criticized as broad + vague.
- Wrong: treat 2012 timeline case as effect size → Right: one observed participant = illustration.
- Limit: distinctiveness works only when rare; overuse cancels itself + users may mistake salient blocks for ads.
- Limit: even two animations in different screen areas can overstimulate; overused salience tools become noise.
- Limit: overload defeats attempts to guide attention; concurrent changes can each go unnoticed.
- Limit: large type / corner position does not pull eye out of locked-on region.
- Limit: overly strong warnings → avoidance, not action.
- Dating caveat for one body of decision research: cognitive-bias work 1972 + 1974; attention capacity model 1973; prospect theory 1979; framing 1981; peak-end work 1993, 1996 + 2003; experiencing vs remembering self 2005; 2011 book using System 1 / System 2 labels coined earlier by others → match year to specific claim.

## Check questions
- (Tunnel vision, change blindness) Critical information inside region user reads/acts in? Look for: key facts in corner labels, sidebars or headers off reading path; new UI appearing far from its trigger.
- (Banner blindness, faux ads + Von Restorff Effect) Real content avoids ad styling + ad zones at every screen size? Look for: content beside ads, in banner slots or banner-shaped; boxed, colored or animated sections; contrasting blocks on mobile.
- (Change blindness) Important changes noticed? Look for: weak change cues; several simultaneous competing updates.
- Measurable form: compare each region's eyetracking-fixation share w/ its screen-area share; far fewer fixations than space share = region filtered, whatever it holds.
- Design tested w/ novices + experts, not judged from designer's view?

## Symptoms → fixes
|Symptom|Likely cause (laws)|Fix|
|---|---|---|
|Important update, prominent element or new control goes unseen|Selective Attention: tunnel vision, change blindness|strong cue in reading path / beside control in use; one change at a time|
|Promotion, emphasized element or real content skipped as ad|Selective Attention: banner blindness; Von Restorff Effect|styling consistent w/ surroundings; no ad styling or ad slots; test on mobile|
|Key control below the fold / off-screen never found, e.g. Save at long page's end|Selective Attention: tunnel vision + visibility-of-system-status heuristic; not Fitts's Law (assumes visible target)|sticky save bar once something changes, or auto-save w/ visible saved state; warn on leaving w/ unsaved changes|
|Field errors fire while user typing, or valid fields get noisy checkmarks|Selective Attention: interruption; Cognitive Load; error-prevention heuristic|validate when user leaves field or submits; once error shows, recheck live so it clears; keep valid fields quiet; focus first error / linked summary|
|Grid of look-alike cards hard to compare|Cognitive Load + Working Memory (comparing across cards); not Similarity (uniform cards correctly read as one content type); not Selective Attention|show deciding attributes (price, rating, key spec) consistently; add sorting + filters|

## Hypothetical examples
- Hypothetical (reading path): pharmacy refill page states pickup deadline in sentence user reads, not in header label off to side.
- Hypothetical (change near action): banking app updating balance after transfer shows change beside just-tapped button, not in top summary bar.
- Hypothetical (ad zone): city council site keeps service-outage notice in main content column, not in right rail beside sponsor banners.

## Humane bound
- Turned against people when attention taken against their interest, e.g. instant interruption: everything buzzes on arrival since interrupting pays sender better than waiting; other attention hijacks belong here too.
- In fast choices salience acts as default (2012 consumer choice experiment: salience swayed choice more than preference at speed).
- Disguised ads turn people's inattention into agreement.
- Bound by Respectful + Transparent: ads must read unmistakably as ads.
- Further reading for this bound: attention hijacks + their counters; notifications + interruptions; evidence on attention + distraction.

## Related
- von-restorff-effect.md: closely related; shares ad-styling review question, skipped-as-ad symptom + assumed-noticed misreading.
- cognitive-load.md: shares field-error symptom + working-memory-demands misreading; w/ Working Memory, law for look-alike card grids.
- working-memory.md: full working memory → people more distractible; w/ Cognitive Load, law for comparing across look-alike cards.
- chunking.md: one law to cite for screen of many independent settings.
- teslers-law.md: progressive disclosure relocates complexity on settings-heavy screens.
- ../checklists/usability-heuristics-map.md: holds visibility-of-system-status + error-prevention heuristics named in symptoms.
- ../patterns/notifications-and-interruptions.md: humane bounds on what interrupts, when, on what channel + under whose control.
- ../ethics/attention-hijacks.md: levers taking attention against person's interest + counter to each.
- ../evidence/attention-and-distraction.md: humane-design evidence on interruption cost, phone checking + notification load.
- ../principles/respectful.md: principle bounding Selective Attention.
- ../principles/transparent.md: ads must read unmistakably as ads.
- ../guides/laws-and-principles-crosswalk.md: names humane principle bounding Selective Attention.
- ../patterns/calls-to-action-and-touch-targets.md: applies Selective Attention.
- ../patterns/search-and-results.md: applies Selective Attention.
- ../patterns/layout-grouping-and-hierarchy.md: applies Selective Attention.
- ../patterns/dashboards-and-data-displays.md: applies Selective Attention.
- ../patterns/feedback-loading-and-performance.md: applies Selective Attention.
- ../patterns/complexity-management.md: applies Selective Attention.
- ../patterns/calm-technology-and-device-etiquette.md: applies Selective Attention.
