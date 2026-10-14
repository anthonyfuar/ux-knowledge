# Safety and abuse resistance

## Use when
- Covers: misuse cases + abuser personas, tracking + dual-use safeguards, blocking, reporting, moderation + enforcement, identity exposure, contributor edits reaching physical world, protecting children + users of well-being + health products.
- Open when designing/reviewing any feature letting people see, reach, locate, track, report or sanction one another, or one minors / vulnerable people use or could use.
- Principles served: Resilient, Inclusive, Intentional, Empowering, Transparent, Respectful. Resilient served by most entries.

## Stance
- Abusability = successor concern to usability.
- If feature's abuse possible → assume it will happen.
- Most common attacker = not stranger but current / former partner sharing home, devices + passcodes.

## Before launch

### How will this feature be used to hurt someone? (misuse cases + abuser personas next to use cases)
- When: every feature, before launch.
- Do: each user story gets mirrored story of someone using feature to hurt another. Personas for people intending harm. Design misuse mitigations before shipping.
- Avoid: responding to abuse only when press notices. Excuse "we never imagined misuse".
- Why: Resilient.
- Case: email client's read receipts leaked recipients' location, w/ no way to opt out.
- Evidence → case: research in India: women avoided uploading profile photos for fear of stalking. After research, profile-photo guard added; guarded pictures copied about 75% less.

### Whose scenario founds the feature? (vulnerable-centred happy path)
- When: writing feature's founding scenario.
- Do: centre founding scenario on person most at risk + most likely misuse → recovery path built together w/ primary flow.
- Avoid: MVP built on frictionless scenario, edge cases deferred to "later" never coming.
- Why: Resilient.
- Hypothetical: founding scenario for shared family calendar = controlling partner reads user's future whereabouts; user can hide entries from this one person.
- Hypothetical: ride-share's trip-sharing feature ships "stop sharing my trip" control in same release as sharing itself.

### A harm is called an edge case: how to weigh it? (count people, not percentages)
- When: harm dismissed as edge case.
- Do: state absolute number of people affected, not only percentage. Never ship to test cohort anything you would not leave in permanently.
- Avoid: "it's only 1%" or "it's just an MVP" as conversation enders.
- Why: Resilient. Some argue reaching for edge-case label reveals whose problems team decided not to count.
- Hypothetical: ride-hailing safety review restates "a fraction of a percent of trips" as rider headcount behind it.
- Hypothetical: patient-portal team, told login fault hits "only a few users", looks up how many patients affected before deciding it can wait.

## After launch

### Who keeps watching once it ships? (keep watching + budget for failure from day one)
- When: whenever feature ships.
- Do: assume something will turn out wrong. Instrument abuse signals, e.g. unanswered first messages followed by blocks, moderation false positives, safety surveys. Name safeguards steward surviving team turnover. From product's first day, hold means ready for day it breaks down / does harm.
- Avoid: post-launch ownership limited to bug triage. Safeguards no one owns.
- Why: Resilient.
- Hypothetical: smart-doorbell maker's launch plan names safeguards steward + budgets for day someone misuses camera, before first unit ships.

## Tracking + dual-use

### Who could turn this tracking capability on someone? (threat-model the intimate partner)
- When: any capability able to track, locate, monitor / record.
- Do: model attacker w/ passcode, shared accounts + physical device access. List whoever could turn capability on someone: stalkers, employers, abusers, governments, neighbours. Ship detection, alerts + disablement at launch.
- Avoid: safeguards designed only against strangers. Alert pause anyone holding phone can set indefinitely.
- Why: Resilient.
- Case: item tracker planted by cohabiting spouse never registered as separated from owner → no alert fired. Victim's alerts could be paused from her own phone.

### How fast does the affected person learn of the harm? (shrink the harm window w/o alert fatigue)
- When: wherever safety alerts exist.
- Do: minimize time from harm start to affected person told, w/o causing alert fatigue. Distinguish device "moving with you" from one merely "near you". Explain alert's benign triggers. Alerts work across platforms, w/o smartphone + for people w/o hearing: combine sound, vibration + on-screen alerts.
- Avoid: alerts reaching only one phone ecosystem.
- Why: Resilient.
- Cases (anti-patterns seen in tracker alerts): 60-decibel chirp lost in traffic. Sound alerts only after 17 hours + phone alerts only after > 24 hours, delay reduced from original 72.
- Hypothetical: car-sharing app tells account holder by push + text message as soon as second phone pairs to car's digital key; app notes family member pairing can also trigger it.

### Can the targeted person stop it quietly? (discreet stop + report)
- When: someone discovers tracking / targeting aimed at them.
- Do: tracked person can stop device's reporting + file report w/o confronting perpetrator. Require periodic reconfirmation of any "borrowed" or "paused" tracking-device state.
- Avoid: assuming alerted person free to act openly or remove battery in abuser's view.
- Why: Empowering.
- Hypothetical: family location app lets teen quietly stop sharing location w/ one relative + report to service, w/o any notice reaching that relative.

