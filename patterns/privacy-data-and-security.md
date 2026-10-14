# Privacy, data and security

## Scope + principles behind these patterns
- Use for: humane patterns on data minimisation · consent · terms · access + deletion · purpose limits · expiry · de-identification · tracking · advertising · security · always-on collection.
- Applies when: designing/reviewing any field or permission request, sign-up, legal text, stored personal data, data pipeline, data release, third-party tracker, ad model or sensing device.
- Principles underneath:
  - ../principles/transparent.md: underlies privacy patterns; most of them serve it.
  - ../principles/respectful.md: data as part of person, asking only what task needs, advertising w/o granular tracking.
  - ../principles/resilient.md: real-world privacy rule, later decisions, re-identification.
  - ../principles/intentional.md: questioning ambient, always-on collection.

## Data minimisation + consent

### Any collection, retention or sharing decision: whose data is it?
- When: any collection, retention or sharing decision.
- Do: govern personal data as if part of person's body + mind. People own their personal data. Surveilling person = violation. Existing human-rights protections apply to personal data.
- Avoid: "data is the new oil" framing: treats people as resource to extract.
- Why: Respectful (data as part of person).
- Hypothetical: fertility-tracking app writes data rules as if handling user's own body: she owns every entry, nothing beyond what she logs watched, + entries get clinic-record protection.

### Field or permission request: what to ask + how?
- When: any field or permission request.
- Do: state feature needing data beside request; drop any field you cannot justify in one sentence; sensitive questions optional w/ "prefer not to say"; non-binary gender options.
- Avoid: implying permission mandatory when feature works w/o it.
- Why: Respectful (ask only what task needs + say why).
- Hypothetical: library e-book app asks date of birth + home phone to borrow e-book, though lending works w/o either → drop both, or name feature needing each.
- Hypothetical: pharmacy app's location request says "to show the nearest open branch"; declining still lets person type postcode.

### Sign-up: what must the person know before committing?
- When: sign-up.
- Do: before account exists, itemise in plain, concrete terms each commitment person makes + each kind of data collected.
- Avoid: vague terms behind single "I agree" checkbox.
- Why: Transparent (right to know before commitment).
- Hypothetical: gym sign-up shows beside plan choice, before any account exists, plain list: minimum term, cancellation notice, + data kept (check-in times, payment details).

### Legal text required: how to present it?
- When: legal text required.
- Do: two layers: plain-language summary (short sentences, everyday words) beside full legal version; surface relevant terms fragment at decision moment.
- Avoid: thirty pages of tiny type lulling people into clicking agree; price rises hidden in FAQ.
- Why: Transparent.
- Hypothetical: car-rental checkout shows fuel + damage clauses in plain words right beside "add cover?" choice, w/ link to full contract.

### First use, or identity not truly needed: require an account?
- When: first use, or products not truly needing identity.
- Do: people try product w/o profile or social login; no account for appliances.
- Avoid: kitchen device demanding social sign-in.
- Why: Transparent (anonymous mode, no forced accounts).
- Hypothetical: symptom-checker app runs fully w/o account → people can judge it before tying it to their name.

## Access, deletion + limits on later use

### Stored personal data: can people see, fix, export + delete it?
- When: any stored personal data.
- Do: labelled "your data" section to view, correct, export + permanently delete. Deletion = deletion, not deactivation.
- Avoid: data access only via legal request form; deletion only by emailing support.
- Why: Transparent.
- Case: on one job site, users could not find account deletion for four years.
- Hypothetical: language-school portal's "your data" tab: student fixes misspelt name, downloads attendance records + erases account fully, not merely hides it.

### Data given for one purpose: reuse it for another?
- When: data given for one purpose (security, learning, health) could serve another.
- Do: data stays bound to purpose given for; announce any new use before it happens + default it off.
- Avoid: repurposing data behind person's back.
- Why: Transparent.
- Case: phone numbers collected for two-factor authentication then used for contact discovery.
- Hypothetical: badge swipes collected for building security start feeding staff productivity dashboard w/o notice = repurposing behind people's backs.
- Hypothetical: driving-lesson app posts learners' practice routes on public leaderboard, though routes given only to plan lessons = data exposed for another use.
- Hypothetical: email given to clinic for appointment reminders never joins its newsletter list unless patient opts in.

### Details shared for a bounded event: how long do they stay shared?
- When: someone shares details for bounded event: meeting, trip, delivery, shift, repair visit.
- Do: scope sharing to occasion + let it lapse by itself. Where architecture allows → data stays w/ person; service gets only what task needs, only while task lasts. Extending sharing window = deliberate act, not default.
- Avoid: one-time disclosure treated as standing grant.
- Why: Transparent + Respectful. One-time disclosure turned standing grant → detail offered for one afternoon stays visible + searchable for years.
- Hypothetical: home-repair app shares customer's address + gate code w/ technician only for booked visit; access closes when job marked done, w/ explicit "keep for future visits" option.

### Designing a data pipeline: keep insight or identity?
- When: designing data pipelines.
- Do: extract insight service needs from consented data, minimising identifier retention; sensitive analysis (voice tone, sleep, ambient audio) on device + purgeable.
- Avoid: hoarding raw personal data because it might prove valuable someday; cloud-stored ambient recordings w/ vague sharing rules.
- Why: Transparent (insight, not identity).
- Hypothetical: call-centre quality tool derives resolved/not-resolved tag per call, then deletes source recordings + caller numbers.