### What does setup say about misuse? (warn at setup + keep an accountability trail)
- When: dual-use device / feature first activated.
- Do: at setup, state purpose + warn: tracking another person w/o their agreement illegal in many jurisdictions; device built to be found; service can release owner's identity to law enforcement. Accountability trail: each unit tied to serial number + account.
- Avoid: marketing dual-use device's convenience while silent about misuse.
- Why: Transparent.
- Case: parents hiding trackers in their child's car did not perceive it as stalking until told.

## Self-protection, reporting + enforcement

### What do blocking, muting + restricting actually do? (specify self-protection tools)
- When: shipping any self-protection tool.
- Do: document, for each direction, what blocked person can still see, send or infer. Audience + commenters restrictable independently. Decide deliberately whether users can block moderators. Check whether people can game blocking.
- Avoid: "block" w/ undocumented visibility effect. Limiting victim's own speech as only remedy.
- Why: Resilient.
- Hypothetical: professional-networking site's block page states, per direction, what blocked person can still see (e.g. posts in shared group) + what they can no longer send.

### What happens after someone presses report? (full reporting loop, incl. appeal)
- When: wherever report button exists.
- Do:
  1. Acknowledge receipt.
  2. Explain interim tools reporter can use meanwhile.
  3. Communicate decision.
  4. Allow appeal.
  5. Staff review queue.
  6. Check no one can weaponize reporting itself.
- Avoid: report form dropping into void. Replying "does not violate our standards" while rumours turn into mob violence.
- Why: Resilient.
- Hypothetical: tenants' forum report screen tells reporter they can mute poster while waiting; later shows decision w/ appeal button.

### Who reviews, and how are they protected? (staff the review queue as part of the product)
- When: any report, appeal or moderation decision reaches human reviewer.
- Do: budget queue as permanent cost of shipping feature. Enough reviewers for volume feature generates, in languages audience speaks. Reviewer terms secure enough they can say work harms them. Protect reviewers w/:
  - rotation off graphic queues
  - muted + blurred previews by default
  - ceiling on exposure per shift
  - counselling needing no disclosure to manager
  - way to escalate case, not absorb it alone
- Avoid: response time resting on small contracted team paid least market allows. Treating review's psychological cost as somebody else's expense line.
- Why: Resilient (also Inclusive).
- Hypothetical: city-services app adding photo uploads hires reviewers speaking city's main languages; gives them blurred previews + rotation off graphic queues.

### How to sanction someone? (enforce quickly, w/ specific explanations)
- When: sanctioning someone.
- Do: publish community standards + their consequences. Secure executive backing for enforcement. Tell sanctioned person promptly + precisely what behaviour triggered sanction.
- Avoid: vague / absent enforcement.
- Why: Resilient.
- Case: game studio's automated ban notices, sent within minutes + quoting offending chat log, cut reoffending within three months to under 8%.

## Beyond the visible surface

### Where does the harm go once it leaves view? (follow it into closed channels)
- When: open surface can push people into groups, direct messages / another product where you see nothing.
- Do: cap how far uncorroborated claim travels before reaching closed channels. Slow forwarding inside closed groups. Member can report group content from inside group w/o exposing reporter. Count harm organized outside your logs as your product's effect, not someone else's.
- Avoid: safety measurement stopping at what moderation queue sees. Treating public-post coverage as whole-system coverage.
- Why: Resilient. Public surface = recruiting stage; private one = where coordination lands.
- Case: calls to gather spread on open feed, then moved into private groups where participants agreed targets + timing.

### Entering a market where the platform will be the internet: what first? (assess institutional fragility)
- When: entering market where your platform will become synonymous w/ internet.
- Do: before expanding, evaluate local media, courts + police. Hire local-language moderators in proportion to reach. Open local presence. Establish emergency escalation w/ officials + civil society. Ranking experiments there → ethical review.
- Avoid: refusing officials emergency contact because report button exists.
- Why: Intentional.
- Cases (fragile market): roughly 25 local-language moderator roles unfilled while violence spread. 18-second rumour video followed by days of mob attacks, while reports about it came back as not violating standards.

### Hate groups stay within the letter of policy: act? (safety over speech; values, not only policy)
- When: hate groups operate within letter of acceptable-use policy.
- Ask: what question team answers: people free to say things here, or everyone safe to exist here? Ask whether everyone safe to exist on platform, not merely free to speak.
- Do: remove groups based on stated values, not only policy's letter. Small concerns from most endangered people = leading indicators.
- Avoid: "they didn't break our rules" as reason to host organized hate. Requiring proof in large numbers before safety concern counts.
- Objection "a company cannot censor" → answer: company's rules = not constitution. Legal speech protections restrain governments, not private companies. Acceptable-use policy = choices some people wrote down + can rewrite this afternoon.
- Why: Inclusive. Every day hate group stays = decision to keep hosting it. Declining to decide produces outcome like any other decision.
- Case: workplace-chat company removed 28 hate groups technically not in violation of its policy.