### Behavioural, location, health or inferred data: what could it decide later?
- When: collecting behavioural, location, health or inferred data for tailoring or convenience.
- Steps:
  1. Write out consequential decisions same record could feed if it left current setting: insurance price, loan or tenancy approval, employer's conclusions about risk.
  2. Set granularity, retention + sharing against list above, not against feature data powers today.
- Avoid: judging data practice only by current use.
- Misreading: Wrong: "we would never use it that way" substitutes for not holding data → Right: later owner, later policy or lawful demand decides use, not present team.
- Why: Transparent + Resilient.
- Hypothetical: smart-thermostat team notes hour-by-hour occupancy could later tell landlord when tenant away → keeps only daily energy totals.

### Releasing data w/ identifying columns removed: is it anonymous?
- When: personal data published, handed to partner, released for research or sold as aggregate after identifying columns removed.
- Steps:
  1. Before release, decide what could plausibly be joined to data.
  2. Coarsen/bucket fields carrying most uniqueness.
  3. Suppress small counts or add noise to them.
  4. Bind recipients by contract to attempt no re-identification.
- Avoid: releasing event/location history at full precision only because name column dropped.
- Misreading: Wrong: promising anonymity when data only pseudonymous → Right: de-identification = risk reduction, not guarantee; assume someone can trace de-identified data back.
- Why: Transparent + Resilient. A few ordinary attributes (dates, postcode, timestamps, movement trail, rare mix of preferences) usually single out individual once joined to what recipient already holds.
- Hypothetical: hospital releasing appointment data to partner: exact birth dates → age bands, postcodes → regions, + blanks any cell w/ very few patients.

## Tracking, surveillance + security

### Third-party script, pixel or SDK present: audit?
- When: any third-party script, pixel or SDK present.
- Steps:
  1. Scan for ad trackers, third-party cookies, fingerprinting, session recording, keystroke capture before submit, platform pixels.
  2. Remove trackers you cannot justify; disclose remaining ones.
- Avoid: adding analytics + social widgets w/o inventory.
- Why: Transparent (audit your own trackers).
- Case: more than 250 game apps, some for children, reported to listen for TV ads while idle.
- Hypothetical: bank keeps register of every third-party script on login + payment pages; any script w/o stated reason removed, rest listed in privacy notice.

### Ads fund the product: target on what?
- When: ads fund product.
- Do: sell attention on context, not profiles; advertisers measure results w/ own tagged links; analytics on own servers.
- Avoid: depending on platform controlling both audience + numbers; every visitor fed into identity graph in exchange for "free" analytics.
- Why: Respectful (advertising w/o granular tracking).
- Hypothetical: city events app sells ad slots by event category + counts visits on own server, sharing those totals w/ advertisers.

### Sensing + logging could make surveillance trivial: how much protection?
- When: sensing + logging could make surveillance trivial.
- Do: real-world privacy rule: aim for physical world's protections, no more + no less, where intrusion possible only w/ effort + always leaves evidence. Encrypt + pseudonymise data; prefer decentralised + end-to-end designs; support two-factor authentication + secure credential storage.
- Avoid: silent access to personal records leaving no evidence.
- Why: Resilient.
- Hypothetical: health-records portal shows each patient log of every staff member opening their file + when; encrypts records so anyone copying database cannot read them.

### Device would listen, watch or record in background: under what conditions?
- When: device would listen, watch or record in background.
- Do: indicate clearly when device listening; physical mute; explicit, repeated consent for background action; ambient recordings stored locally by default.
- Avoid: home camera or robot patrolling + recording by default; luxury surveillance = surveillance sold as convenience + later handed to police w/o owner's consent.
- Why: Intentional (question ambient, always-on collection). Buyer's comfort = consent from buyer alone, never from everyone device captures. Recordings later read by parties buyer never pictured: neighbours, employers, partners, police, stalkers. Buying rests on belief buyer's own life holds nothing worth watching.
- Misreading: Wrong: customer demand for surveillance device = permission → Right: not permission granted by people it films.
- Hypothetical: voice-controlled oven asks again each time before running background task + keeps recordings on appliance.
- Hypothetical: robot vacuum maps rooms w/o filming people, never sets off on patrol by itself + keeps map inside home unit.

### Continuous log of presence, location or activity: how long to keep it?
- When: product keeps continuous log of presence, location, viewing or nearby activity.
- Do: decide in advance what records others may request later → fix retention window before launch. Shortest history doing job, aged out automatically. State what product keeps + how long.
- Symptom → finding: open-ended retention defended as "we may need it later" = review finding.
- Why: continuous log lets someone ask past questions nobody thought to ask then: person's whereabouts, what they lingered over, others present in room. Harm concentrates in this retrospective power, not in any single capture.
- Hypothetical: car-sharing app keeps trip routes only until trip billed, then ages them out automatically; privacy page states retention window.

## Related
- defaults-and-choice-architecture.md: opt-in for collecting + sharing data, no preselected consent, equal-weight decline, symmetric exit for cancellation + account deletion.
- transparency-and-honesty.md: honest controls, true cost, honesty tests.
- forms-and-data-entry.md: usability side: fields, formats + validation timing.
- safety-and-abuse-resistance.md: misuse cases, blocking + reporting, vulnerable people + children.
- calm-technology-and-device-etiquette.md: peripheral attention, quiet signalling, failing gracefully; manners for ambient + connected devices.
- ../evidence/personalization-and-surveillance.md: evidence on tracking, inference + data misuse.
- ../checklists/calm-technology-scorecard.md: scores product on attention, notifications, privacy, well-being + failure states.
- ../principles/transparent.md: principle most privacy patterns serve.