## Identity exposure

### What could one user gather about another? (audit the doxxing surface)
- When: people can see data about each other.
- Do: inventory what others can gather + combine to identify / locate someone. For each data field, ask whether you need it. Revisit inventory on schedule, together w/ security.
- Avoid: collecting everything in case it turns out useful.
- Why: Respectful.
- Case: global activity heatmaps revealed military bases' layouts.
- Hypothetical: school-parents' chat app lists every field one parent can see about another (child's class, pickup times, phone number) + drops pickup times as not needed.

### What name must people show? (no forced legal name in public view)
- When: deciding what people must display, verify or keep consistent across service.
- Do: separate name shown to others from any name held for legal / payment reasons. Displayed name changeable w/o losing history, contacts or account. Former names, merged profiles + linked accounts kept out of search + suggestions.
- Avoid: authenticity policy enforced via user reports → hands unmasking tool to whoever wants somebody unmasked. Profile surfacing every previous name.
- Why: Resilient (also Inclusive). Legal-name requirement = fastest route back to someone relocated to escape abuser; exposes trans people, people known by another name at work, performers, people whose speech endangers them where they live.
- Hypothetical: after member changes display name in choir's scheduling app, old name drops out of member search + mention suggestions while rehearsal history stays.

## Edits that reach the physical world

### Contributors can change data that moves people or money: how to govern them?
- When: unpaid / lightly vetted contributors can change data moving people, vehicles, deliveries or money, e.g. road classification + geometry, place records, opening hours, capacity, safety flags.
- Do: require training / test for edit classes carrying physical risk. Each contributor accountable to operator under stable identity, even where public sees only handle. Queue high-impact edits for someone qualified before they reach anyone. Those living w/ result (residents, local businesses, authority responsible for street) get route to contest edit; route outranks contributor status, not sits beneath it.
- Avoid: contribution ladder where rank earned by edit volume settles safety disputes. Overruling someone whose own street affected + labelling them bad actor for correcting it. Contributor anonymity existing mainly to blunt liability.
- Why: Resilient (also Intentional).
- Hypothetical: volunteer-maintained accessibility map requires short test before anyone can mark station entrance step-free + ties each such edit to contributor's account, though public sees only handle.

## Children + health

### Minors use or could use the product: which defaults? (protect children from persuasive design)
- When: minors use or could use product.
- Do: detect / declare age + apply stricter defaults for minors:

|Default for minors|Setting|
|---|---|
|Late-night push notifications|none|
|Autoplay|off|
|Break reminders|on|
|Recommendations|tighter limits|
|Sharing|private by default|
|Social-rejection triggers|none|
|Data collection|minimal|

  - Family controls: downtime, always-allowed contacts, exception requests, guaranteed emergency calling.
- Avoid: identical engagement settings for 13-year-old + 40-year-old.
- Why: Resilient.
- Case (anti-pattern seen in practice): internal tooling flagging insecure teens for advertisers.
- Hypothetical: game console's child profile starts w/ late-night notifications off, sharing private + data collection limited to what play needs.

### Product touches mental or physical health: what changes? (well-being + health = sensitive category)
- When: product touches mental health, mood, meditation, fitness, sleep, food, recovery or medical condition.
- Do:
  - All records = health information, incl. engagement traces: mood entries, session times, skipped days + use lapses all describe someone's state.
  - Records on device where possible; wholly out of advertising + general analytics; exportable + deletable from one place. Never used to time re-engagement.
  - Assume some of audience has obsessive-compulsive traits, scrupulosity, eating disorder or health anxiety → for them counter, target or broken run acts as symptom, not motivation.
  - Every tracked number optional, adjustable + switchable off w/o losing product. No rankings of people against each other.
- Avoid: calm surface over anxiety engine. Mood logs in same pipeline as product analytics. Win-back push built on somebody's low-mood history. Well-being marketing claim product's mechanics contradict.
- Why: Resilient (also Inclusive).
- Hypothetical: food-diary app sends no win-back message after lapse, keeps entries out of product analytics + lets each person export / delete them all from one settings page.

## Related
- ../methods/misuse-case-brainstorming.md: lists how someone could use feature to harm.
- [Safety and abuse evidence](../evidence/safety-and-abuse.md): harassment, stalking + intimate-partner abuse through products.
- [Children and adolescents evidence](../evidence/children-and-adolescents.md): effects on minors + age-appropriate design.
- ../principles/resilient.md: principle most entries here serve.
- privacy-data-and-security.md: data minimisation, consent, access + deletion, for doxxing surface + health records.
- habits-streaks-and-gamification.md: streaks, counters, rewards + their effect on vulnerable people.
- friction-undo-and-confirmation.md: speed bumps on sharing + forwarding, step-up authentication.
- errors-and-input-tolerance.md: usability side of edge cases, error prevention + recovery.
- ../principles/inclusive.md · ../principles/intentional.md · ../principles/empowering.md · ../principles/transparent.md · ../principles/respectful.md: other principles these entries serve.
